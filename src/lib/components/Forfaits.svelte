<script>
  const handleClick = (url) => {
    window.open(url, "_blank");
  };
</script>

<section class="hero min-h-screen bg-[#06070b]" id="forfaits">
  <div class="container px-6 py-10 mx-auto">
    <h2 class="text-center text-clampTitle font-bold pb-6 text-white">
      Nos Forfaits
    </h2>

    <div
      class="grid grid-cols-1 gap-8 sm:grid-cols-2 lg:grid-cols-3 mt-8 xl:mt-12"
    >
      <!-- Basic Plan -->
      <div
        class="bg-white rounded-lg shadow-lg p-6 relative overflow-hidden h-fit"
      >
        <div class="absolute top-0 right-0 m-4">
          <span
            class="inline-flex items-center px-3 py-1 rounded-full text-sm font-medium bg-purple-100 text-purple-800"
          >
            De Base
          </span>
        </div>
        <div class="mb-8">
          <h3 class="text-2xl font-semibold text-black">Présence Sociale</h3>
          <p class="mt-4 text-custom-black">
            Parfait pour les particuliers et les petites équipes.
          </p>
        </div>
        <!-- <div class="mb-8">
          <span class="text-5xl font-extrabold text-white">$49</span>
          <span class="text-xl font-medium text-custom-black">/mo</span>
        </div> -->
        <ul class="mb-8 space-y-4 text-custom-black">
          <li class="flex items-center">
            <svg
              class="h-6 w-6 text-green-400 mr-2"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M5 13l4 4L19 7"
              />
            </svg>
            <span>4 vidéos courtes par mois (1 par semaine)</span>
          </li>
          <li class="flex items-center">
            <svg
              class="h-6 w-6 text-green-400 mr-2"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M5 13l4 4L19 7"
              />
            </svg>
            <span>Gestion de 2 réseaux sociaux</span>
          </li>
          <li class="flex items-center">
            <svg
              class="h-6 w-6 text-green-400 mr-2"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M5 13l4 4L19 7"
              />
            </svg>
            <span>1 campagne publicitaire</span>
          </li>
        </ul>
        <a
          on:click={() =>
            handleClick("https://calendly.com/louisemilevromet/30min")}
          class="block w-full py-3 px-6 text-center rounded-md text-white font-medium bg-gradient hover:bg-gradientHover cursor-pointer"
        >
          Prendre un rendez-vous
        </a>
      </div>

      <!-- Pro Plan -->
      <div
        class="bg-white rounded-lg shadow-lg p-6 relative overflow-hidden h-fit"
      >
        <div class="absolute top-0 right-0 m-4">
          <span
            class="inline-flex items-center px-3 py-1 rounded-full text-sm font-medium bg-green-100 text-green-800"
          >
            Pro
          </span>
        </div>
        <div class="mb-8">
          <h3 class="text-2xl font-semibold text-black">Engagement Avancé</h3>
          <p class="mt-4 text-custom-black">
            Idéal pour les entreprises en croissance et les grandes entreprises
          </p>
        </div>
        <!-- <div class="mb-8">
          <span class="text-5xl font-extrabold text-white">$199</span>
          <span class="text-xl font-medium text-custom-black">/mo</span>
        </div> -->
        <ul class="mb-8 space-y-4 text-custom-black">
          <li class="flex items-center">
            <svg
              class="h-6 w-6 text-green-400 mr-2"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M5 13l4 4L19 7"
              />
            </svg>
            <span>8 vidéos courtes par mois (2 par semaine)</span>
          </li>
          <li class="flex items-center">
            <svg
              class="h-6 w-6 text-green-400 mr-2"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M5 13l4 4L19 7"
              />
            </svg>
            <span>Gestion de 3 réseaux sociaux</span>
          </li>
          <li class="flex items-center">
            <svg
              class="h-6 w-6 text-green-400 mr-2"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M5 13l4 4L19 7"
              />
            </svg>
            <span>2 campagnes publicitaires</span>
          </li>
        </ul>
        <a
          on:click={() =>
            handleClick("https://calendly.com/louisemilevromet/30min")}
          class="block w-full py-3 px-6 text-center rounded-md text-white font-medium bg-gradient hover:bg-gradientHover cursor-pointer"
        >
          Prendre un rendez-vous
        </a>
      </div>

      <!-- Enterprise Plan -->
      <div
        class="bg-white rounded-lg shadow-lg p-6 relative overflow-hidden h-fit"
      >
        <div class="absolute top-0 right-0 m-4">
          <span
            class="inline-flex items-center px-3 py-1 rounded-full text-sm font-medium bg-yellow-100 text-yellow-800"
          >
            Entreprise
          </span>
        </div>
        <div class="mb-8">
          <h3 class="text-2xl font-semibold text-black">Domination Digitale</h3>
          <p class="mt-4 text-custom-black">
            Adapté aux déploiements à grande échelle et aux besoins
            personnalisés
          </p>
        </div>
        <!-- <div class="mb-8">
          <span class="text-5xl font-extrabold text-white">Custom</span>
        </div> -->
        <ul class="mb-8 space-y-4 text-custom-black">
          <li class="flex items-center">
            <svg
              class="h-6 w-6 text-green-400 mr-2"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M5 13l4 4L19 7"
              />
            </svg>
            <span>12 vidéos courtes par mois (3 par semaine)</span>
          </li>
          <li class="flex items-center">
            <svg
              class="h-6 w-6 text-green-400 mr-2"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M5 13l4 4L19 7"
              />
            </svg>
            <span>Gestion de 4 réseaux sociaux</span>
          </li>
          <li class="flex items-center">
            <svg
              class="h-6 w-6 text-green-400 mr-2"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M5 13l4 4L19 7"
              />
            </svg>
            <span>3 campagnes publicitaires</span>
          </li>
          <li class="flex items-center">
            <svg
              class="h-6 w-6 text-green-400 mr-2"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M5 13l4 4L19 7"
              />
            </svg>
            <span
              >Analyse détaillée et optimisation continue des stratégies</span
            >
          </li>
        </ul>
        <a
          on:click={() =>
            handleClick("https://calendly.com/louisemilevromet/30min")}
          class="block w-full py-3 px-6 text-center rounded-md text-white font-medium bg-gradient hover:bg-gradientHover cursor-pointer"
        >
          Prendre un rendez-vous
        </a>
      </div>
    </div>
  </div>
</section>
