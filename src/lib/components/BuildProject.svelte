<script lang="ts">
  import Button from './Button.svelte';
</script>

<section class="bg-white py-24 border-t border-gray-100">
  <div class="container-custom mb-16 flex flex-col md:flex-row justify-between items-end gap-8">
    <h2 class="text-4xl font-bold tracking-tight">Build your own project</h2>
    <Button variant="primary" className="bg-pienso-blue hover:bg-sky-500 text-white rounded-none">Book a demo</Button>
  </div>

  <div class="container-custom overflow-x-auto">
    <div class="min-w-[800px] flex items-center justify-between relative py-20">
      <!-- Connecting Line -->
      <div class="absolute top-1/2 left-0 w-full h-1 bg-gray-100 -z-10 transform -translate-y-1/2"></div>

      <!-- Step 1: Ingest -->
      <div class="relative group">
        <div class="text-xs font-bold uppercase mb-4 text-center">Ingest</div>
        <div class="w-40 h-40 bg-pienso-red transform -skew-x-12 shadow-lg flex items-center justify-center">
            <div class="w-32 h-32 border-2 border-white/20"></div>
        </div>
      </div>

      <!-- Arrow -->
      <div class="text-gray-300">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M5 12h14M12 5l7 7-7 7"/></svg>
      </div>

      <!-- Step 2: Annotate -->
      <div class="relative group">
        <div class="text-xs font-bold uppercase mb-4 text-center">Annotate</div>
        <div class="w-40 h-40 bg-pienso-blue transform rotate-3 shadow-lg flex items-center justify-center">
             <div class="w-32 h-32 border-2 border-white/20 rounded-full"></div>
        </div>
      </div>

      <!-- Arrow -->
      <div class="text-gray-300">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M5 12h14M12 5l7 7-7 7"/></svg>
      </div>

      <!-- Step 3: Deep Learning -->
      <div class="relative group">
        <div class="text-xs font-bold uppercase mb-4 text-center">Deep Learning</div>
        <div class="w-40 h-40 bg-pienso-green transform -rotate-6 shadow-lg flex items-center justify-center">
             <div class="w-32 h-32 border-2 border-white/20"></div>
        </div>
      </div>

      <!-- Arrow -->
      <div class="text-gray-300">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M5 12h14M12 5l7 7-7 7"/></svg>
      </div>

      <!-- Step 4: Explore -->
      <div class="relative group">
        <div class="text-xs font-bold uppercase mb-4 text-center">Explore</div>
        <div class="w-40 h-40 bg-gray-200 rounded-full shadow-lg flex items-center justify-center border-4 border-gray-100">
             <div class="w-20 h-20 bg-gray-300 rounded-full"></div>
        </div>
      </div>
    </div>
  </div>
</section>
