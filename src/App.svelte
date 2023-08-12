<script lang="ts">
  import Header from './Header.svelte';
  import Hero from './Hero.svelte';
  import Presentation from './Presentation.svelte';
  import ProductContainer from './ProductContainer.svelte';
  import ToppBanner from './ToppBanner.svelte';
</script>

<header>
  <ToppBanner />
  <Header />
</header>

<main>
  <Hero />
  <Presentation />
  <ProductContainer />
</main>

<footer />

<style>
</style>
