<script>
  import BackgroundGradient from "./ui/BackgroundGradient/BackgroundGradient.svelte";
</script>

<section class="hero min-h-screen bg-[#06070b]" id="realisations">
  <div class="container px-6 py-10 mx-auto">
    <h2 class="text-center text-clampTitle font-bold pb-6 text-white">
      Réalisations
    </h2>
    <div
      class="grid grid-cols-1 gap-8 mt-8 xl:mt-12 xl:gap-12 sm:grid-cols-2 xl:grid-cols-4 lg:grid-cols-3"
    >
      <!-- Video 1 -->
      <BackgroundGradient class="rounded-xl max-w-sm p-4 sm:p-10 ">
        <div class="w-full video-container cursor-pointer">
          <iframe
            src="https://drive.google.com/file/d/1I9WPJeC3VzkOv-qVmSxHRjYWoyqU4q0u/preview"
            allow="autoplay"
          ></iframe>
        </div>
      </BackgroundGradient>

      <!-- Video 2 -->
      <BackgroundGradient class="rounded-xl max-w-sm p-4 sm:p-10 ">
        <div class="w-full video-container cursor-pointer">
          <iframe
            src="https://drive.google.com/file/d/1zWR8XV-h3_egTbGK5y52QIoFiShV00jL/preview"
            width="640"
            height="480"
            allow="autoplay"
          ></iframe>
        </div>
      </BackgroundGradient>

      <!-- Video 3 -->
      <BackgroundGradient class="rounded-xl max-w-sm p-4 sm:p-10 ">
        <div class="w-full video-container cursor-pointer">
          <iframe
            src="https://drive.google.com/file/d/1x4C8GRWpQNp1RaObcxfZMvrq3fO-UO1Y/preview"
            width="640"
            height="480"
            allow="autoplay"
          ></iframe>
        </div>
      </BackgroundGradient>

      <!-- Video 4 -->
      <BackgroundGradient class="rounded-xl max-w-sm p-4 sm:p-10 ">
        <div class="w-full video-container cursor-pointer">
          <iframe
            src="https://drive.google.com/file/d/1MLdQF7-AUA3XrzyNHF-gMS_oD9A2JnQe/preview"
            width="640"
            height="480"
            allow="autoplay"
          ></iframe>
        </div>
      </BackgroundGradient>

      <!-- Video 5 -->
      <BackgroundGradient class="rounded-xl max-w-sm p-4 sm:p-10 ">
        <div class="w-full video-container cursor-pointer">
          <iframe
            src="https://drive.google.com/file/d/1gBvAq1pBj6vCtigeJa_hpO2Gy0MHm2gd/preview"
            width="640"
            height="480"
            allow="autoplay"
          ></iframe>
        </div>
      </BackgroundGradient>

      <!-- Video 6 -->
      <BackgroundGradient class="rounded-xl max-w-sm p-4 sm:p-10 ">
        <div class="w-full video-container cursor-pointer">
          <iframe
            src="https://drive.google.com/file/d/1e49rZsejdfJK6iiNcfvon0HI_HJHUZpR/preview"
            width="640"
            height="480"
            allow="autoplay"
          ></iframe>
        </div>
      </BackgroundGradient>

      <!-- Video 7 -->
      <BackgroundGradient class="rounded-xl max-w-sm p-4 sm:p-10 ">
        <div class="w-full video-container cursor-pointer">
          <iframe
            src="https://drive.google.com/file/d/19H9yva1PG-mNIiMevDBPM8-CnDUkZ1Zl/preview"
            width="640"
            height="480"
            allow="autoplay"
          ></iframe>
        </div>
      </BackgroundGradient>

      <!-- Video 8 -->
      <BackgroundGradient class="rounded-xl max-w-sm p-4 sm:p-10 ">
        <div class="w-full video-container cursor-pointer">
          <iframe
            src="https://drive.google.com/file/d/1YqznRYMlePMO658BXGEW58lG8-H1-Hz4/preview"
            width="640"
            height="480"
            allow="autoplay"
          ></iframe>
        </div>
      </BackgroundGradient>
    </div>
  </div>
</section>

<style>
  /* Ajoutez ce code CSS */
  @media screen and (max-width: 640px) {
    .video-container {
      max-width: 300px;
      margin: auto;
    }
  }

  .video-container {
    position: relative;
    width: 100%;
    padding-bottom: 177.78%; /* 16:9 ratio, 9/16 = 0.5625, 100 / 0.5625 = 177.78 */
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
  .background-gradient {
    background: linear-gradient(to right, #fff, #e0e0e0); /* Example gradient */
    padding: 20px;
    border-radius: 1rem;
    max-width: 320px;
    margin: 0 auto;
  }
</style>
