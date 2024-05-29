<script lang="ts">
  export let showFade: boolean = true;
</script>

<div
  class="relative opacity-10 flex h-screen w-full items-center justify-center bg-black bg-grid-white/[0.2]"
>
  <!-- Radial gradient for the container to give a faded look -->
  {#if showFade}
    <div
      class="pointer-events-none absolute inset-0 flex items-center justify-center bg-black [mask-image:radial-gradient(ellipse_at_center,transparent_20%,black)]"
    ></div>
  {/if}
  <slot />
</div>
