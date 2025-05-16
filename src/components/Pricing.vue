<template>
  <section id="pricing" class="bg-primary relative py-20 sm:py-25 lg:py-30">
    <div
      class="before:absolute before:content-[''] before:top-0 before:right-0 before:w-full before:h-full before:opacity-30 before:z-0"
    >
      <div class="container mx-auto px-4">
        <div class="text-center mb-12">
          <p class="text-sm sm:text-base text-gray-300 mb-2">
            Whats the function
          </p>
          <h2 class="text-2xl sm:text-3xl lg:text-4xl font-bold text-white">
            Let's see how it works
          </h2>
        </div>

        <div class="flex flex-wrap justify-center md:flex-nowrap">
          <div
            class="w-[438px] md:w-1/2 lg:w-2/7 xl:w-2/7 max-w-md md:max-w-none bg-[#2F5392] rounded-lg p-4 sm:p-6 md:p-8 lg:p-10 my-10 md:my-0 md:ml-6 relative mr-5"
          >
            <div class="mb-8 lg:mb-12">
              <div class="flex justify-between items-start">
                <div>
                  <h2
                    class="text-xl sm:text-2xl font-bold text-white mb-2 sm:mb-3"
                  >
                    Free Plan
                  </h2>
                  <p class="text-white opacity-70 text-sm sm:text-base">
                    For Small teams or office
                  </p>
                </div>
              </div>
            </div>

            <ul class="space-y-4 sm:space-y-5">
              <li
                v-for="(feature, index) in freeFeatures"
                :key="index"
                class="flex items-start text-white"
                :class="{ 'opacity-55': !feature.included }"
              >
                <button class="text-secondary mr-2 mt-1" aria-label="list icon">
                  <svg
                    v-if="feature.included"
                    stroke="currentColor"
                    fill="currentColor"
                    stroke-width="0"
                    viewBox="0 0 512 512"
                    height="1em"
                    width="1em"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M256 48C141.1 48 48 141.1 48 256s93.1 208 208 208 208-93.1 208-208S370.9 48 256 48zm106.5 150.5L228.8 332.8h-.1c-1.7 1.7-6.3 5.5-11.6 5.5-3.8 0-8.1-2.1-11.7-5.7l-56-56c-1.6-1.6-1.6-4.1 0-5.7l17.8-17.8c.8-.8 1.8-1.2 2.8-1.2 1 0 2 .4 2.8 1.2l44.4 44.4 122-122.9c.8-.8 1.8-1.2 2.8-1.2 1.1 0 2.1.4 2.8 1.2l17.5 18.1c1.8 1.7 1.8 4.2.2 5.8z"
                    ></path>
                  </svg>
                  <svg
                    v-else
                    stroke="currentColor"
                    fill="currentColor"
                    stroke-width="0"
                    viewBox="0 0 512 512"
                    height="1em"
                    width="1em"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M256 48C141.1 48 48 141.1 48 256s93.1 208 208 208 208-93.1 208-208S370.9 48 256 48zm52.7 283.3L256 278.6l-52.7 52.7c-6.2 6.2-16.4 6.2-22.6 0-3.1-3.1-4.7-7.2-4.7-11.3 0-4.1 1.6-8.2 4.7-11.3l52.7-52.7-52.7-52.7c-3.1-3.1-4.7-7.2-4.7-11.3 0-4.1 1.6-8.2 4.7-11.3 6.2-6.2 16.4-6.2 22.6 0l52.7 52.7 52.7-52.7c6.2-6.2 16.4-6.2 22.6 0 6.2 6.2 6.2 16.4 0 22.6L278.6 256l52.7 52.7c6.2 6.2 6.2 16.4 0 22.6-6.2 6.3-16.4 6.3-22.6 0z"
                    ></path>
                  </svg>
                </button>
                <span>{{ feature.text }}</span>
              </li>
            </ul>

            <div class="text-center mt-10 lg:mt-16">
              <button
                class="border border-white rounded-[45px] w-[150px] h-[46px] bg-white text-black font-semibold hover:shadow-2xl hover:cursor-pointer"
              >
                Signup Now
              </button>
            </div>
          </div>

          <div
            class="w-full md:w-1/2 lg:w-2/7 xl:w-2/7 max-w-md md:max-w-none bg-white rounded-lg p-4 sm:p-6 md:p-8 lg:p-10 relative"
          >
            <div
              class="absolute top-4 sm:top-5 bg-orange-500 text-white text-sm font-bold px-3 py-1 rounded-md"
            >
              Recommended
            </div>

            <div class="mb-8 lg:mb-12">
              <div class="flex justify-between items-start">
                <div>
                  <h2
                    class="text-xl sm:text-2xl font-semibold text-gray-900 mb-2 sm:mb-3 mt-2"
                  >
                    Premium
                  </h2>
                  <p class="text-gray-700 text-sm sm:text-base">
                    For startup enterprise
                  </p>
                </div>
                <div class="flex flex-col text-right">
                  <span class="text-sm sm:text-base mb-2">Starting from</span>
                  <div
                    class="text-secondary font-bold text-xl sm:text-2xl lg:text-3xl"
                  >
                    $29.99<sub class="relative bottom-1">/mo</sub>
                  </div>
                </div>
              </div>
            </div>

            <ul class="space-y-4 sm:space-y-5">
              <li
                v-for="(feature, index) in premiumFeatures"
                :key="index"
                class="flex items-start text-gray-800"
              >
                <button class="text-secondary mr-2 mt-1" aria-label="list icon">
                  <svg
                    stroke="currentColor"
                    fill="currentColor"
                    stroke-width="0"
                    viewBox="0 0 512 512"
                    height="1em"
                    width="1em"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M256 48C141.1 48 48 141.1 48 256s93.1 208 208 208 208-93.1 208-208S370.9 48 256 48zm106.5 150.5L228.8 332.8h-.1c-1.7 1.7-6.3 5.5-11.6 5.5-3.8 0-8.1-2.1-11.7-5.7l-56-56c-1.6-1.6-1.6-4.1 0-5.7l17.8-17.8c.8-.8 1.8-1.2 2.8-1.2 1 0 2 .4 2.8 1.2l44.4 44.4 122-122.9c.8-.8 1.8-1.2 2.8-1.2 1.1 0 2.1.4 2.8 1.2l17.5 18.1c1.8 1.7 1.8 4.2.2 5.8z"
                    ></path>
                  </svg>
                </button>
                <span>{{ feature.text }}</span>
              </li>
            </ul>

            <div class="text-center mt-10 lg:mt-16">
              <button
                class="bg-blue-900 text-white rounded-[45px] w-[150px] h-[46px] text-sm font-medium hover:shadow-lg hover:shadow-blue-300 sm:text-base lg:text-base hover:cursor-pointer"
              >
                Signup Now
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script >
export default {
  data() {
    return {
      freeFeatures: [
        {
          text: "Ultimate access to all course, exercises and assessments",
          included: true,
        },
        {
          text: "Free access for all kind of exercise corrections with downloads.",
          included: true,
        },
        {
          text: "Total assessment corrections with free download access system",
          included: true,
        },
        {
          text: "Unlimited download of courses on the mobile app contents",
          included: false,
        },
        {
          text: "Download and print courses and exercises in PDF",
          included: false,
        },
      ],
      premiumFeatures: [
        {
          text: "Ultimate access to all course, exercises and assessments",
          included: true,
        },
        {
          text: "Free access for all kind of exercise corrections with downloads.",
          included: true,
        },
        {
          text: "Total assessment corrections with free download access system",
          included: true,
        },
        {
          text: "Unlimited download of courses on the mobile app contents",
          included: true,
        },
        {
          text: "Download and print courses and exercises in PDF",
          included: true,
        },
      ],
    };
  },
};
</script>

<style>
.bg-primary {
  background-color: #1f3e76;
}
.bg-secondary {
  background-color: #25cb9e;
}
.text-secondary {
  color: #25cb9e;
}
</style>