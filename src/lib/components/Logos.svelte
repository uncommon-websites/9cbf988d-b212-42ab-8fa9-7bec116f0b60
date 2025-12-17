<script lang="ts">
  import SectionWrapper from './SectionWrapper.svelte';
</script>

<SectionWrapper withBorderBottom={true} className="py-12">
  <div class="px-4 md:px-12 flex flex-col md:flex-row items-center justify-between gap-8">
    <!-- Logos -->
    <div class="flex flex-wrap items-center gap-8 md:gap-12 grayscale opacity-60">
        <!-- OrderBilly -->
        <div class="h-6 font-bold text-lg tracking-tight">OrderBilly</div>
        <!-- Generic Company Names -->
        <div class="h-6 font-semibold text-base tracking-wide">TechFlow</div>
        <div class="h-6 font-medium text-base uppercase tracking-widest text-xs">BUILDCO</div>
        <div class="h-6 font-bold text-lg lowercase italic font-serif">marketwise</div>
        <div class="h-6 font-semibold text-base">Venture+</div>
    </div>

    <!-- Trust Text -->
    <div class="text-gray-400 text-sm font-light text-right md:text-left">
      Trusted by 1,000+ finance teams
    </div>
  </div>
</SectionWrapper>
