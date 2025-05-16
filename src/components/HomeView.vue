<template>
  <div>
    <div class="relative w-full h-[900-px]">
      <div
        id="navbar"
        class="w-full fixed top-0 left-0 z-10 px-4 py-3 transition-colors duration-100 bg-transparent text-white font-semibold"
      >
        <div
          class="max-w-screen-xl mx-auto flex justify-between items-center relative"
        >
          <!-- Logo -->
          <div class="flex items-center space-x-3">
            <img src="../assets/images/logo.png" alt="Logo" class="w-8 h-8" />
            <p id="logotext" class="text-xl font-bold">Startup Landing</p>
          </div>

          <!-- Desktop Nav -->
          <nav id="rout" class="hidden lg:flex space-x-8">
            <router-link to="#home">Home</router-link>
            <router-link to="#features">Features</router-link>
            <router-link to="#testimonial">Testimonial</router-link>
            <router-link to="#pricing">Pricing</router-link>
          </nav>

          <!-- Button -->
          <button
            id="butn"
            class=" border border-white rounded-full w-[150px] h-[46px] hover:bg-white hover:text-black"
          >
            Get Started
          </button>

          <!-- Mobile Menu Toggle -->
          <button @click="toggleMenu" class="lg:hidden focus:outline-none">
            <svg
              class="w-6 h-6"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 6h16M4 12h16M4 18h16"
              ></path>
            </svg>
          </button>

          <!-- Mobile Menu -->
          <div
            v-if="menuOpen"
            class="absolute top-[70px] left-0 w-full bg-white bg-opacity-90 text-black flex flex-col space-y-4 px-4 py-6 lg:hidden"
          >
            <router-link to="#home" @click="closeMenu">Home</router-link>
            <router-link to="#features" @click="closeMenu"
              >Features</router-link
            >
            <router-link to="#testimonial" @click="closeMenu"
              >Testimonial</router-link
            >
            <router-link to="#pricing" @click="closeMenu">Pricing</router-link>
           
          </div>
        </div>
      </div>
      <div
        id="home"
        class="h-[900px] bg-[#1F3E76] bg-opacity-50 rounded-br-[250px] flex"
      >
        <div class="absolute left-50 top-35 text-white w-[480px] h-[172px]">
          <p class="text-[66px] font-semibold">
            Experience your ultimate mobile application
          </p>
          <p class="text-lg mt-10">
            Get your blood tests delivered at let home collect sample from the
            victory of the managements that supplies best design system
            guidelines ever.
          </p>
          <div class="mt-10 flex">
            <button
              class="bg-white text-black font-semibold rounded-[45px] w-[150px] h-[46px] mr-5"
            >
              Get Started
            </button>
            <button
              class="flex items-center font-semibold hover:cursor-pointer"
              @click="isOpen = !isOpen"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="size-8 mr-2"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M21 12a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z"
                />
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M15.91 11.672a.375.375 0 0 1 0 .656l-5.603 3.113a.375.375 0 0 1-.557-.328V8.887c0-.286.307-.466.557-.327l5.603 3.112Z"
                />
              </svg>
              Watch Video
            </button>
            <div v-if="isOpen" class="fixed left-0 top-0 z-20">
              <button
                class="bg-black opacity-40 fixed left-0 top-0 w-screen h-[900px] hover:cursor-pointer"
                @click="isOpen = !isOpen"
              ></button>

              <video id="video" controls>
                <source
                  src="https://youtu.be/ZNA9rmDsYVE"
                  type="video/mp4"
                  class="absolute left-40 top-40"
                />
              </video>
            </div>
          </div>
        </div>
        <!-- <div>
          <div
            class="w-[390px] h-[450px] rounded-br-[500px] rounded-tr-[400px] bg-white opacity-5"
          ></div>
          <div class="w-[390px] h-[450px] flex">
            <div
              class="w-[170px] h-[450px] bg-white opacity-5 rounded-tl-[150px]"
            ></div>
            <div
              class="w-[220px] h-[450px] bg-white opacity-5 rounded-r-[500px]"
            ></div>
          </div>
        </div>
        <div
          class="w-[500px] h-[800px] bg-white opacity-5 rounded-br-[300px]"
        ></div>
        <div
          class="absolute top-50 right-33 w-[500px] h-[700px] bg-white opacity-5 rounded-tl-[300px]"
        ></div>
        <div
          class="absolute top-0 right-0 w-[132px] h-[200px] bg-white opacity-5"
        ></div> -->
        <!-- <div class="absolute top-55 right-0 w-[132px] h-[450px]">
          <img :src="img1" alt="" />
        </div> -->
        <img
          src="https://startup-app-modern.vercel.app/_next/static/images/banner-thumb-10b963235571f7743a4fdb04280058ad.png"
          class="absolute top-35 left-155 w-[900px] h-auto hidden md:block"
        />

        <div class="absolute left-50 bottom-45 flex">
          <p class="text-white mr-5 opacity-60 text-[20px]">Sponsored by:</p>
          <div class="flex justify-between w-[370px] h-[28px]">
            <img
              src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTAwIiBoZWlnaHQ9IjI4IiBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHhtbG5zOnhsaW5rPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5L3hsaW5rIj48cGF0aCBmaWxsPSJ1cmwoI3BhdHRlcm4wKSIgZD0iTTAgMGgxMDB2MjhIMHoiLz48ZGVmcz48cGF0dGVybiBpZD0icGF0dGVybjAiIHBhdHRlcm5Db250ZW50VW5pdHM9Im9iamVjdEJvdW5kaW5nQm94IiB3aWR0aD0iMSIgaGVpZ2h0PSIxIj48dXNlIHhsaW5rOmhyZWY9IiNpbWFnZTAiIHRyYW5zZm9ybT0ic2NhbGUoLjAwNjY3IC4wMjM4KSIvPjwvcGF0dGVybj48aW1hZ2UgaWQ9ImltYWdlMCIgd2lkdGg9IjE1MCIgaGVpZ2h0PSI0MiIgeGxpbms6aHJlZj0iZGF0YTppbWFnZS9wbmc7YmFzZTY0LGlWQk9SdzBLR2dvQUFBQU5TVWhFVWdBQUFKWUFBQUFxQ0FZQUFBQlJDYUxzQUFBSVFFbEVRVlI0bk8xY3oyOGJSUlIrYSsvYWFac21jZEpFclVzTkRnY2tEcURJVWdNNUlOVnlwZVNBeENVSUNVNUlwRGM0b2VZdmdPVEdDYW5tektVQkRsd2NxZGI2WnVTb2tRK0FPRkJjVVVFbG9LMmhSUzB0aVlNbWZSdkdremM3cyt0Wng3SHpTU3RaM3ZIc3ZKbHYzNjk1WSt1OTVVOUFSRGFUemdEQTJ3Q1EySGRURHpzQXNBVUEvd0RBWFFENEFRQ3UzN3gxdStYMzYrTEhINFI4M0JGNkRiWmtQRzhBUUxLRHNWcElTbmFOTUs0Q3dIdzJrLzRSQUw2NmVldjI0eU1tOURkaUV1bEdJcENhUGVzRkFQZ3dtMG1mSGRRSkh4VHNJMVkyazQ3NWFESVRZSDIvbTgya1U0TSsrZjBNU21PZDY0SzhjUUI0WjNDbWVmQkFFZXU1THMzQ3hKRko3RjlReERyVFJXbGY3ZmNKSGxSUXhKcm80bHhNRHZiMDl5OG9ZcDNzb3JST3YwL3dvSUtLL3BUNXE1MmRIZGplOXMxMWtyQXNDNitubndIZ2ljbDVYNjlzN0FSb3Zvblgya0ordG14eUhQMEV0dForV0s5c0ZBRGdtdEJrdVkxWTJVeDZESk9idm5qeVpBdGFpZ2VxRUkvRklKbDBIaDNnR3VUd1dpcTV0VFVBdUxTUW4yMGU0SGo2Q3FJcHpPb0kxeW1wR0xaYkxSZ2RQajZlbjV1Wno4L05LTWtjTVJiWlcxZHlhMGU1TlVNUWlhWE1ZYWxVWXhDY0hENTJBZ0JlQVlEQ2djN0NVekR0ZGJVSHh0RVhFSW1sak5KTThTb2VpMjNiOGJobml1Znljek9SUklnTCtWbUx2d0JnbkprOUFHZ1F6UXNsdDlZTEpELzBFSjMzTVpWQXJWWndwNTNDaWVOREQ3a0lsQzM0eXdBUXVST05mbFFSL2FyckFEQXRORmxTamFQazFwaDJZMmF6dVpDZjNZeDJ4TjBITHg4R09JRWhFdXVZcW9OV3k0ekttcG9ZRlV0eU10MmNRVWF3a2x0YkJZQXJ3cTE5R2d0OXJ5WDB4WExDUGZDaVMwWllQZ0FvdWJYTFJIL2xoZnpzcW14Y0piY21SbGlBR3JhQXorZXh6SWhkY212czViaU05ejAvc1lrdlNGRVY5ZnJKdDE3WmFKTnYvc0o1clFCbnp4Um1NMmxiWi9QWmhJODFsSFFlSlJ4YlRHdDBNMy9tWVkzNHJzMkJ4N2YzSndCWUVTZWRRdzd2WDhmMkhwcElDUDVha2cwR2Z5dTJuMTdJenpad1hPSzlWTW10TGFMbVhSTEdudUtDa3N1S1oyckx0MTdaa0xWcEErOWphV21NVG9uRmJGNG1QVWtsWnJzZUdhclNDempwMTBTeStXQWFGOUl6cnhSeHA3bjdJaWovanVwanJ5L1V1S3J4clpUYzJqNUNoNVZ2dmJJaEcvOGUrQVZXYmo0elVuV3FyNlpPamQyMzQzRXFDZnV3dzY0RFE5QXVGRmFJU1dmYVl4bXZJbW9sSHF6OXJvWkE0bExFa0FVSVFZbkZqNitoOEExWGlIUktSL0w1Z1RkOXAxV05PN1dDcWRIaEJ4TmpKMlZGaEg5MjFuc29pRDRMZUl1RFdrVmNhSmFsZjVQL291VFdpbWlLZUN5aVh3UklEUEU1QlZ3MEVlTHpOaFhCZ2VkZ3MrVHVIZ0hSOUswUWJabldXalVzSHdsZVl5azNuOE9hUVdiakpzZEg3cCtaVFBuNVViK0g2andrMERSUWI1NzMxcWZ3TTMvdGM3cHg0VVZOa2VMdXJ4RnZQUlVnVUNUMzAxWWUya2lGejF5VkVKZC9ocFo4OHhmTys4b25BNit4aGxXTnd4QXJtWEFlUDNONllpZVpjRlRsemo4SDdsd0RoT1BxT2NHVUdXeDZDNEtFdVdob0dHdUMwODZjN3B5Z2phanhxSWkxS1pLS3d5b1JLT3c5dzdCOCs4QVRTM2tpUnpmVndKS2ZMRTgxT1Q3aUpCUE9rTVpQSGtWRkxNSWsrRUc2WDRqK1dFNTRXejNOby9MVnlzUWlGNFFjRVdVR3FTU3UyQzhKOXR1U1c5c2swaU1GS3YwZ2t3L1REVnFSSUk5ZFltVXo2UW1kcUN3V3M3YkhSazcrSFkvSDJoZ1dqOFdzZUR4bU9ZNXREeVdjWTVabHhRT21EK3B1dGQ1NjYvWFhnbzdmRkpxWUU5cjM5bk1tVXhrSnljRDZMYm0xSmtGSzN0OFJGMC9IREtweVNzcWNrd241S0hnYVM5a3BLM041OXV6VVZzS3hSMDBPQU04ZmZtTzR6eUJncG0rVjBnNllyRFMxeFNPYVE3WjlsRUlOR1RRYU5BTEQ4clhCSTFaYTFURGgyQzBpcVdrQ0ZiZGFmeENGY0lobHlmZWJhRzVrcG8vS21qZTVFTHpCYVFTLzVLS0hvc1FjcmhHLzFUR0RPcEE2MlJISTF3YVBXRk9xaGduSC9yZkRRNndVMkFucHF1RSsyK0MzZmFLQTZQU3pTYjVJaGY5bzVsVGpZRnN2RGNFNjVDVHBDRjF0dFVoRmN2RC9OZzFGQm0vOFd2S3hnRzI5c2hHNFRzMUxOeWpOR3hMTEpMNERnQy9jYXQxY0hZNVppRys3WDA1SjF6OFJDYlBJYmZqNnRaTWg1NVBrcGJhT0dweUdqa0srUFhqRVVtNCtKeFBPZHRET0pXQVo5cThCNEV1M1dqZlZaemN3VFJVQ29ra0pTNnhwUWxzRk5ZTlhSSEtoUTA1RnczNlplVksrOWNwR0tNZmV6bWJTRGg0ZzlZWGoyTExqK0RwZ3RlMi9BTUQzQVBDdFc2MGJyWFdQQ0tMWllwK3ZZaWE2eVdXeXRaMWZpVGtVVFZKUXB6MkhtOTlsSEJjVllYcmd6YVp4K1hqWXV1WElNY3M2cnRIc0RnQ3dPaEptTmgvajlSY0EzT3Roa3lkRGtYanJDejRSSEpVNXAwRDFLL2FsaXpJM0hoVUJ4TWczS3ZsMllldFVOVGkydmFPajFSamozV3E5cTFzelVZRTUvWmhma3BhNUlDNXhKU282V1BNaFZsQXpXTWIreEpveUVhd21xeTA2amxDK1hjUjBUajRuSEZ2SEYvcW5YMGpsWVNFL2V3blRGZFJpbHpHS292YmsvUHBzK0ZSbEJzNWQ0Zk12U3Zwc1lPS1gzRERXa1cvK3d2bEE4bm13UHZyMDZ2dFlCeTVGYW1UNDRkaklDWlVwL05XdDFqOExNd2dQVWZ6eEdwNWY3QmhDOUNiTmYrbkFKekg1dkV4alNTb1dsdmwwQ21vZ3oyOEtWRFl0a3k5czRZR3RzL21jU05oYkduMzlFV29FaHdTbWF0dDk4a3ZsVHBPaStQdFFmWml1M2JkMWpya25IRnVIdG5mTkRLbi93SjM4OFlya3FJeDQyRVJ1VDBMckQ5WWtGWjhpN3ZUVHhCZ0dkVUNDUjk4ZDgyZkUraHdBWHBRMmVIcjI3eVdOdm82SUZRNmJxbXJNd3dqNzVxM2JOd0RnaG16cytibVpjeHJFWW9jTjcvWGI1SFFCUlhUQWRRS0JKcEU1NzluL210QXhoVHIvbDlVOFpOc3ozWVpZWWRGQVoxMmJHSmhXQ0JYNkh3UjBpSFZLbzgxdnZTcWd5ZithNkFDa1k5NGpZNHNFT3Z0L2Q5RFV5ZkRnZ0F2MWp0QnJBSUQvQUZNRHl0UmEyMDFkQUFBQUFFbEZUa1N1UW1DQyIvPjwvZGVmcz48L3N2Zz4="
              alt=""
            />
            <img
              src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iODUiIGhlaWdodD0iMjgiIGZpbGw9Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgeG1sbnM6eGxpbms9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkveGxpbmsiPjxwYXRoIGZpbGw9InVybCgjcGF0dGVybjApIiBkPSJNMCAwaDg1djI4SDB6Ii8+PGRlZnM+PHBhdHRlcm4gaWQ9InBhdHRlcm4wIiBwYXR0ZXJuQ29udGVudFVuaXRzPSJvYmplY3RCb3VuZGluZ0JveCIgd2lkdGg9IjEiIGhlaWdodD0iMSI+PHVzZSB4bGluazpocmVmPSIjaW1hZ2UwIiB0cmFuc2Zvcm09Im1hdHJpeCguMDA3ODQgMCAwIC4wMjM4IC0uMDAyIDApIi8+PC9wYXR0ZXJuPjxpbWFnZSBpZD0iaW1hZ2UwIiB3aWR0aD0iMTI4IiBoZWlnaHQ9IjQyIiB4bGluazpocmVmPSJkYXRhOmltYWdlL3BuZztiYXNlNjQsaVZCT1J3MEtHZ29BQUFBTlNVaEVVZ0FBQUlBQUFBQXFDQVlBQUFCN3VWTkRBQUFKaEVsRVFWUjRuTzFjQjR4V1JSRCs3Z0N4S3daRTVEejFUcXlJb2dJMmlpakZnaWlpTVhZVTdJZ0ZOWlpZTUZZRURVcEVVYkdCYUxBVEVWSHNIU3VLbklpSGlJcllVT0E0am9Nemc5OUxOcE41NzkvOS93ZWMrTDdrd3QyKzNYMWJabWRudnBsSDBhU3BIeUFBNVFBT0JYQUFnRjBBdEFEUUdNQktBTDhEK0E3QUp3Q21BSGdEd0lxUXpqT3NlZmdJUURHQTNnQUdBOWcvWUlRL0FiZ2J3RDBBRm1aN0c0U2RBRHloR2x3RDRQbTBYMVNjNDNrN0FCOENlRHB3OHdWYkE3Z0pRQVdBNHdzWTQvOFJHd0RZUS8xc3NUcldJVTRBaWdCY0R1QmRBSHNYK0k0dEFUd080QUVBNnhYWVY0YVUwZERvcmdHQTBRRDZKYnhxS1RWREJYK1hOcVVVbHBZeGJVNEg4QmVBaTdOTnJEL1FBbENVWS9QRnNMc1R3Q1FBeTJMcWlMbzZoeHZleUNrWGdibCtYVnE4ZFFINkNoZ2NzL20vQXVnRG9BdUFaeE0yWC9BNWdMTUI3QWJnSFpiSjVuZW5Cc2hRaitBS3dGNEFiamFHOWhWVit6T0J3NTVGZ2JrcTIvejZpK2dLRU5VL2luZTVpMG9BWFFFc3lITUd0ZlFFTXRSVFJCcWdOMTArdlhsOUM5ajhEUDhCUkFKd3ZqSFVFV1QxTXF6RGFFakNwcXVhb2hoNXQ5YWphUmZSeld4SnowSzAwbXdBTlNuMTM0SjhSUzBaekQ5VDZuZFRBTnZ5YXYyUnh2VHFobkF0MndIWUVNQWZBT2FScWpjaEF0Q05DK3hpWWoxUi9YSXRuUWZnY0FCTjFiTmxkRXZIQUpqQXpRdEJEM284WXFBMlVlMitCL0FDN2FLdkF2dmRHTUNaQUU0R3NLZDY5aVdBaDBpUnl6dDdxdWN5ajhXQjd3T1p3NU1BbkFwZ1gyWEwvUTFnTW9EYkFFelREU1VXTUJMQXVhcDhBSUQ3OHhoSVdoRGFjMlFBaFN3TGV4cUFqejNxN2toVzhrQ1B1blVVc0lzOXZaaWpLRFROYzlTYnhRMFpyY3EzQnpDSGd2T3BldGFQd3FQUmhXUGN6bU44c3FjREFWUkhCYUlCV2hrVmZSWXlRaWxkeUh4UVNkN0F4UTRBWHVaaStLSTFnUGQ0Q3A1TWFOT05jWTJOUGZzdElxSFZrWnBpVGtMZEt3SGM2Tmx2S3diSkNzVXAzUHhjTVowSS9SbkZsYmxVZ1FMUXpLZzRMMkJnWFRtSWZDQ2swdEZPdTZZTUpjZEpzNmo1NVZSNUdtSWJQTVo3N3hYanVhakc1MkxhNWtJcjl0bWUvV3VjbDJQemF3M1cxYUxoUTlBOVlmTnJHWjV2YXJqMkVzb2ZSMjIxcXJHdUFDN3ltc0JXNmgyampNMnZvK3ByUndOblEycWRLM2kvdVlpRVFOL3AwbWE4c2ZsVjVDbDJZOXNOcUZJbkdITXY1L2cwUlB2Y1laVFBvZmJZa24wMzVkOXpVMWpYVFFBOGJHeitQTDZqQ2RkVzVuTU1yeHdYdldrdnJPcGdxZkdDelZJWXBBL2NEZG1QZzNXeG5GeEVQeG93ZFh6MkE0QmJBTFJsRW9xTDVveGt1cmlJMXJnTFdheDJaQ3BuOE5SVTA3QThGc0NKUmtMTHNVWlkvSFlWOHdDMVJSdWUwTWp5LzUxL3QyR1V0UkFNTkE3UHAxeVBNWTRodVp4WG50Zzd2Nmo2d3ZxdVYwejNSS084d0FIbWc0RkdtOHM1Z1RqSTV2Y3lOTllBSi9UY2dDcmF4UXFxd0JrSmZZdWF2Tm9vdjhENWZWZDZFeTdtVUpBWHhmVDdGNTliVjRrdnpsRDFsZ0E0RXNCdlJ2dDk2TkxyUXkydTczSEZ0S0ExRGdnWXpEaXFISitmSDFUYlNDb2IwTlZ6SWE3WVhSN3ZuMkZZeDFzNEo3VWRKK3RpcktlaE85eXdoNDV3N3U4K1Jwc2h4dFdrTWQ5emJoWWtXNmhNbGQrbnhyayt2YUtQK0hNYXl6UTZGbFBsYWZRTkdGQU5VNzV5L2NpcDIwYTFyZVMvWlNSTlhEd2I0TnVQTjhxaVJKWjlqR2ZqUFB1VnVUMmx5amJpSmdnNnFHZkxZK3dIQzdwZlg3UXg2azNpdjZLNWgxS3JqNG1aZXpYdEJ6Rm96eEpKZnB2cXlFMDVha05qNlBVOEIybWh1MUVXK2JwV0VrbVNldmFwVzVMUTkvU0F2aTBpYUd1V2w2ank3eEpVdjBiSS9GeFk4MmxOcnFLSFFlcEZtRTNYYzR4Ny9SU1RVUnRyTkxnMXdMLzB3Y2xHbmFuT09EU1dCUFJ0R2JMUlFqUTJubFViWlhHd05qUlNwOXFyQ0JuemlwaHg1NFBoWkJYMTVxOWtJbWxQRW1ERHRPMFJMZnp0aGlIVm5xNVdHdWhBMThQRlo0NTdZckZzcFFIdnRlcEdmVnFHa2JZSmtxQ3ZMZENpaHhFemlFdUhzOUFrVDA3Q1I4Z1cwTDNkbnVzK09TNGVFQW5BWEViL05JYlFIU29Fell3VVp5aWYraHRqZ05xNlRvSjF2VVFxZHFieHJGdEEzd2NiWlJYcUhSR2FrMVB3UWFlQU1iajRPdUhaV3dCT29OQmU1Y001dUtyM1dnRGZHczhmQVhCaHd0MlNoRExhRWRvSHIxVHM0U0ttamJub2JPUW9XQkFWUDBpVml6Qzl4dC9mTklUcmZNOE01ZDBONGZyYzBRQlRqRGFYZXZRTEkvN2lpMmxHd0dnbGZmMU96TUNPaTVKdXFyV2xLd0JMNk5ab0ZWTk1wdXZsQU9sdXlBbCtSbC9aUlIzOVdEM0lCNDEreGhwUlFCY2lsUGNhYW5xU0U4MlVLK0JGOWJ5Y3lhMUpRcjBadlFWZDV4SG45K2NkWVlod3FvY1gxVDlHYS9tZzJ0Q294Ukd6bHdCeHRSK2wyejhnbXBjMnZxYnp6ckNTUGc5aDR5bnNZRmZGZ0RXanVyeUZKM3drS1V1TndjN3BkUEd3d2VxMVlwQ25vMUcvaENTUm5yZ0kySFdxYklqRElrYVF6T1d4cEdvMTlxSTZiYTNLNTlQbmpsQkYrMG5qY2M1VE00UnlNQzZqMEJhQ29USGsxNmlZUUpkbzRKZElGbTNDT1loZFVCcjNhVmhIU3ZmbUhvT3NJdGZ1Z3l0akVrOGpkS1puWUhrRlh3QjRueFBma1c2cVhtQndReXcxUEN6bW00U2xYSXlaN0s4RGlUQkxPL1Jpcm9TTFJzeCt0cTZybjNsZ2ZxSjkwRE9IQVJvU0RoYVc4Z2FqajRYVWdMTTR0clk4bUhxdDVObzRMT25id0ZLcXdCQldNQTVWbEZBZkFxWS9UMGcrTHFob2hPTmlQa3B0eU9lOThwdkNxcE03Tk9aWkNXMmRRaW4wRUFFb1l1RHJoRHpmSlJwd1ZOSWl6NlVtT04yZ2NFTXdrYXJVbDMyN24xeDU2QWVsd3hNMkgyUVYrekFiSndSVlhQeTR6UWRwMk03VVVMN1FtaVFVZGN3SEdCYlliakVUYlZaNVlibE9XWlFSc3dQZHdjazVQZ3FKc0lDbnVDMVBYS1ZIR3hkQ0ErL016VXJ5ZSt0NHQwbXMveEtQejlGckdYVHFRdThnVjkxSEtieFdKbzdHanp3d2c2ajY0ekNmcHpacDR4YVRvbmQvNWh2MVZ0RFdPRERHcm5KUlF6dHJGOWVJRFAzL0FVQVdyRDM1OEpZMEtxcTRVYk5wU0ZZWVJsZStFTzc5SU9lN3d5Z3BWS2pZVjJPaW1iNG9welhlbXQ1R0xSZDZHb1U5MzRoZEl5YktkS0lCMW9qamZJc2V5VEllRFAyNTkxWkcyRFlFWmVSUG92blVVQmlqLzdOQmV5eDVDVUNHZERDSXJtaUVHaDZ1dEE2T0Y5TGsrdi92NkV6VnVvZm5PbWcyY3ZxYTNueWtrSmVXNFYvQzYxeUhKQ3VoalpHVVZpZFcvbUdxTE5jZHZscVFhWURDY2FSaVNQZW54eE9YZVZ6R1hBRE5NenkyTmdhZmFZRENjUW1OVkRlMjBKZUc4Z2ptV3l3aVhkMlRmTWhHNnEwVGpmVDROWUxNQ0V3SEF4UkZISUtGdEJ2U3lCWU9SbllGcElQUnRPcGp2OEdMd1VKcWhiV3krY2dFSUZXTW9QRlg0ZG5wVk9ic3JWVVZuTmtBNlVLSUhvbVNTa1JWYUdjeENDVi9VUHg3SVdHRUVSVldUNHhBaVhLdVhRRDRCNHU0SERneVltb3BBQUFBQUVsRlRrU3VRbUNDIi8+PC9kZWZzPjwvc3ZnPg=="
              alt=""
            />
            <img
              src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTIzIiBoZWlnaHQ9IjI0IiBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPjxwYXRoIGQ9Ik0xNC4yNjggNC41MUw3LjEzNCA5LjAybDcuMTM0IDQuNTEtNy4xMzQgNC41MUwwIDEzLjUwNWw3LjEzNC00LjUxTDAgNC41MSA3LjEzNCAwbDcuMTM0IDQuNTF6bS03LjE3IDE0Ljk4bDcuMTMzLTQuNTEgNy4xMzQgNC41MUwxNC4yMzEgMjRsLTcuMTM0LTQuNTF6bTcuMTctNS45ODVsNy4xMzQtNC41MS03LjEzNC00LjQ4NUwyMS4zNjUgMCAyOC41IDQuNTFsLTcuMTM0IDQuNTEgNy4xMzQgNC41MS03LjEzNCA0LjUxLTcuMDk3LTQuNTM1ek0zNC4wOTYgNC41MWg1Ljc2OGMzLjY3OCAwIDYuNzE2IDIuMTA5IDYuNzE2IDYuOTIzdjEuMDEyYzAgNC44NTEtMi44NDEgNy4wMzMtNi42MDUgNy4wMzNoLTUuODhWNC41MXptMy4yMjIgMi43MTh2OS41MmgyLjQ3M2MyLjA5IDAgMy40OTMtMS4zNTMgMy40OTMtNC4zNjR2LS43OTJjMC0zLjAxMS0xLjQ3Ni00LjM2NC0zLjYwNC00LjM2NGgtMi4zNjJ6bTEwLjk3Mi4xNDZoMi41ODNsLjQxOCAyLjgxNmMuNDkyLTEuOTE0IDEuNzQ3LTIuOTM4IDQuMDIyLTIuOTM4aC44djMuMjNoLTEuMzI5Yy0yLjYyIDAtMy4yNi45MDItMy4yNiAzLjQ2MnY1LjU3SDQ4LjM0VjcuMzc1aC0uMDV6bTguNDYyIDYuMzE0di0uMzQxYzAtNC4wNTkgMi42Mi02LjI3NyA2LjE4Ny02LjI3NyAzLjY0IDAgNi4xODcgMi4yMTggNi4xODcgNi4yNzd2LjM0MWMwIDMuOTg2LTIuNDcyIDYuMTMxLTYuMTg3IDYuMTMxLTMuOTQ4LS4wMzYtNi4xODctMi4xMzMtNi4xODctNi4xM3ptOS4xMTQtLjAzNnYtLjMwNWMwLTIuMjU1LTEuMTQ0LTMuNjA4LTIuOTY0LTMuNjA4LTEuNzgzIDAtMi45NjQgMS4yNDMtMi45NjQgMy42MDh2LjMwNWMwIDIuMTgyIDEuMTQ0IDMuNDI1IDIuOTY0IDMuNDI1IDEuODItLjAzNyAyLjk2NC0xLjI0NCAyLjk2NC0zLjQyNXpNNzAuOCA3LjM3NGgyLjY1NmwuMzA4IDIuMjkyYy42NC0xLjUzNiAyLjAwNS0yLjU5NiA0LjAyMi0yLjU5NiAzLjExMiAwIDUuMTY2IDIuMjE4IDUuMTY2IDYuMzI2di4zNDFjMCAzLjk4Ni0yLjI3NSA2LjA5NC01LjE2NiA2LjA5NC0xLjkzMSAwLTMuMjYtLjg2NS0zLjkxMS0yLjI1NXY2LjEzMWgtMy4xMTJMNzAuOCA3LjM3NHptOC45MTcgNi4yNzh2LS4yNjhjMC0yLjQxNC0xLjI1NC0zLjYwOC0yLjkyNy0zLjYwOC0xLjc4NCAwLTIuOTY1IDEuMzUzLTIuOTY1IDMuNjA3di4yMzJjMCAyLjE0NSAxLjE0NCAzLjQ5OCAyLjkyOCAzLjQ5OCAxLjgzMy0uMDM2IDIuOTY0LTEuMTk0IDIuOTY0LTMuNDYxem03Ljk0NiAzLjYybC0uMjcgMi4yMThIODQuNjZWMy4zMTVoMy4xMTJWOS41MmMuNjg5LTEuNTg1IDIuMDU0LTIuNDUgMy45ODUtMi40NSAyLjkyNy4wMzYgNS4wOTIgMi4wMzUgNS4wOTIgNi4wNTd2LjM3OGMwIDQuMDIzLTIuMDU0IDYuMzI2LTUuMTY2IDYuMzI2LTIuMDU0LS4wNDgtMy4zODItLjk4Ny00LjAyMi0yLjU2em01LjkxNi0zLjc2N3YtLjMwNGMwLTIuMjE5LTEuMjE3LTMuNDYyLTIuOTI3LTMuNDYyLTEuNzQ3IDAtMi45NjQgMS4zOS0yLjk2NCAzLjQ5OHYuMjY4YzAgMi4yNTUgMS4xOCAzLjU3MiAyLjkyNyAzLjU3MiAxLjg3IDAgMi45NjQtMS4xNTggMi45NjQtMy41NzJ6bTQuNjM3LjE4M3YtLjM0MWMwLTQuMDU5IDIuNjItNi4yNzcgNi4xODctNi4yNzcgMy42NDEgMCA2LjE4NyAyLjIxOCA2LjE4NyA2LjI3N3YuMzQxYzAgMy45ODYtMi41MDkgNi4xMzEtNi4xODcgNi4xMzEtMy45NDgtLjAzNi02LjE4Ny0yLjEzMy02LjE4Ny02LjEzem05LjEzOS0uMDM2di0uMzA1YzAtMi4yNTUtMS4xNDQtMy42MDgtMi45NjQtMy42MDgtMS43ODMgMC0yLjk2NCAxLjI0My0yLjk2NCAzLjYwOHYuMzA1YzAgMi4xODIgMS4xNDQgMy40MjUgMi45NjQgMy40MjUgMS44MzMtLjAzNyAyLjk2NC0xLjI0NCAyLjk2NC0zLjQyNXptNy40MDUtLjQ1MWwtNC4yOTMtNS44MjdoMy42NzhsMi40NzIgMy42NDUgMi41MDktMy42NDVoMy42NDFsLTQuMzU0IDUuNzlMMTIzIDE5LjQ5aC0zLjYwNGwtMi44MDQtNC4wMjItMi43MzEgNC4wMjJoLTMuNzY0bDQuNjYyLTYuMjl6IiBmaWxsPSIjQjdCRUM5Ii8+PC9zdmc+"
              alt=""
            />
          </div>
        </div>
      </div>
    </div>
    <div id="features">
      <About />
    </div>
    <div>
      <qwe />
      <feat />
      <Testimonial id="testimonial" />
      <Pricing id="pricing" />
      <Faq />
      <Foter />
    </div>
  </div>
