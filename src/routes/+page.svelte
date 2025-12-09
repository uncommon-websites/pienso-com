<script lang="ts">
  import Header from "$lib/components/Header.svelte";
  import Hero from "$lib/components/Hero.svelte";
  import ImageBanner from "$lib/components/ImageBanner.svelte";
  import Manifesto from "$lib/components/Manifesto.svelte";
  import Quote from "$lib/components/Quote.svelte";
  import Process from "$lib/components/Process.svelte";
  import PromptFactory from "$lib/components/PromptFactory.svelte";
  import UseCasesList from "$lib/components/UseCasesList.svelte";
  import BuildProject from "$lib/components/BuildProject.svelte";
  import WorkWithPienso from "$lib/components/WorkWithPienso.svelte";
  import Features from "$lib/components/Features.svelte";
  import Security from "$lib/components/Security.svelte";
  import FooterCTA from "$lib/components/FooterCTA.svelte";
  import Footer from "$lib/components/Footer.svelte";
</script>

<div class="min-h-screen flex flex-col">
  <Header />
  
  <main class="flex-grow">
    <Hero />
    <ImageBanner />
    <Manifesto />
    <Quote />
    <Process />
    <PromptFactory />
    <UseCasesList />
    <BuildProject />
    <WorkWithPienso />
    <Features />
    <Security />
    <FooterCTA />
  </main>

  <Footer />
</div>

