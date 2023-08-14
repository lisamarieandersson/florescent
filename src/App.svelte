<script lang="ts">
  import Footer from './Footer.svelte';
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
  <Presentation />
</main>

<footer>
  <Footer />
</footer>

<style>
</style>
