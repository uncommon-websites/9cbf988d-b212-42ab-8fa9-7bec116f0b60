<script lang="ts">
  import SectionWrapper from './SectionWrapper.svelte';
</script>

<div class="bg-black text-white py-24 px-4 md:px-8 max-w-[1400px] mx-auto relative">
    <div class="px-4 md:px-12 flex flex-col md:flex-row items-center justify-between gap-8">
        <div>
            <h2 class="font-serif text-3xl md:text-4xl mb-3">
                Ready to automate your invoices?
            </h2>
            <p class="text-gray-400 text-sm">Join 1,000+ finance teams saving hours every month</p>
        </div>
        
        <a href="#" class="inline-flex items-center px-6 py-3 bg-white text-black font-medium rounded hover:bg-gray-100 transition-colors">
            Start free trial <span class="ml-2">→</span>
        </a>
    </div>
</div>

<SectionWrapper withBorderBottom={false} className="py-12">
    <div class="px-4 md:px-12">
        <!-- Top Row -->
        <div class="flex flex-col md:flex-row justify-between items-start md:items-center border-b border-gray-200 border-dashed pb-12 mb-12">
            <div class="text-xs text-gray-500 mb-4 md:mb-0">
                hello@cashfeed.com
            </div>
            
            <div class="flex space-x-6 text-xs text-gray-500 font-medium">
                <a href="#" class="hover:text-gray-900">Features</a>
                <a href="#" class="hover:text-gray-900">Pricing</a>
                <a href="#" class="hover:text-gray-900">Integrations</a>
                <a href="#" class="hover:text-gray-900">Customers</a>
            </div>
        </div>

        <!-- Bottom Row -->
        <div class="flex flex-col md:flex-row justify-between items-start md:items-center text-[10px] text-gray-400">
            <div class="mb-4 md:mb-0">
                ©2025 Cashfeed BV. All rights reserved.
            </div>
            
            <div class="mb-4 md:mb-0">
                Cashfeed BV, Dok-Noord 4D 101, 9000 Gent, Belgium • BE1020118217
            </div>
            
            <div class="flex space-x-4">
                <a href="#" class="hover:text-gray-600">Privacy Policy</a>
                <span>•</span>
                <a href="#" class="hover:text-gray-600">Terms of Service</a>
            </div>
        </div>
    </div>
</SectionWrapper>

<!-- Cookie Banner -->
<div class="fixed bottom-4 right-4 bg-white border border-gray-200 shadow-lg p-4 rounded-lg max-w-sm z-50 flex items-center gap-4">
    <p class="text-xs text-gray-600">
        We use cookies to personalize content, run ads, and analyze traffic.
    </p>
    <button class="text-xs font-medium bg-gray-100 hover:bg-gray-200 px-3 py-1 rounded transition-colors">
        Okay
    </button>
</div>
