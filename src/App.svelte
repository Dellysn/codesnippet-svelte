<script>
  import NavBar from "./components/NavBar.svelte";
  import About from "./pages/About.svelte";
  import Contact from "./pages/Contact.svelte";
  import Service from "./pages/Service.svelte";
  import Pricing from "./pages/Pricing.svelte";
  import Team from "./pages/Team.svelte";
  import Testimonial from "./pages/Testimonial.svelte";
  import Home from "./pages/Home.svelte";
  import Promo from "./pages/Promo.svelte";
  import Footer from "./components/Footer.svelte";
</script>

<style>
</style>

<NavBar />
<main>
  <Home />
  <About />
  <Service />
  <Team />
  <Promo />
  <Pricing />
  <Testimonial />
  <Contact />
  <Footer />
</main>
