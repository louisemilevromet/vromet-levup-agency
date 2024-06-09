<script>
  import CardContainer from "./ui/ThreeDCardEffect/CardContainer.svelte";
  import CardItem from "./ui/ThreeDCardEffect/CardItem.svelte";

  let isMouseEntered = false;

  // Function to handle mouse enter and leave events
  function handleMouseEnter(event) {
    const svg = event.currentTarget.querySelector("svg path");
    svg.setAttribute("fill", "url(#grad1)");
  }

  function handleMouseLeave(event) {
    const svg = event.currentTarget.querySelector("svg path");
    svg.setAttribute("fill", "currentColor");
  }

  const openLink = (url) => {
    window.open(url, "_blank");
  };
</script>

<section class="hero min-h-screen bg-[#06070b]" id="apropos">
  <div class="container px-6 py-10 mx-auto">
    <!-- <h2 class="text-center text-clampTitle font-bold pb-6 text-white">
      À propos du fondateur
    </h2> -->

    <div
      class="flex lg:flex-row gap-[10vw] mt-8 xl:mt-12 flex-col items-center"
    >
      <CardContainer bind:isMouseEntered={isMouseEntered} class="">
        <CardItem
          isMouseEntered={isMouseEntered}
          translateZ="20"
          className="w-full"
        >
          <img
            src="/LouisEmileVromet.png"
            class=" rounded-xl object-cover group-hover/card:shadow-xl bg-[#282828]"
            alt="Louis-Émile Vromet"
          />
        </CardItem>
      </CardContainer>

      <div class="text-left self-start">
        <h3 class="text-white font-bold text-4xl pb-10">
          À propos du fondateur
        </h3>
        <p class="pb-10 text-custom-grey">
          Résidant à Québec, je suis passionné par le digital avec une formation
          collégiale en technique d'intégration multimédia. Cela fait plus d'un
          ans que j'offre mes services en tant que monteur vidéo. J'ai travaillé
          avec plusieurs particuliers pour les aider à atteindre leurs objectifs
          en matière de contenu vidéo.
        </p>
        <h3 class="text-white font-bold text-4xl pb-10">À propos de LEVup</h3>
        <p class="pb-10 text-custom-grey">
          LEVup est une agence de marketing spécialisée dans la création de
          contenu vidéo pour les PME et entrepreneurs. Nous aidons nos clients à
          augmenter leur chiffre d'affaires grâce à des vidéos de haute qualité
          et des campagnes publicitaires stratégiques.
        </p>
        <div class="flex flex-row gap-10 justify-between flex-wrap">
          <div class="flex flex-row gap-4 lg:justify-start justify-center">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="20"
              height="20"
              fill="currentColor"
              class="bi bi-envelope"
              viewBox="0 0 16 16"
            >
              <path
                d="M0 4a2 2 0 0 1 2-2h12a2 2 0 0 1 2 2v8a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2zm2-1a1 1 0 0 0-1 1v.217l7 4.2 7-4.2V4a1 1 0 0 0-1-1zm13 2.383-4.708 2.825L15 11.105zm-.034 6.876-5.64-3.471L8 9.583l-1.326-.795-5.64 3.47A1 1 0 0 0 2 13h12a1 1 0 0 0 .966-.741M1 11.105l4.708-2.897L1 5.383z"
              />
            </svg>
            <p class="text-custom-grey">louisemilevromet@gmail.com</p>
          </div>
          <div class="flex flex-row gap-4 lg:justify-start justify-center">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="20"
              height="20"
              fill="currentColor"
              class="bi bi-telephone"
              viewBox="0 0 16 16"
            >
              <path
                d="M3.654 1.328a.678.678 0 0 0-1.015-.063L1.605 2.3c-.483.484-.661 1.169-.45 1.77a17.6 17.6 0 0 0 4.168 6.608 17.6 17.6 0 0 0 6.608 4.168c.601.211 1.286.033 1.77-.45l1.034-1.034a.678.678 0 0 0-.063-1.015l-2.307-1.794a.68.68 0 0 0-.58-.122l-2.19.547a1.75 1.75 0 0 1-1.657-.459L5.482 8.062a1.75 1.75 0 0 1-.46-1.657l.548-2.19a.68.68 0 0 0-.122-.58zM1.884.511a1.745 1.745 0 0 1 2.612.163L6.29 2.98c.329.423.445.974.315 1.494l-.547 2.19a.68.68 0 0 0 .178.643l2.457 2.457a.68.68 0 0 0 .644.178l2.189-.547a1.75 1.75 0 0 1 1.494.315l2.306 1.794c.829.645.905 1.87.163 2.611l-1.034 1.034c-.74.74-1.846 1.065-2.877.702a18.6 18.6 0 0 1-7.01-4.42 18.6 18.6 0 0 1-4.42-7.009c-.362-1.03-.037-2.137.703-2.877z"
              />
            </svg>
            <p class="text-custom-grey">+1 (418) 552-6074</p>
          </div>
          <ul class="flex lg:justify-start justify-center flex-row gap-4">
            <li
              class="cursor-pointer icon-container"
              on:mouseenter={handleMouseEnter}
              on:mouseleave={handleMouseLeave}
              on:click={() =>
                openLink("https://www.instagram.com/louisss_emile/")}
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="22"
                height="22"
                fill="currentColor"
                class="bi bi-instagram"
                viewBox="0 0 16 16"
              >
                <defs>
                  <linearGradient id="grad1" x1="0%" y1="0%" x2="100%" y2="0%">
                    <stop offset="0%" stop-color="#3483CD" />
                    <stop offset="100%" stop-color="#1BC178" />
                  </linearGradient>
                </defs>
                <path
                  d="M8 0C5.829 0 5.556.01 4.703.048 3.85.088 3.269.222 2.76.42a3.9 3.9 0 0 0-1.417.923A3.9 3.9 0 0 0 .42 2.76C.222 3.268.087 3.85.048 4.7.01 5.555 0 5.827 0 8.001c0 2.172.01 2.444.048 3.297.04.852.174 1.433.372 1.942.205.526.478.972.923 1.417.444.445.89.719 1.416.923.51.198 1.09.333 1.942.372C5.555 15.99 5.827 16 8 16s2.444-.01 3.298-.048c.851-.04 1.434-.174 1.943-.372a3.9 3.9 0 0 0 1.416-.923c.445-.445.718-.891.923-1.417.197-.509.332-1.09.372-1.942C15.99 10.445 16 10.173 16 8s-.01-2.445-.048-3.299c-.04-.851-.175-1.433-.372-1.941a3.9 3.9 0 0 0-.923-1.417A3.9 3.9 0 0 0 13.24.42c-.51-.198-1.092-.333-1.943-.372C10.443.01 10.172 0 7.998 0zm-.717 1.442h.718c2.136 0 2.389.007 3.232.046.78.035 1.204.166 1.486.275.373.145.64.319.92.599s.453.546.598.92c.11.281.24.705.275 1.485.039.843.047 1.096.047 3.231s-.008 2.389-.047 3.232c-.035.78-.166 1.203-.275 1.485a2.5 2.5 0 0 1-.599.919c-.28.28-.546.453-.92.598-.28.11-.704.24-1.485.276-.843.038-1.096.047-3.232.047s-2.39-.009-3.233-.047c-.78-.036-1.203-.166-1.485-.276a2.5 2.5 0 0 1-.92-.598 2.5 2.5 0 0 1-.6-.92c-.109-.281-.24-.705-.275-1.485-.038-.843-.046-1.096-.046-3.233s.008-2.388.046-3.231c.036-.78.166-1.204.276-1.486.145-.373.319-.64.599-.92s.546-.453.92-.598c.282-.11.705-.24 1.485-.276.738-.034 1.024-.044 2.515-.045zm4.988 1.328a.96.96 0 1 0 0 1.92.96.96 0 0 0 0-1.92m-4.27 1.122a4.109 4.109 0 1 0 0 8.217 4.109 4.109 0 0 0 0-8.217m0 1.441a2.667 2.667 0 1 1 0 5.334 2.667 2.667 0 0 1 0-5.334"
                />
              </svg>
            </li>
            <li
              class="cursor-pointer icon-container"
              on:mouseenter={handleMouseEnter}
              on:mouseleave={handleMouseLeave}
              on:click={() =>
                openLink(
                  "https://www.linkedin.com/in/louis-%C3%A9mile-vromet-5575a0267/"
                )}
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="22"
                height="22"
                fill="currentColor"
                class="bi bi-linkedin"
                viewBox="0 0 16 16"
              >
                <defs>
                  <linearGradient id="grad1" x1="0%" y1="0%" x2="100%" y2="0%">
                    <stop offset="0%" stop-color="#3483CD" />
                    <stop offset="100%" stop-color="#1BC178" />
                  </linearGradient>
                </defs>
                <path
                  d="M0 1.146C0 .513.526 0 1.175 0h13.65C15.474 0 16 .513 16 1.146v13.708c0 .633-.526 1.146-1.175 1.146H1.175C.526 16 0 15.487 0 14.854zm4.943 12.248V6.169H2.542v7.225zm-1.2-8.212c.837 0 1.358-.554 1.358-1.248-.015-.709-.52-1.248-1.342-1.248S2.4 3.226 2.4 3.934c0 .694.521 1.248 1.327 1.248zm4.908 8.212V9.359c0-.216.016-.432.08-.586.173-.431.568-.878 1.232-.878.869 0 1.216.662 1.216 1.634v3.865h2.401V9.25c0-2.22-1.184-3.252-2.764-3.252-1.274 0-1.845.7-2.165 1.193v.025h-.016l.016-.025V6.169h-2.4c.03.678 0 7.225 0 7.225z"
                />
              </svg>
            </li>
            <li
              class="cursor-pointer icon-container"
              on:mouseenter={handleMouseEnter}
              on:mouseleave={handleMouseLeave}
              on:click={() =>
                openLink(
                  "https://www.facebook.com/profile.php?id=100011321763721"
                )}
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="22"
                height="22"
                fill="currentColor"
                class="bi bi-facebook"
                viewBox="0 0 16 16"
              >
                <defs>
                  <linearGradient id="grad1" x1="0%" y1="0%" x2="100%" y2="0%">
                    <stop offset="0%" stop-color="#3483CD" />
                    <stop offset="100%" stop-color="#1BC178" />
                  </linearGradient>
                </defs>
                <path
                  d="M16 8.049c0-4.446-3.582-8.05-8-8.05C3.58 0-.002 3.603-.002 8.05c0 4.017 2.926 7.347 6.75 7.951v-5.625h-2.03V8.05H6.75V6.275c0-2.017 1.195-3.131 3.022-3.131.876 0 1.791.157 1.791.157v1.98h-1.009c-.993 0-1.303.621-1.303 1.258v1.51h2.218l-.354 2.326H9.25V16c3.824-.604 6.75-3.934 6.75-7.951"
                />
              </svg>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</section>

<style>
  .icon-container svg {
    transition: fill 0.3s ease;
  }

  ul {
    color: #a6aeb6;
  }
</style>
