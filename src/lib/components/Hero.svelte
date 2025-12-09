<script lang="ts">
  import Button from './Button.svelte';
</script>

<section class="relative bg-white pt-20 pb-20 overflow-hidden">
  <div class="container-custom grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
    <!-- Left: 3D Shapes -->
    <div class="relative h-[400px] w-full flex items-center justify-center">
      <!-- Abstract representation of the shapes using CSS/SVG -->
      <div class="relative w-full h-full">
        <!-- Red Cube-ish shape -->
        <div class="absolute top-10 left-10 w-32 h-32 bg-pienso-red transform rotate-12 rounded-xl shadow-xl z-10"></div>
        <!-- Blue Pyramid-ish shape -->
        <div class="absolute top-40 left-40 w-0 h-0 border-l-[60px] border-l-transparent border-r-[60px] border-r-transparent border-b-[100px] border-b-pienso-blue transform -rotate-12 z-20"></div>
        <!-- Grey Cylinder-ish shape -->
        <div class="absolute top-20 right-20 w-24 h-40 bg-gray-400 rounded-full transform rotate-45 opacity-50 z-0"></div>
      </div>
    </div>

    <!-- Right: Content -->
    <div class="max-w-xl">
      <h1 class="text-5xl md:text-7xl font-bold leading-[0.95] tracking-tight mb-8">
        For anyone with a data set and <span class="text-pienso-blue">a question.</span>
      </h1>
      
      <p class="text-lg md:text-xl text-gray-800 mb-10 leading-relaxed max-w-md">
        Use Machine Learning to explore language data without a single line of code.
        Experiment, train, and deploy effortlessly, with an interactive and responsive learning interface that imprints your expertise at AI scale.
      </p>

      <Button variant="primary" size="lg" className="bg-pienso-blue hover:bg-sky-500 text-white rounded-none px-8 py-3 text-sm font-bold">
        Book a demo
      </Button>
    </div>
  </div>
</section>
