<script>
  import { Hamburger } from 'svelte-hamburgers';
  import Menu from './Menu.svelte';

  let open;
</script>

<div class="header-container">
  <div class="right-content">
    <div class="mobile-hamburger">
      <Hamburger
        --border-radius="0"
        --layer-height="0.10rem"
        --layer-spacing="0.5rem"
        --layer-width="1.7rem"
        --padding="0"
        bind:open
      />
    </div>
    <img
      class="logo-desktop"
      src="../logotyp-florescent.svg"
      alt="Florescent Logo"
    />
  </div>
  <div class="centered-content centered-logo">
    <Menu />
    <img
      class="logo-mobile"
      src="../logotyp-florescent.svg"
      alt="Florescent Logo"
    />
  </div>
  <div class="left-content">
    <span class="material-symbols-outlined"> shopping_bag </span>
  </div>
</div>

<style>
  .header-container {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    align-items: center;
    height: 6.125rem;
    padding: 0 1.5rem;
    /* border: solid 0.025rem #000000; */
  }

  .mobile-hamburger {
    display: none;
  }

  .logo-desktop {
    padding-left: 0.5rem;
    width: 12rem;
    height: auto;
  }

  .logo-mobile {
    width: 12rem;
    height: auto;
    display: none;
  }

  .left-content {
    text-align: right;
  }
  .material-symbols-outlined {
    font-size: 2rem;
  }

  /* Media query for mobile and tablet screens */
  @media (max-width: 768px) {
    .header-container {
      padding-left: 0.938rem;
      padding-right: 0.938rem;
    }
    .logo-desktop {
      display: none;
    }

    .logo-mobile {
      display: block;
    }

    .centered-logo {
      display: flex;
      justify-content: center;
      align-items: center;
    }
    .mobile-hamburger {
      display: block;
      padding-left: 0.5rem;
    }
  }
</style>
