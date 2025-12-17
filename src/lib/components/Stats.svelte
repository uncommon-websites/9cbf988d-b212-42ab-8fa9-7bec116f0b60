<script lang="ts">
  import SectionWrapper from './SectionWrapper.svelte';
</script>

<SectionWrapper withBorderBottom={true} className="py-24">
  <div class="px-4 md:px-12 grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-12">
    <!-- Stat 1 -->
    <div class="text-center md:text-left">
      <div class="font-serif text-5xl md:text-6xl text-gray-900 mb-4">
        3.5M+
      </div>
      <p class="text-gray-500 text-sm max-w-xs mx-auto md:mx-0">
        Invoices processed and counting
      </p>
    </div>

    <!-- Stat 2 -->
    <div class="text-center md:text-left">
      <div class="font-serif text-5xl md:text-6xl text-gray-900 mb-4">
        1,000+
      </div>
      <p class="text-gray-500 text-sm max-w-xs mx-auto md:mx-0">
        Finance teams trust Cashfeed daily
      </p>
    </div>

    <!-- Stat 3 -->
    <div class="text-center md:text-left">
      <div class="font-serif text-5xl md:text-6xl text-gray-900 mb-4">
        75%
      </div>
      <p class="text-gray-500 text-sm max-w-xs mx-auto md:mx-0">
        Fewer manual mistakes reported
      </p>
    </div>

    <!-- Stat 4 -->
    <div class="text-center md:text-left">
      <div class="font-serif text-5xl md:text-6xl text-gray-900 mb-4">
        92%
      </div>
      <p class="text-gray-500 text-sm max-w-xs mx-auto md:mx-0">
        Faster approvals on average
      </p>
    </div>
  </div>
</SectionWrapper>
