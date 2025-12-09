<script lang="ts">
  import Button from './Button.svelte';
  
  let isMenuOpen = false;
</script>

<header class="bg-pienso-green text-black py-4 px-6 md:px-12">
  <div class="container-custom flex items-center justify-between">
    <!-- Logo -->
    <a href="/" class="text-3xl font-bold tracking-tighter flex items-center gap-2">
      <span class="font-display">pienso</span>
    </a>

    <!-- Desktop Navigation -->
    <nav class="hidden md:flex items-center gap-8 text-sm font-medium">
      <div class="group relative cursor-pointer">
        <span class="flex items-center gap-1">Platform <svg width="10" height="6" viewBox="0 0 10 6" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M1 1L5 5L9 1" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></svg></span>
      </div>
      <div class="group relative cursor-pointer">
        <span class="flex items-center gap-1">Use Cases <svg width="10" height="6" viewBox="0 0 10 6" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M1 1L5 5L9 1" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></svg></span>
      </div>
      <div class="group relative cursor-pointer">
        <span class="flex items-center gap-1">Resources <svg width="10" height="6" viewBox="0 0 10 6" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M1 1L5 5L9 1" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></svg></span>
      </div>
      <div class="group relative cursor-pointer">
        <span class="flex items-center gap-1">Company <svg width="10" height="6" viewBox="0 0 10 6" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M1 1L5 5L9 1" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></svg></span>
      </div>
    </nav>

    <!-- CTA -->
    <div class="hidden md:block">
      <a href="/demo" class="text-sm font-medium hover:opacity-80 transition-opacity">Book a demo</a>
    </div>

    <!-- Mobile Menu Button -->
    <button class="md:hidden" on:click={() => isMenuOpen = !isMenuOpen}>
      <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
        <path d="M4 6h16M4 12h16M4 18h16" />
      </svg>
    </button>
  </div>
</header>
