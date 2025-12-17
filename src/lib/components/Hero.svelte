<script lang="ts">
  import SectionWrapper from './SectionWrapper.svelte';
</script>

<SectionWrapper withBorderBottom={true} className="py-20 md:py-24">
  <div class="px-4 md:px-12 max-w-4xl mx-auto text-center">
    <h1 class="font-serif text-5xl md:text-7xl text-gray-900 mb-6 leading-tight">
      Process invoices in <br/> seconds, not hours
    </h1>
    <p class="text-gray-500 text-lg md:text-xl max-w-2xl mx-auto mb-10 leading-relaxed font-light">
      Automated retrieval, AI-powered matching, and one-click payments. Join 1,000+ finance teams saving 1,000+ hours monthly with invoice automation that actually works.
    </p>
    <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
      <a href="#" class="inline-flex items-center px-6 py-3 bg-black text-white font-medium rounded hover:bg-gray-800 transition-colors">
        Start free trial <span class="ml-2">→</span>
      </a>
      <a href="#" class="inline-flex items-center px-6 py-3 border border-gray-300 text-gray-700 font-medium rounded hover:border-gray-400 transition-colors">
        Watch demo
      </a>
    </div>
    <p class="text-gray-400 text-sm mt-4">No credit card required • Setup in 2 minutes</p>
  </div>

  <div class="mt-16 md:mt-20 px-4 md:px-12">
    <div class="relative w-full aspect-[16/9] md:aspect-[21/9] rounded-lg overflow-hidden bg-gray-200 shadow-2xl">
      <img 
        src="/generated/image-finance-team-members-collaborating-at-a--1765976739509-0.webp" 
        alt="Finance team collaborating" 
        class="w-full h-full object-cover"
      />
    </div>
  </div>
</SectionWrapper>
