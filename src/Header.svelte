<script>
  import { Hamburger } from 'svelte-hamburgers';
  import Menu from './Menu.svelte';

  let open;
</script>

<div class="header">
  <div class="right-content">
    <div class="mobile-hamburger">
      <Hamburger
        --border-radius="0"
        --layer-height="0.15rem"
        --layer-spacing="0.5rem"
        --layer-width="1.7rem"
        --padding="0"
        bind:open
      />
    </div>
    <img
      class="logo-desktop-tablet"
      src="../logotyp-florescent.svg"
      alt="Florescent Logo"
    />
  </div>
  <div class="centered-content">
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
  .header {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    align-items: center;
    height: 6.125rem;
    padding: 0 1.5rem;
    border: solid 0.025rem #000000;
  }

  .mobile-hamburger {
    display: none;
  }

  .logo-desktop-tablet {
    padding-left: 0.5rem;
    width: 12rem;
    height: auto;
  }

  .logo-mobile {
    width: 12rem;
    height: auto;
  }

  .logo-mobile {
    display: none;
  }

  .left-content {
    text-align: right;
  }
  .material-symbols-outlined {
    font-size: 2rem;
  }

  /* Media query for mobile screens */
  @media (max-width: 768px) {
    .header {
      padding-left: 0.938rem;
      padding-right: 0.938rem;
    }
    .logo-desktop-tablet {
      display: none;
    }

    .logo-mobile {
      display: block;
    }
    .mobile-hamburger {
      display: block;
      padding-left: 0.5rem;
    }
  }
</style>
