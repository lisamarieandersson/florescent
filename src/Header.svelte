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
        --layer-width="1.6rem"
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
    height: 5rem;
    padding: 0 49.375rem;
  }

  .mobile-hamburger {
    display: none;
  }

  .logo-desktop {
    padding-left: 0.625rem;
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
    font-size: 2.2rem;
    padding-right: 0.106rem;
  }

  /* Media query for large desktop screens */
  @media (max-width: 2560px) {
    .header-container {
      padding: 0 29.375rem;
    }
  }

  /* Media queries for standard desktop screens */
  @media (max-width: 1920px) {
    .header-container {
      padding: 0 1.5rem;
    }
  }

  /* Media query for tablet and mobile screens */
  @media (max-width: 768px) {
    .header-container {
      padding: 0 0.938rem;
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

  /* Media query for smaller mobile screens */
  @media (max-width: 280px) {
    .logo-mobile {
      width: 9rem;
    }

    .material-symbols-outlined {
      font-size: 2.1rem;
    }
  }
</style>
