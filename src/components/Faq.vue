<template>
  <section class="py-20 sm:py-25 xl:py-30">
    <div class="container mx-auto px-4">
      <div class="text-center mb-12">
        <p class="text-sm sm:text-base text-gray-500 mb-2">Get your question answer</p>
        <h2 class="text-2xl sm:text-3xl lg:text-4xl font-bold text-gray-900">Frequently asked question</h2>
      </div>

      <div class="w-full md:w-4/5 lg:w-3/4 mx-auto space-y-6">
        <div class="border-b border-gray-200 pb-4 overflow-hidden">
          <button 
            @click="toggleFAQ(0)"
            class="flex items-center w-full text-left text-base sm:text-lg font-medium text-gray-900 relative pl-10 sm:pl-14"
          >
            <span 
              class="absolute left-0 w-3 h-1 sm:w-6 sm:h-6 rounded-full bg-green-500 flex items-center justify-center"
              :class="{ 'after:opacity-0': !faqs[0].isOpen }"
            >
              <span class="absolute w-3 h-1 bg-white"></span>
              <span 
                class="absolute w-1 h-3 bg-white transition-all duration-300"
                :class="{ 'rotate-90': faqs[0].isOpen }"
              ></span>
            </span>
            How to contact with riders emergency ?
          </button>
          <div 
            class="text-sm sm:text-base text-gray-700 pl-10 sm:pl-14 overflow-hidden transition-all duration-300"
            :style="{ height: faqs[0].isOpen ? faqs[0].height : '0px', marginTop: faqs[0].isOpen ? '12px' : '0px' }"
            ref="faq0"
          >
            <div class="pb-2 sm:pb-3">
              Get your website ads tests delivered at let collect sample from the victory of the managements that supplies best design system which guidelines ever with multiple features.
            </div>
          </div>
        </div>

        <div class="border-b border-gray-200 pb-4 overflow-hidden">
          <button 
            @click="toggleFAQ(1)"
            class="flex items-center w-full text-left text-base sm:text-lg font-medium text-gray-900 relative pl-10 sm:pl-14"
          >
            <span 
              class="absolute left-0 w-3 h-1 sm:w-6 sm:h-6 rounded-full bg-green-500 flex items-center justify-center"
              :class="{ 'after:opacity-0': !faqs[1].isOpen }"
            >
              <span class="absolute w-3 h-1 bg-white"></span>
              <span 
                class="absolute w-1 h-3 bg-white transition-all duration-300"
                :class="{ 'rotate-90': faqs[1].isOpen }"
              ></span>
            </span>
            App installation failed, how to update system information?
          </button>
          <div 
            class="text-sm sm:text-base text-gray-700 pl-10 sm:pl-14 overflow-hidden transition-all duration-300"
            :style="{ height: faqs[1].isOpen ? faqs[1].height : '0px', marginTop: faqs[1].isOpen ? '12px' : '0px' }"
            ref="faq1"
          >
            <div class="pb-2 sm:pb-3">
              Rhino skin maybe thick but it can be quite sensitive to sunburns and insect bites which is why they like wallow so much – when the mud dries it acts as protection from the sunburns and insects.
            </div>
          </div>
        </div>

        <div class="border-b border-gray-200 pb-4 overflow-hidden">
          <button 
            @click="toggleFAQ(2)"
            class="flex items-center w-full text-left text-base sm:text-lg font-medium text-gray-900 relative pl-10 sm:pl-14"
          >
            <span 
              class="absolute left-0 w-3 h-1 sm:w-6 sm:h-6 rounded-full bg-green-500 flex items-center justify-center"
              :class="{ 'after:opacity-0': !faqs[2].isOpen }"
            >
              <span class="absolute w-3 h-1 bg-white"></span>
              <span 
                class="absolute w-1 h-3 bg-white transition-all duration-300"
                :class="{ 'rotate-90': faqs[2].isOpen }"
              ></span>
            </span>
            Website response taking time, how to improve?
          </button>
          <div 
            class="text-sm sm:text-base text-gray-700 pl-10 sm:pl-14 overflow-hidden transition-all duration-300"
            :style="{ height: faqs[2].isOpen ? faqs[2].height : '0px', marginTop: faqs[2].isOpen ? '12px' : '0px' }"
            ref="faq2"
          >
            <div class="pb-2 sm:pb-3">
              Get your blood tests delivered at the home collect a sample from management news. Get your blood tests delivered at the home collect a sample from management news. Get your blood tests delivered at the home collect a sample from management news. Get your blood tests delivered at the home.
            </div>
          </div>
        </div>

        <div class="border-b border-gray-200 pb-4 overflow-hidden">
          <button 
            @click="toggleFAQ(3)"
            class="flex items-center w-full text-left text-base sm:text-lg font-medium text-gray-900 relative pl-10 sm:pl-14"
          >
            <span 
              class="absolute left-0 w-3 h-1 sm:w-6 sm:h-6 rounded-full bg-green-500 flex items-center justify-center"
              :class="{ 'after:opacity-0': !faqs[3].isOpen }"
            >
              <span class="absolute w-3 h-1 bg-white"></span>
              <span 
                class="absolute w-1 h-3 bg-white transition-all duration-300"
                :class="{ 'rotate-90': faqs[3].isOpen }"
              ></span>
            </span>
            New update fixed all bug and issues
          </button>
          <div 
            class="text-sm sm:text-base text-gray-700 pl-10 sm:pl-14 overflow-hidden transition-all duration-300"
            :style="{ height: faqs[3].isOpen ? faqs[3].height : '0px', marginTop: faqs[3].isOpen ? '12px' : '0px' }"
            ref="faq3"
          >
            <div class="pb-2 sm:pb-3">
              If you're looking to hunt a unicorn, but don't know where to begin, try Lake Superior State University in Sault Ste. Marie, Michigan. Since 1971, the university has issued permits to unicorn questers.
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      faqs: [
        { 
          isOpen: true,
          height: 'auto'
        },
        { 
          isOpen: false,
          height: 'auto'
        },
        { 
          isOpen: false,
          height: 'auto'
        },
        { 
          isOpen: false,
          height: 'auto'
        }
      ]
    }
  },
  mounted() {
    this.$nextTick(() => {
      this.faqs.forEach((faq, index) => {
        if (faq.isOpen) {
          this.faqs[index].height = `${this.$refs[`faq${index}`].scrollHeight}px`;
        }
      });
    });
  },
  methods: {
    toggleFAQ(index) {
      this.faqs.forEach((faq, i) => {
        if (i !== index) {
          this.faqs[i].isOpen = false;
        }
      });
      
      this.faqs[index].isOpen = !this.faqs[index].isOpen;
      
      this.$nextTick(() => {
        if (this.faqs[index].isOpen) {
          this.faqs[index].height = `${this.$refs[`faq${index}`].scrollHeight}px`;
        } else {
          this.faqs[index].height = '0px';
        }
      });
    }
  }
}
</script>

