<script>
  import Lenis from "lenis";
  import { browser } from "$app/environment";

  import Apropos from "../lib/components/Apropos.svelte";
  import Hero from "../lib/components/Hero.svelte";
  import Forfaits from "../lib/components/Forfaits.svelte";
  import Realisation from "../lib/components/Realisation.svelte";
  import Services from "../lib/components/Services.svelte";
  import FAQ from "../lib/components/FAQ.svelte";
  import Footer from "../lib/components/Footer.svelte";

  if (browser) {
    const lenis = new Lenis();

    function raf(time) {
      lenis.raf(time);
      requestAnimationFrame(raf);
    }

    requestAnimationFrame(raf);
  }
</script>

<Hero />
<Apropos />
<Services />
<Realisation />
<Forfaits />
<FAQ />
<Footer />
