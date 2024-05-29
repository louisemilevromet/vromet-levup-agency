<script>
  const handleClick = (url) => {
    window.open(url, "_blank");
  };

  const scrollTo = (section) => {
    console.log("ok");
    const scroll = document.getElementById(section);
    scroll.scrollIntoView({ behavior: "smooth" });
  };
</script>

<div class="navbar absolute top-0 z-10">
  <div class="navbar-start">
    <div class="dropdown">
      <div
        tabindex="0"
        role="button"
        class="btn btn-ghost lg:hidden hover:!bg-[#1f29371a]"
      >
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-5 w-5"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
          ><path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M4 6h16M4 12h8m-8 6h16"
          /></svg
        >
      </div>
      <ul
        tabindex="0"
        class="menu menu-sm dropdown-content mt-3 z-[1] p-2 shadow bg-[#06070b] rounded-box w-52"
      >
        <li
          on:click={() => {
            scrollTo("apropos");
          }}
        >
          <a class="active:!text-custom-grey">À Propos</a>
        </li>
        <li
          on:click={() => {
            scrollTo("services");
          }}
        >
          <a class="active:!text-custom-grey">Services</a>
        </li>
        <li
          on:click={() => {
            scrollTo("realisations");
          }}
        >
          <a class="active:!text-custom-grey">Réalisations</a>
        </li>
        <li
          on:click={() => {
            scrollTo("forfaits");
          }}
        >
          <a class="active:!text-custom-grey">Forfaits</a>
        </li>
      </ul>
    </div>
    <a class="btn btn-ghost text-xl hover:!bg-[#1f29371a]">LEVup Agency</a>
  </div>
  <div class="navbar-center hidden lg:flex">
    <ul class="menu menu-horizontal px-1">
      <li
        on:click={() => {
          scrollTo("apropos");
        }}
      >
        <a
          class="active:!bg-[#06070b] active:!text-custom-grey hover:!bg-[#1f29371a]"
          >À propos</a
        >
      </li>
      <li
        on:click={() => {
          scrollTo("services");
        }}
      >
        <a
          class="active:!bg-[#06070b] active:!text-custom-grey hover:!bg-[#1f29371a]"
          >Services</a
        >
      </li>
      <li
        on:click={() => {
          scrollTo("realisations");
        }}
      >
        <a
          class="active:!bg-[#06070b] active:!text-custom-grey hover:!bg-[#1f29371a]"
          >Réalisations</a
        >
      </li>
      <li
        on:click={() => {
          scrollTo("forfaits");
        }}
      >
        <a
          class="active:!bg-[#06070b] active:!text-custom-grey hover:!bg-[#1f29371a]"
          >Forfaits</a
        >
      </li>
    </ul>
  </div>
  <div class="navbar-end">
    <a href="mailto: louisemilevromet@gmail.com" class="btn">Nous contacter</a>
  </div>
</div>

<style>
  .navbar-start {
    color: white;
  }
  ul {
    color: white;
  }
  .navbar-end a {
    color: black;
    border-color: white;
    background-color: white;
  }
  .menu {
    font-size: 1rem;
  }
</style>
