<script>
  import { onMount } from "svelte";

  let isOpen = [];

  onMount(() => {
    // Initialize the isOpen array with false values for each FAQ item
    isOpen = new Array(10).fill(false);
  });

  function toggle(index) {
    isOpen = isOpen.map((item, i) => (i === index ? !item : false));
  }
</script>

<section class="hero min-h-screen bg-[#06070b]">
  <div class="container px-6 py-10 mx-auto z-10">
    <div class="rounded">
      <div class="flex flex-col md:flex-row">
        <div class="md:w-1/3">
          <div
            class="sticky inset-x-0 top-0 left-0 py-12 text-center md:text-left"
          >
            <h2 class="text-3xl text-white mb-8 font-bold">
              Questions fréquemment posées.
            </h2>
            <div class="mb-2 text-custom-grey">
              Pas trouvé de réponse à vos questionnements ?
            </div>
            <div class="text-white">
              Contactez-nous par n'importe quels réseaux sociaux !
            </div>
          </div>
        </div>
        <div class="md:w-2/3 pb-12">
          <div class="">
            <!-- FAQ 1 -->
            <div class="item px-6 py-6">
              <a
                href="#"
                class="flex items-center justify-between"
                on:click|preventDefault={() => toggle(0)}
              >
                <h3
                  class={isOpen[0]
                    ? "text-white font-bold"
                    : "font-bold text-custom-grey"}
                >
                  Pourquoi est-il important pour une PME d'utiliser le marketing
                  vidéo ?
                </h3>
                <svg
                  class={`w-5 h-5 ${isOpen[0] ? "transform rotate-180" : "text-gray-500"}`}
                  fill="none"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path d="M19 9l-7 7-7-7"></path>
                </svg>
              </a>
              {#if isOpen[0]}
                <div
                  class="mt-3 text-white"
                  on:click_outside={() => (isOpen[0] = false)}
                >
                  <p class="text-custom-grey">
                    Le marketing vidéo est crucial car il permet de capturer
                    l'attention de manière plus efficace que les textes ou
                    images seuls. Les vidéos peuvent augmenter significativement
                    l'engagement, améliorer le taux de conversion et aider à
                    construire une présence en ligne plus forte. Elles sont
                    également préférées par les algorithmes des réseaux sociaux,
                    augmentant ainsi votre visibilité.
                  </p>
                </div>
              {/if}
            </div>

            <!-- FAQ 2 -->
            <div class="item px-6 py-6">
              <a
                href="#"
                class="flex items-center justify-between"
                on:click|preventDefault={() => toggle(1)}
              >
                <h4
                  class={isOpen[1]
                    ? "text-white font-bold"
                    : "font-bold text-custom-grey"}
                >
                  Quel type de contenu vidéo créez-vous ?
                </h4>
                <svg
                  class={`w-5 h-5 ${isOpen[1] ? "transform rotate-180" : "text-gray-500"}`}
                  fill="none"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path d="M19 9l-7 7-7-7"></path>
                </svg>
              </a>
              {#if isOpen[1]}
                <div
                  class="mt-3 text-white"
                  on:click_outside={() => (isOpen[1] = false)}
                >
                  <p class="text-custom-grey">
                    Nous spécialisons dans la création de vidéos courtes
                    adaptées aux plateformes sociales comme Facebook, Instagram,
                    et TikTok, idéales pour captiver rapidement l'audience. Nous
                    produisons des vidéos éducatives, des témoignages, des
                    démonstrations de produits, et des vidéos promotionnelles
                    qui mettent en valeur vos services et produits de manière
                    créative et engageante.
                  </p>
                </div>
              {/if}
            </div>

            <!-- FAQ 3 -->
            <div class="item px-6 py-6">
              <a
                href="#"
                class="flex items-center justify-between"
                on:click|preventDefault={() => toggle(2)}
              >
                <h4
                  class={isOpen[2]
                    ? "text-white font-bold"
                    : "font-bold text-custom-grey"}
                >
                  Comment gérez-vous les campagnes publicitaires sur Google et
                  Meta ?
                </h4>
                <svg
                  class={`w-5 h-5 ${isOpen[2] ? "transform rotate-180" : "text-gray-500"}`}
                  fill="none"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path d="M19 9l-7 7-7-7"></path>
                </svg>
              </a>
              {#if isOpen[2]}
                <div
                  class="mt-3 text-white"
                  on:click_outside={() => (isOpen[2] = false)}
                >
                  <p class="text-custom-grey">
                    Nous créons et gérons des campagnes publicitaires ciblées en
                    utilisant des données démographiques et comportementales
                    pour atteindre précisément votre public cible. Nous
                    optimisons continuellement les campagnes pour assurer le
                    meilleur retour sur investissement, en ajustant les
                    stratégies basées sur les performances des annonces et les
                    interactions des utilisateurs.
                  </p>
                </div>
              {/if}
            </div>

            <!-- FAQ 4 -->
            <div class="item px-6 py-6">
              <a
                href="#"
                class="flex items-center justify-between text-custom-grey"
                on:click|preventDefault={() => toggle(3)}
              >
                <h4 class={isOpen[3] ? "text-white font-bold" : "font-bold"}>
                  Quel est l'avantage de publier régulièrement sur les réseaux
                  sociaux ?
                </h4>
                <svg
                  class={`w-5 h-5 ${isOpen[3] ? "transform rotate-180" : "text-gray-500"}`}
                  fill="none"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path d="M19 9l-7 7-7-7"></path>
                </svg>
              </a>
              {#if isOpen[3]}
                <div
                  class="mt-3 text-white"
                  on:click_outside={() => (isOpen[3] = false)}
                >
                  <p class="text-custom-grey">
                    Publier régulièrement sur les réseaux sociaux aide à
                    maintenir et à accroître votre visibilité en ligne, à
                    engager votre communauté et à renforcer la fidélité de la
                    clientèle. Cela crée également une image de marque cohérente
                    et dynamique qui attire de nouveaux clients et encourage les
                    interactions régulières avec votre marque.
                  </p>
                </div>
              {/if}
            </div>

            <!-- FAQ 5 -->
            <div class="item px-6 py-6">
              <a
                href="#"
                class="flex items-center justify-between"
                on:click|preventDefault={() => toggle(4)}
              >
                <h4
                  class={isOpen[4]
                    ? "text-white font-bold"
                    : "font-bold text-custom-grey"}
                >
                  Comment mesurerez-vous le succès de nos campagnes de marketing
                  digital ?
                </h4>
                <svg
                  class={`w-5 h-5 ${isOpen[4] ? "transform rotate-180" : "text-gray-500"}`}
                  fill="none"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path d="M19 9l-7 7-7-7"></path>
                </svg>
              </a>
              {#if isOpen[4]}
                <div
                  class="mt-3 text-white"
                  on:click_outside={() => (isOpen[4] = false)}
                >
                  <p class="text-custom-grey">
                    Nous utilisons une variété d'outils analytiques pour mesurer
                    le succès de vos campagnes de marketing digital, y compris
                    le trafic web, le taux de conversion, l'engagement sur les
                    réseaux sociaux, et le ROI des campagnes publicitaires. Nous
                    fournissons des rapports détaillés qui vous permettent de
                    voir les performances de chaque campagne et d'ajuster les
                    stratégies selon les résultats obtenus.
                  </p>
                </div>
              {/if}
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
