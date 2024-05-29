<script>
  import BackgroundGradient from "./ui/BackgroundGradient/BackgroundGradient.svelte";

  function startVideo(event) {
    const thumbnail = event.currentTarget;
    const iframe = thumbnail.nextElementSibling;
    iframe.src += "&autoplay=1";
    thumbnail.style.display = "none";
    iframe.style.display = "block";
  }
</script>

<section class="hero min-h-screen bg-[#06070b]" id="realisations">
  <div class="container px-6 py-10 mx-auto">
    <h2 class="text-center text-clampTitle font-bold pb-6 text-white">
      Réalisations
    </h2>
    <div
      class="grid grid-cols-1 gap-8 mt-8 xl:mt-12 xl:gap-12 sm:grid-cols-2 xl:grid-cols-4 lg:grid-cols-3"
    >
      <!-- Video 1 with Vimeo -->
      <BackgroundGradient class="rounded-xl max-w-sm p-4 sm:p-10">
        <div class="w-full video-container cursor-pointer">
          <div style="padding:177.78% 0 0 0;position:relative;">
            <iframe
              src="https://player.vimeo.com/video/951654954?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479"
              frameborder="0"
              allow="autoplay; fullscreen; picture-in-picture; clipboard-write"
              style="position:absolute;top:0;left:0;width:100%;height:100%;"
              title="2024-04-14-vromet5-v1"
            ></iframe>
          </div>
          <script src="https://player.vimeo.com/api/player.js"></script>
        </div>
      </BackgroundGradient>

      <!-- Video 2 with Vimeo -->
      <BackgroundGradient class="rounded-xl max-w-sm p-4 sm:p-10">
        <div class="w-full video-container cursor-pointer">
          <div style="padding:177.78% 0 0 0;position:relative;">
            <iframe
              src="https://player.vimeo.com/video/951657071?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479"
              frameborder="0"
              allow="autoplay; fullscreen; picture-in-picture; clipboard-write"
              style="position:absolute;top:0;left:0;width:100%;height:100%;"
              title="Vidéo 2"
            ></iframe>
          </div>
          <script src="https://player.vimeo.com/api/player.js"></script>
        </div>
      </BackgroundGradient>

      <!-- Video 3 with Vimeo -->
      <BackgroundGradient class="rounded-xl max-w-sm p-4 sm:p-10">
        <div class="w-full video-container cursor-pointer">
          <div style="padding:177.78% 0 0 0;position:relative;">
            <iframe
              src="https://player.vimeo.com/video/951660844?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479"
              frameborder="0"
              allow="autoplay; fullscreen; picture-in-picture; clipboard-write"
              style="position:absolute;top:0;left:0;width:100%;height:100%;"
              title="Vidéo 3"
            ></iframe>
          </div>
          <script src="https://player.vimeo.com/api/player.js"></script>
        </div>
      </BackgroundGradient>

      <!-- Video 4 with Vimeo -->
      <BackgroundGradient class="rounded-xl max-w-sm p-4 sm:p-10">
        <div class="w-full video-container cursor-pointer">
          <div style="padding:177.78% 0 0 0;position:relative;">
            <iframe
              src="https://player.vimeo.com/video/951663151?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479"
              frameborder="0"
              allow="autoplay; fullscreen; picture-in-picture; clipboard-write"
              style="position:absolute;top:0;left:0;width:100%;height:100%;"
              title="Vidéo 4"
            ></iframe>
          </div>
          <script src="https://player.vimeo.com/api/player.js"></script>
        </div>
      </BackgroundGradient>

      <!-- Video 5 with Vimeo -->
      <BackgroundGradient class="rounded-xl max-w-sm p-4 sm:p-10">
        <div class="w-full video-container cursor-pointer">
          <div style="padding:177.78% 0 0 0;position:relative;">
            <iframe
              src="https://player.vimeo.com/video/951664100?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479"
              frameborder="0"
              allow="autoplay; fullscreen; picture-in-picture; clipboard-write"
              style="position:absolute;top:0;left:0;width:100%;height:100%;"
              title="Vidéo 5"
            ></iframe>
          </div>
          <script src="https://player.vimeo.com/api/player.js"></script>
        </div>
      </BackgroundGradient>

      <!-- Video 6 with Vimeo -->
      <BackgroundGradient class="rounded-xl max-w-sm p-4 sm:p-10">
        <div class="w-full video-container cursor-pointer">
          <div style="padding:177.78% 0 0 0;position:relative;">
            <iframe
              src="https://player.vimeo.com/video/951666200?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479"
              frameborder="0"
              allow="autoplay; fullscreen; picture-in-picture; clipboard-write"
              style="position:absolute;top:0;left:0;width:100%;height:100%;"
              title="2024-03-04-ben7-v1"
            ></iframe>
          </div>
          <script src="https://player.vimeo.com/api/player.js"></script>
        </div>
      </BackgroundGradient>

      <!-- Video 7 with Vimeo -->
      <BackgroundGradient class="rounded-xl max-w-sm p-4 sm:p-10">
        <div class="w-full video-container cursor-pointer">
          <div style="padding:177.78% 0 0 0;position:relative;">
            <iframe
              src="https://player.vimeo.com/video/951741304?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479"
              frameborder="0"
              allow="autoplay; fullscreen; picture-in-picture; clipboard-write"
              style="position:absolute;top:0;left:0;width:100%;height:100%;"
              title="Vidéo 7"
            ></iframe>
          </div>
          <script src="https://player.vimeo.com/api/player.js"></script>
        </div>
      </BackgroundGradient>

      <!-- Video 8 with Vimeo -->
      <BackgroundGradient class="rounded-xl max-w-sm p-4 sm:p-10">
        <div class="w-full video-container cursor-pointer">
          <div style="padding:177.78% 0 0 0;position:relative;">
            <iframe
              src="https://player.vimeo.com/video/951741741?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479"
              frameborder="0"
              allow="autoplay; fullscreen; picture-in-picture; clipboard-write"
              style="position:absolute;top:0;left:0;width:100%;height:100%;"
              title="Vidéo 8"
            ></iframe>
          </div>
          <script src="https://player.vimeo.com/api/player.js"></script>
        </div>
      </BackgroundGradient>
    </div>
  </div>
</section>

<style>
  .video-container {
    position: relative;
    width: 100%;
    padding-bottom: 177.78%; /* 9:16 ratio */
    height: 0;
    overflow: hidden;
    border-radius: 1rem;
  }
  .video-container iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    border: 0;
  }
  .thumbnail {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-size: cover;
    background-position: center;
    cursor: pointer;
    display: flex;
    justify-content: center;
    align-items: center;
    color: white;
    font-size: 2rem;
  }
  .play-button {
    width: 80px;
    height: 80px;
    background: rgba(0, 0, 0, 0.6);
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 2rem;
    color: white;
  }
</style>
