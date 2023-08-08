<script>
  import Menu from './Menu.svelte';
</script>

<div class="header">
  <img src="../logotyp-florescent.svg" alt="Florescent Logo" />
  <Menu />
  <span class="material-symbols-outlined"> shopping_bag </span>
</div>

<style>
  .header {
    display: grid;
    grid-template-columns: 1fr auto 1fr;
    align-items: center;
    height: 6.125rem;
    background-color: #f2efea;
    padding-left: 2rem;
    padding-right: 2rem;
  }

  img {
    width: 10rem;
    height: auto;
    padding-left: 0.4rem;
  }

  .material-symbols-outlined {
    font-size: 2rem;
    text-align: right;
  }
</style>
