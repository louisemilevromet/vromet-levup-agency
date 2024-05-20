<script lang="ts">
  import { cn } from "$lib/utils";

  export let className: string | undefined = undefined;
  export let containerClassName: string | undefined = undefined;
  export let isMouseEntered = false;

  let containerRef: HTMLDivElement;

  const handleMouseMove = (e: MouseEvent) => {
    if (!containerRef) return;
    const { left, top, width, height } = containerRef.getBoundingClientRect();
    const offsetX = e.clientX - left; // position horizontale du curseur par rapport au coin supérieur gauche de l'image
    const offsetY = e.clientY - top; // position verticale du curseur par rapport au coin supérieur gauche de l'image
    const centerX = width / 2; // position horizontale du centre de l'image par rapport à son coin supérieur gauche
    const centerY = height / 2; // position verticale du centre de l'image par rapport à son coin supérieur gauche
    const deltaX = (offsetX - centerX) / 10; // différence horizontale entre la position du curseur et le centre de l'image
    const deltaY = (offsetY - centerY) / 10; // différence verticale entre la position du curseur et le centre de l'image
    containerRef.style.transform = `rotateY(${deltaX}deg) rotateX(${-deltaY}deg)`; // inversion du mouvement sur l'axe Y
  };

  const handleMouseEnter = (e: MouseEvent) => {
    isMouseEntered = true;
    if (!containerRef) return;
  };

  const handleMouseLeave = (e: MouseEvent) => {
    if (!containerRef) return;
    isMouseEntered = false;
    containerRef.style.transform = `rotateY(0deg) rotateX(0deg)`;
  };
</script>

<div
  class={cn("shrink-0 w-[50vw] max-w-sm shadow-2xl", containerClassName)}
  style="perspective: 1000px;"
>
  <div
    bind:this={containerRef}
    on:mouseenter={handleMouseEnter}
    on:mousemove={handleMouseMove}
    on:mouseleave={handleMouseLeave}
    class={cn(
      "relative flex items-center justify-center transition-all duration-200 ease-linear",
      className
    )}
    style="transform-style: preserve-3d;"
  >
    <slot />
  </div>
</div>
