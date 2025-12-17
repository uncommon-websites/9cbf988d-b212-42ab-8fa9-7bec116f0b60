<script lang="ts">
  import SectionWrapper from './SectionWrapper.svelte';
  import SolutionBlock from './SolutionBlock.svelte';
</script>

<SectionWrapper withBorderBottom={true} className="">
  <div class="px-4 md:px-12">
    <div class="py-16 text-center">
      <h2 class="font-serif text-4xl text-gray-900">How Cashfeed works</h2>
    </div>

    <!-- Block 1 -->
    <SolutionBlock
      label="Automatic Retrieval"
      title="Never chase invoices again"
      description="Cashfeed automatically retrieves invoices from your email (IMAP), dedicated inbox, and even portals behind login walls. No more forwarding, downloading, or manual entry—every invoice flows directly into your system."
    >
      <!-- Visual for Block 1: Invoice Sources -->
      <div class="relative w-full h-full flex items-center justify-center">
        <!-- Central Hub -->
        <div class="w-20 h-20 bg-black shadow-lg rounded-lg flex items-center justify-center z-10 border border-gray-100">
           <svg class="w-10 h-10 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"></path></svg>
        </div>
        
        <!-- Connected Sources -->
        <div class="absolute top-1/4 left-1/4 bg-white p-3 shadow rounded border border-gray-100 animate-pulse">
            <svg class="w-6 h-6 text-gray-700" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path></svg>
            <div class="mt-1 text-[10px] text-center font-medium">Email</div>
        </div>
        <div class="absolute top-1/4 right-1/4 bg-white p-3 shadow rounded border border-gray-100">
            <svg class="w-6 h-6 text-gray-700" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 15a4 4 0 004 4h9a5 5 0 10-.1-9.999 5.002 5.002 0 10-9.78 2.096A4.001 4.001 0 003 15z"></path></svg>
            <div class="mt-1 text-[10px] text-center font-medium">Portal</div>
        </div>
        <div class="absolute bottom-1/4 left-1/3 bg-white p-3 shadow rounded border border-gray-100">
            <svg class="w-6 h-6 text-gray-700" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 4H6a2 2 0 00-2 2v12a2 2 0 002 2h12a2 2 0 002-2V6a2 2 0 00-2-2h-2m-4-1v8m0 0l3-3m-3 3L9 8m-5 5h2.586a1 1 0 01.707.293l2.414 2.414a1 1 0 00.707.293h3.172a1 1 0 00.707-.293l2.414-2.414a1 1 0 01.707-.293H20"></path></svg>
            <div class="mt-1 text-[10px] text-center font-medium">Inbox</div>
        </div>
         <div class="absolute bottom-1/4 right-1/3 bg-white p-3 shadow rounded border border-gray-100">
            <svg class="w-6 h-6 text-gray-700" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 10v6m0 0l-3-3m3 3l3-3m2 8H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"></path></svg>
            <div class="mt-1 text-[10px] text-center font-medium">Upload</div>
        </div>
        
        <!-- Connecting Lines -->
        <svg class="absolute inset-0 w-full h-full pointer-events-none opacity-20" viewBox="0 0 400 300">
            <path d="M100 100 L200 150 M300 100 L200 150 M150 220 L200 150 M250 220 L200 150" stroke="currentColor" stroke-width="1" stroke-dasharray="4 4" />
        </svg>
      </div>
    </SolutionBlock>

    <!-- Block 2 -->
    <SolutionBlock
      label="AI-Powered Matching"
      title="Approve in one click"
      description="Our AI automatically matches invoices to the right ledger accounts and cost centers, then routes them to the correct approver. Your team gets Slack or email notifications and can approve with a single click—no more hunting through spreadsheets."
      reversed={true}
    >
      <!-- Visual for Block 2: Approval Card -->
      <div class="bg-white rounded-lg shadow-xl p-6 w-3/4 max-w-sm border border-gray-100">
        <div class="flex items-center justify-between mb-4">
            <div class="flex items-center space-x-2">
                <div class="w-8 h-8 rounded bg-gray-900 flex items-center justify-center text-white text-xs font-bold">CF</div>
                <div>
                    <div class="text-xs font-semibold">Supplier Invoice</div>
                    <div class="text-[10px] text-gray-500">€2,450.00</div>
                </div>
            </div>
            <div class="px-2 py-1 bg-green-100 text-green-700 text-[10px] font-medium rounded">Matched</div>
        </div>
        <div class="space-y-2 mb-4 text-xs">
            <div class="flex justify-between">
                <span class="text-gray-500">Ledger:</span>
                <span class="font-medium">Office Supplies</span>
            </div>
            <div class="flex justify-between">
                <span class="text-gray-500">Cost Center:</span>
                <span class="font-medium">Operations</span>
            </div>
            <div class="flex justify-between">
                <span class="text-gray-500">Approver:</span>
                <span class="font-medium">Sarah M.</span>
            </div>
        </div>
        <button class="w-full bg-black text-white py-2.5 rounded text-sm font-medium flex items-center justify-center space-x-2 hover:bg-gray-800 transition-colors">
            <span>Approve & Pay</span>
            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
        </button>
      </div>
    </SolutionBlock>

    <!-- Block 3 -->
    <SolutionBlock
      label="Seamless Integration"
      title="Sync with your accounting software"
      description="Real-time integration with Xero, QuickBooks, and Exact Online means your ledger accounts and cost centers are always up to date. Plus, get PEPPOL compliance set up in under 2 minutes for Belgian e-invoicing requirements."
    >
       <!-- Visual for Block 3: Integration Dashboard -->
       <div class="bg-white rounded shadow-lg p-6 w-2/3 max-w-xs border border-gray-100 relative">
          <div class="flex justify-between items-center mb-4 pb-3 border-b">
              <div class="font-bold text-sm">Integrations</div>
              <div class="w-2 h-2 bg-green-500 rounded-full animate-pulse"></div>
          </div>
          <div class="space-y-3">
              <div class="flex items-center justify-between p-2 bg-gray-50 rounded">
                  <div class="flex items-center space-x-2">
                      <div class="w-6 h-6 bg-blue-600 rounded flex items-center justify-center text-white text-[8px] font-bold">X</div>
                      <span class="text-xs font-medium">Xero</span>
                  </div>
                  <span class="text-[10px] text-green-600 font-medium">Connected</span>
              </div>
              <div class="flex items-center justify-between p-2 bg-gray-50 rounded">
                  <div class="flex items-center space-x-2">
                      <div class="w-6 h-6 bg-green-500 rounded flex items-center justify-center text-white text-[8px] font-bold">Q</div>
                      <span class="text-xs font-medium">QuickBooks</span>
                  </div>
                  <span class="text-[10px] text-green-600 font-medium">Connected</span>
              </div>
              <div class="flex items-center justify-between p-2 bg-gray-50 rounded">
                  <div class="flex items-center space-x-2">
                      <div class="w-6 h-6 bg-purple-600 rounded flex items-center justify-center text-white text-[8px] font-bold">S</div>
                      <span class="text-xs font-medium">Slack</span>
                  </div>
                  <span class="text-[10px] text-green-600 font-medium">Connected</span>
              </div>
          </div>
          <div class="mt-4 pt-3 border-t text-center">
              <span class="text-[10px] text-gray-500">Last sync: 2 minutes ago</span>
          </div>
       </div>
    </SolutionBlock>
  </div>
</SectionWrapper>
