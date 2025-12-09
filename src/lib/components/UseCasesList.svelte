<script lang="ts">
  const cases = [
    {
      title: "Because language use is always evolving.",
      subtitle: "Content Moderation",
      description: "Flagging harmful or misleading content is one of today's biggest challenges. Pienso's Deep Learning enables nuanced moderation, while retraining models quickly and easily lets you keep pace.",
      iconColor: "bg-pienso-green",
      image: "https://placehold.co/400x300/f0fdf4/166534?text=Content+Moderation+UI"
    },
    {
      title: "Because customers tell you how they feel.",
      subtitle: "Customer Insights",
      description: "You'll likely have plenty of customer data — but are you using it fully? With Deep Learning, you can assess even subtle aspects like emotional response, evaluate agent performance, and predict churn, all of which help you retain customers.",
      iconColor: "bg-pienso-blue",
      image: "https://placehold.co/400x300/f0f9ff/0369a1?text=Customer+Insights+UI"
    },
    {
      title: "Because intel is hidden in your documents.",
      subtitle: "Document Intelligence",
      description: "About 80% of an organization's intel is buried in unstructured documents. Imprinting your language models with your nuanced understanding makes classification far more accurate — with benefits that range from better tagging to detecting areas of risk.",
      iconColor: "bg-pienso-red",
      image: "https://placehold.co/400x300/fef2f2/991b1b?text=Document+Intelligence+UI"
    },
    {
      title: "Because cyber criminals use AI too.",
      subtitle: "Document Intelligence",
      description: "Cyber crime is skyrocketing and everyone's at risk, as bad actors use the latest tech to circumvent security measures. Pienso helps you quickly and easily retrain models as their strategies evolve, keeping you a step ahead.",
      iconColor: "bg-gray-600",
      image: "https://placehold.co/400x300/f3f4f6/1f2937?text=Security+Analysis+UI"
    }
  ];
</script>

<section class="bg-white py-24">
  <div class="container-custom mb-24">
    <div class="grid grid-cols-1 md:grid-cols-2 gap-12">
      <h2 class="text-4xl md:text-5xl font-bold tracking-tight max-w-md">
        Deep Learning is in your future.
      </h2>
      <p class="text-lg text-gray-600 max-w-md ml-auto">
        Every specialist sector stands to benefit from the application of LLMs. Question, reflect, and invent new use cases — Pienso equips you with the tools to participate fully in the AI-powered world.
      </p>
    </div>
  </div>

  <div class="container-custom space-y-32">
    {#each cases as item}
      <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center border-t border-gray-100 pt-16">
        <!-- Icon -->
        <div class="lg:col-span-1">
          <div class={`w-12 h-12 ${item.iconColor} rounded-full flex items-center justify-center text-white`}>
            {#if item.subtitle === "Content Moderation"}
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"></path></svg>
            {:else if item.subtitle === "Customer Insights"}
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polygon points="12 2 15.09 8.26 22 9.27 17 14.14 18.18 21.02 12 17.77 5.82 21.02 7 14.14 2 9.27 8.91 8.26 12 2"></polygon></svg>
            {:else if item.title.includes("hidden in your documents")}
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline><line x1="16" y1="13" x2="8" y2="13"></line><line x1="16" y1="17" x2="8" y2="17"></line><polyline points="10 9 9 9 8 9"></polyline></svg>
            {:else}
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="3" y="11" width="18" height="11" rx="2" ry="2"></rect><path d="M7 11V7a5 5 0 0 1 10 0v4"></path></svg>
            {/if}
          </div>
        </div>

        <!-- Text -->
        <div class="lg:col-span-4">
          <h3 class="text-2xl font-bold mb-8 leading-tight">{item.title}</h3>
          
          <div class="space-y-4">
            <h4 class="font-bold text-sm uppercase tracking-wide">{item.subtitle}</h4>
            <p class="text-sm text-gray-600 leading-relaxed">
              {item.description}
            </p>
          </div>
        </div>

        <!-- Image -->
        <div class="lg:col-span-6 lg:col-start-7">
          <div class="bg-gray-50 rounded-lg p-4 shadow-sm">
            <img src={item.image} alt={item.subtitle} class="w-full h-auto rounded shadow-sm border border-gray-100" />
          </div>
        </div>
      </div>
    {/each}
  </div>
</section>
