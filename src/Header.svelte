<script>
  import { Hamburger } from 'svelte-hamburgers';
  import Menu from './Menu.svelte';

  let open;
</script>

<div class="header">
  <div>
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
  <Menu />
  <img
    class="logo-mobile"
    src="../logotyp-florescent.svg"
    alt="Florescent Logo"
  />
  <span class="material-symbols-outlined"> shopping_bag </span>
</div>

<style>
  .header {
    display: grid;
    grid-template-columns: 1fr auto 1fr;
    align-items: center;
    height: 6.125rem;
    padding-left: 2rem;
    padding-right: 2rem;
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
  .material-symbols-outlined {
    font-size: 2rem;
    text-align: right;
  }

  /* Media query for mobile screens */
  @media (max-width: 768px) {
    .header {
      padding-left: 1rem;
      padding-right: 1rem;
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
