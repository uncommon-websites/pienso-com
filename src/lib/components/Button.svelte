<script lang="ts">
  export let variant: 'primary' | 'secondary' | 'outline' | 'text' = 'primary';
  export let size: 'sm' | 'md' | 'lg' = 'md';
  export let href: string | undefined = undefined;
  export let className: string = '';

  const baseStyles = "inline-flex items-center justify-center font-medium transition-colors duration-200 focus:outline-none focus:ring-2 focus:ring-offset-2 disabled:opacity-50 disabled:pointer-events-none";
  
  const variants = {
    primary: "bg-pienso-blue hover:bg-sky-500 text-white",
    secondary: "bg-white text-pienso-text hover:bg-gray-50 border border-gray-200",
    outline: "border border-current bg-transparent hover:bg-white/10",
    text: "bg-transparent hover:bg-gray-100 text-pienso-text"
  };

  const sizes = {
    sm: "px-3 py-1.5 text-sm",
    md: "px-6 py-3 text-base",
    lg: "px-8 py-4 text-lg"
  };

  $: classes = `${baseStyles} ${variants[variant]} ${sizes[size]} ${className}`;
</script>

{#if href}
  <a {href} class={classes} {...$$restProps}>
    <slot />
  </a>
{:else}
  <button class={classes} {...$$restProps}>
    <slot />
  </button>
{/if}
