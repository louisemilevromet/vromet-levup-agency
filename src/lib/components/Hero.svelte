<script>
  import NavBar from "./NavBar.svelte";
  import DotBackground from "./ui/DotBackground/DotBackground.svelte";

  const handleClick = (section) => {
    const scroll = document.getElementById(section);
    scroll.scrollIntoView({ behavior: "smooth" });
  };
</script>

<div
  class="hero min-h-screen"
  style="background-image: url('/Background.png');"
>
  <NavBar />
  <DotBackground />

  <div class="hero-content text-center text-neutral-content">
    <div class="">
      <h1 class="mb-8 text-clampHero font-bold text-white">LEVup Agency.</h1>
      <p class="mb-8 text-custom-grey">
        Transformez vos clics en clients : Boostez votre visibilité en
        maximisant vos profits !
      </p>
      <div id="mouse-scroll" on:click={() => handleClick("apropos")}>
        <div class="mouse">
          <div class="mouse-in"></div>
        </div>
        <div>
          <span class="down-arrow-1"></span>
          <span class="down-arrow-2"></span>
          <span class="down-arrow-3"></span>
        </div>
      </div>
    </div>
  </div>
</div>

<style>
  body {
    background: #464646;
  }

  a {
    display: flex;
  }
  #mouse-scroll {
    display: flex;
    width: fit-content;
    margin: auto;
    flex-direction: column;
    align-items: center;
    cursor: pointer;
  }
  #mouse-scroll span {
    display: block;
    width: 5px;
    height: 5px;
    -ms-transform: rotate(45deg);
    -webkit-transform: rotate(45deg);
    transform: rotate(45deg);
    border-right: 2px solid #fff;
    border-bottom: 2px solid #fff;
    margin: 0 0 3px 0;
  }
  #mouse-scroll .mouse {
    height: 21px;
    width: 14px;
    border-radius: 10px;
    -webkit-transform: none;
    -ms-transform: none;
    transform: none;
    border: 2px solid #ffffff;
    top: 170px;
  }
  #mouse-scroll .down-arrow-1 {
    margin-top: 6px;
  }
  #mouse-scroll .down-arrow-1,
  #mouse-scroll .down-arrow-2,
  #mouse-scroll .down-arrow-3 {
    -webkit-animation: mouse-scroll 1s infinite;
    -moz-animation: mouse-scroll 1s infinite;
    animation: mouse-scroll 1s infinite;
  }
  #mouse-scroll .down-arrow-1 {
    -webkit-animation-delay: 0.1s;
    -moz-animation-delay: 0.1s;
    animation-delay: 0.1s;
    -webkit-animation-direction: alternate;
  }
  #mouse-scroll .down-arrow-2 {
    -webkit-animation-delay: 0.2s;
    -moz-animation-delay: 0.2s;
    animation-delay: 0.2s;
    -webkit-animation-direction: alternate;
  }
  #mouse-scroll .down-arrow-3 {
    -webkit-animation-delay: 0.3s;
    -moz-animation-delay: 0.3s;
    animation-delay: 0.3s;
    -webkit-animation-direction: alternate;
  }
  #mouse-scroll .mouse-in {
    height: 5px;
    width: 2px;
    display: block;
    margin: 5px auto;
    background: #ffffff;
    position: relative;
  }
  #mouse-scroll .mouse-in {
    -webkit-animation: animated-mouse 1.2s ease infinite;
    -moz-animation: mouse-animated 1.2s ease infinite;
    animation: animated-mouse 1.2s ease infinite;
  }

  @-webkit-keyframes animated-mouse {
    0% {
      opacity: 1;
      -webkit-transform: translateY(0);
      transform: translateY(0);
    }
    100% {
      opacity: 0;
      -webkit-transform: translateY(6px);
      transform: translateY(6px);
    }
  }
  @-webkit-keyframes mouse-scroll {
    0% {
      opacity: 1;
    }
    50% {
      opacity: 0.5;
    }
    100% {
      opacity: 1;
    }
  }
  @keyframes mouse-scroll {
    0% {
      opacity: 0;
    }
    50% {
      opacity: 0.5;
    }
    100% {
      opacity: 1;
    }
  }
</style>
