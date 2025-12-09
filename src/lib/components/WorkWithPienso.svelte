<script lang="ts">
  const steps = [
    {
      id: "01",
      title: "Structured or unstructured",
      description: "Whether you're a non-technical type, a data scientist, or an analyst — and whether your data is structured or raw — Pienso can help you categorize, label and analyze it. Imprint your intuitive knowledge and categorizations. Instead of one general LLM, use the best model for your need.",
      image: "https://placehold.co/1000x600/e0f2fe/0369a1?text=Structured+Data+Interface"
    },
    {
      id: "02",
      title: "Experiment boundlessly.",
      description: "Sculpt each topic and imprint your intuitive knowledge with nuanced labels and categorizations. Instead of one general LLM, use the best model for your current need. Closed-source LLMs allow limited fine-tuning, they're nothing like the customization possible when you have complete control over your models — no changes when you deploy — that's the power of Pienso.",
      image: "https://placehold.co/1000x600/f0fdf4/166534?text=Experiment+Interface"
    },
    {
      id: "03",
      title: "Transparency.",
      description: "While some closed-source LLMs allow limited fine-tuning, they're nothing like the customization possible when you can see and change every parameter. Fine-tune your LLM and pay only when you deploy — that's the power of Pienso. LM in your own environment means you understand why your model makes the decisions it does.",
      image: "https://placehold.co/1000x600/fef2f2/991b1b?text=Transparency+Interface"
    },
    {
      id: "04",
      title: "Deploy and thrive.",
      description: "Closed-model providers like GPT-4 can suddenly change parameters, making them unreliable. With Pienso, you have complete control over your models — no changes that you haven't made yourself. Deploy your fine-tuned LLM in your own environment under your enterprise security. Accelerate deployment on cloud through our trusted low-latency partners like Core for the ideal combination of security and speed.",
      image: "https://placehold.co/1000x600/fffbeb/b45309?text=Deploy+Interface"
    },
    {
      id: "05",
      title: "Quickly and cost-effectively.",
      description: "Deploy your fine-tuned LLM in your own environment under your enterprise security. Accelerate deployment on cloud through our trusted low-latency partners like Core for the ideal combination of security and speed. Pay only for models deployed.",
      image: "https://placehold.co/1000x600/f3f4f6/1f2937?text=Cost+Effective+Interface"
    }
  ];
</script>

<section class="bg-pienso-light-green py-24">
  <div class="container-custom space-y-32">
    {#each steps as step}
      <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-start">
        <!-- Text -->
        <div class="lg:col-span-4 sticky top-24">
          <h2 class="text-4xl md:text-5xl font-bold leading-tight mb-8">
            How to work with Pienso
          </h2>
          
          <div class="flex items-baseline justify-between border-t border-black/10 pt-4 mb-8">
             <span class="text-pienso-green font-bold text-2xl">{step.id}</span>
             <span class="font-bold text-2xl">/ 05</span>
          </div>

          <h3 class="text-2xl font-bold mb-4">{step.title}</h3>
          <p class="text-sm leading-relaxed text-gray-700">
            {step.description}
          </p>
        </div>

        <!-- Image -->
        <div class="lg:col-span-8">
          <div class="bg-white p-2 rounded-lg shadow-lg">
             <img src={step.image} alt={step.title} class="w-full h-auto rounded border border-gray-100" />
          </div>
        </div>
      </div>
    {/each}
  </div>
</section>