</template>

<script setup>
import About from "./Features.vue";
import Testimonial from "./Testimonial.vue";
import Foter from "./Footer.vue";
import qwe from "./QualityFeat.vue";
import Faq from "./Faq.vue";
import feat from "./Feat.vue";
import Pricing from "./Pricing.vue";

import { ref } from "vue";
const isOpen = ref(false);
window.addEventListener("scroll", function () {
  const navbar = document.getElementById("navbar");
  const nav = document.getElementById("rout");
  const btn = document.getElementById("butn");
  const logo = document.getElementById("logotext");
  if (window.scrollY > 5) {
    navbar.classList.add("bg-white", "border", "border-b-gray-200");
    navbar.classList.remove("bg-transparent", "text-white");
    nav.classList.add("text-gray-700");
    btn.classList.add(
      "text-[#1F3E76]",
      "border-[#1F3E76]",
      "hover:bg-[#1F3E76]",
      "hover:text-white"
    );
    btn.classList.remove("border-white", "hover:bg-white", "hover:text-black");
  } else {
    navbar.classList.remove("bg-white", "border", "border-b-gray-200");
    navbar.classList.add("bg-transparent", "text-white");
    btn.classList.remove(
      "text-[#1F3E76]",
      "border-[#1F3E76]",
      "hover:bg-[#1F3E76]",
      "hover:text-white"
    );
    btn.classList.add("border-white", "hover:bg-white", "hover:text-black");
    nav.classList.remove("text-gray-700");
  }
});
const menuOpen=ref(false)
const toggleMenu = () => {
  menuOpen.value = !menuOpen.value;
};
const closeMenu = () => {
  menuOpen.value = false;
};
</script>

<style>
#video {
  width: 880px;
  height: 540px;
}
</style>