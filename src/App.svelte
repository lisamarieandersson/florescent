<script lang="ts">
  import Contact from './Contact.svelte';
  import Footer from './Footer.svelte';
  import Header from './Header.svelte';
  import Hero from './Hero.svelte';
  import Presentation from './Presentation.svelte';
  import ProductContainer from './ProductContainer.svelte';
  import ShopNowCollage from './ShopNowCollage.svelte';
  import ToppBanner from './ToppBanner.svelte';
</script>

<header>
  <ToppBanner />
  <Header />
</header>

<main>
  <Hero />
  <ShopNowCollage />
  <ProductContainer />
  <Presentation />
  <Contact />
</main>

<footer>
  <Footer />
</footer>

<style>
</style>
