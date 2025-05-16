<template>
  <section id="feature" class="pt-20 pb-20 sm:pt-24 sm:pb-24 xl:pt-30 xl:pb-30">
    <div
      class="box-border w-full mx-auto px-5 sm:px-7.5 max-w-full 
             sm:max-w-none md:max-w-[780px] lg:max-w-[1020px] 
             xl:max-w-[1200px] 2xl:max-w-[1310px]"
    >
      <div
    class="w-full flex flex-col items-center mt-[-5px] mb-[50px] sm:mb-[60px] lg:mb-[65px] xl:mb-[75px]"
  >
    <p
      class="text-xs sm:text-sm text-[#244886] font-bold uppercase tracking-[1.5px] sm:tracking-[2px] text-center mb-2 leading-[1.5]"
    >
     
       Quality features
    </p>
    <h2
      class="text-[24px] sm:text-[28px] xl:text-[32px] 2xl:text-[36px] font-bold leading-[1.3] md:leading-[1.2] text-center text-[#0F2137] tracking-[-0.5px]"
    >
     
      Meet exciting feature of app
    </h2>
  </div>
  <div class="grid gap-y-9 w-full mx-auto px-0 pt-0 grid-cols-1
              sm:w-4/5
              md:gap-y-10 md:grid-cols-2 md:w-full
              lg:px-10
              xl:grid-cols-3
              2xl:px-20
              3xl:pt-4">
    
    <div class="flex flex-col items-start text-center px-0
                sm:px-4
                md:px-6
                xl:px-8
                2xl:px-10
                3xl:px-16">
      <img src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTEwIiBoZWlnaHQ9IjExMCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48cGF0aCBkPSJNNzUgMEgzNUMxNS42NyAwIDAgMTUuNjcgMCAzNXY0MGMwIDE5LjMzIDE1LjY3IDM1IDM1IDM1aDQwYzE5LjMzIDAgMzUtMTUuNjcgMzUtMzVWMzVjMC0xOS4zMy0xNS42Ny0zNS0zNS0zNXoiIGZpbGw9IiNFNEZGRUUiLz48cGF0aCBkPSJNNzkuNDc5IDY2LjU4OWwtLjEyLTMuNzM1YTIuMzcgMi4zNyAwIDAwLTIuNDQyLTIuM2wtLjUwNy4wMTVhMjEuMjgyIDIxLjI4MiAwIDAwLTYuMTY0LTEwLjY4NmwtLjAzMi0uMDNhMjEuMzYyIDIxLjM2MiAwIDAwLTYuNDktNC4yMDZsNi41NS0uMmE0LjQgNC40IDAgMDA4LjUtMS43MzIgNC40MTUgNC40MTUgMCAwMC0yLjg0LTMuOTg4IDQuMzUyIDQuMzUyIDAgMDAtMS42OTctLjI3NyA0LjQgNC40IDAgMDAtNC4wNTggMy4wNDVsLTExLjc5MS4zNTMtLjAxMy0uNGEyLjM2OSAyLjM2OSAwIDAwLTIuNDQzLTIuM2wtMy43NzQuMTA1YTIuMzU3IDIuMzU3IDAgMDAtMi4yOTIgMi40MzhsLjAxMy40LTExLjc5MS4zNTRhNC40IDQuNCAwIDAwLTguNSAxLjczMiA0LjQgNC40IDAgMDA4LjU4NiAxLjIxMmw2LjU0OS0uMmEyMS40NSAyMS40NSAwIDAwLTExLjcxMiAxNS42NTNsLS42My4wMTlhMi4zNzcgMi4zNzcgMCAwMC0yLjMgMi40NDZsLjExOSAzLjc1YTIuMzY3IDIuMzY3IDAgMDAyLjQ0MyAyLjNsMy43NTEtLjExMmEyLjM3OCAyLjM3OCAwIDAwMi4zLTIuNDQ2bC0uMTItMy43NTFhMi4zNjcgMi4zNjcgMCAwMC0yLjQ0Mi0yLjNoLS4xMDhhMTguNTI3IDE4LjUyNyAwIDAxMTQuMjA3LTE0LjM2NiAyLjM2NSAyLjM2NSAwIDAwMi4yMTUgMS4zNWwzLjc1MS0uMTEyYTIuMzcgMi4zNyAwIDAwMi4xMjItMS40OCAxOC42IDE4LjYgMCAwMTE1LjA5MyAxMy40ODhsLS4yMzEuMDA3YTIuMzc4IDIuMzc4IDAgMDAtMi4zIDIuNDQ2bC4xMTkgMy43NWEyLjM2OSAyLjM2OSAwIDAwMi40NDMgMi4zbDMuNzUtLjExMmEyLjM1NCAyLjM1NCAwIDAwMi4yODYtMi40M3ptLTQzLjc1My43NThsLTIuNjI5LjA4LS4wODQtMi42MyAyLjYyOS0uMDc5LjA4NCAyLjYzem0zOC41ODMtMjQuOTZhMS40NTYgMS40NTYgMCAxMS0xLjMxOC45NCAxLjQ3MiAxLjQ3MiAwIDAxMS4zMTgtLjk0em0tNDAuMjgzIDQuMTM4YTEuNDU2IDEuNDU2IDAgMTEtLjA4LTIuOTEzIDEuNDU2IDEuNDU2IDAgMDEuMDc5IDIuOTE0em0xOC44NzMtLjcxOWwtLjA4NC0yLjYyOSAyLjYyOS0uMDc5LjA0MiAxLjMwNy4wNDIgMS4zMDctMi42MjkuMDk0em0yMS4wMDYgMjAuMzg4bC0uMDg0LTIuNjI5IDIuNjI5LS4wNzguMDg0IDIuNjI5LTIuNjI5LjA3OHoiIGZpbGw9IiM0MDk3NUYiLz48L3N2Zz4=" alt="default alt text" width="110" height="110" 
           class="mx-auto mb-4 w-20
                  sm:w-24
                  md:mb-5
                  xl:mb-6 xl:w-25
                  2xl:w-auto"/>
      <div class="w-full flex flex-col">
        <h2 class="text-[#0F2137] text-lg font-bold leading-snug mb-3
                   xl:text-xl xl:mb-4">Vector Editing</h2>
        <p class="text-base font-normal leading-relaxed
                  md:leading-loose
                  lg:leading-[2]">Get your blood tests delivered at home collect a sample from the your blood tests.</p>
      </div>
    </div>
    
    <div class="flex flex-col items-start text-center px-0
                sm:px-4
                md:px-6
                xl:px-8
                2xl:px-10
                3xl:px-16">
      <img src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTEwIiBoZWlnaHQ9IjExMCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB4bWxuczp4bGluaz0iaHR0cDovL3d3dy53My5vcmcvMTk5OS94bGluayI+PHBhdGggb3BhY2l0eT0iLjA5IiBkPSJNNzUgMEgzNUMxNS42NyAwIDAgMTUuNjcgMCAzNXY0MGMwIDE5LjMzIDE1LjY3IDM1IDM1IDM1aDQwYzE5LjMzIDAgMzUtMTUuNjcgMzUtMzVWMzVjMC0xOS4zMy0xNS42Ny0zNS0zNS0zNXoiIGZpbGw9IiMyNTYzRkYiLz48cGF0aCBmaWxsPSJ1cmwoI3BhdHRlcm4wKSIgZD0iTTMyIDMyaDQ2djQ2SDMyeiIvPjxkZWZzPjxwYXR0ZXJuIGlkPSJwYXR0ZXJuMCIgcGF0dGVybkNvbnRlbnRVbml0cz0ib2JqZWN0Qm91bmRpbmdCb3giIHdpZHRoPSIxIiBoZWlnaHQ9IjEiPjx1c2UgeGxpbms6aHJlZj0iI2ltYWdlMCIgdHJhbnNmb3JtPSJzY2FsZSguMDIxNzQpIi8+PC9wYXR0ZXJuPjxpbWFnZSBpZD0iaW1hZ2UwIiB3aWR0aD0iNDYiIGhlaWdodD0iNDYiIHhsaW5rOmhyZWY9ImRhdGE6aW1hZ2UvcG5nO2Jhc2U2NCxpVkJPUncwS0dnb0FBQUFOU1VoRVVnQUFBQzRBQUFBdUNBWUFBQUJYdVNzM0FBQUFCSE5DU1ZRSUNBZ0lmQWhraUFBQUJOSkpSRUZVYUlIdDJXdW9YY1VWQi9EZk9ibStxb2lLV256VUIzZ25Sa3RCcGFhVWZxZ0thb3dhUlZFeFdORTdTaFdiS0ttbUZ2cXRIeFNVeHZoQWNkUWdpaUJFYTMzRVozd2dWRnRmVkt4bDFBOGFmQVV0OFVIVjF1VDB3OTRuZCtmY2ZlNDk5NXg3Y2tIOHc0YTExNW8xOHo5ejFxdzlhNmJSYXJXRWFIY3N3eG5ZSGsvZzJweThiaFlSb24xS1hpZWdpWWR3WFU3ZWJZeU90ZllvRlVkMitQMGJDM0x5dDYzS3RrU0k1dU11SE5SaGVoc25qT0MzSnBLRzNiQXlSTDhmSXI4Tk9YbWxpKzE0RTBrcmRYOXNqSTYxM3NWK1E2TTJPVnBZbHBNL2RScEMxTVJWdUx6RzcvMFJSVXpQRmhvcWt4YWluK0FjTE0vSkpsd1JvaGF1NlBEYlprU3hFQmQzNlhnZGJ1K0QwSUg0VlNrL2kyZTZ0RnVQdTB2U2gyTTFEc0R1SWJvZ0o5L21aSG1JdnNFZktuN3ZORWJIV29maU9VVk1kK0xjbk53NVhkWWhPaEl2bHE5WDV1U3FLZG9maktld2QwVjlXMDVpcGMzVnhtZitsR1pPM3NCQ1BGOXhlZ2ZuOTBPNnhFNFZlZEpRRE5FOHJPa2dEV01odXJYOWtwUGxXS0ZZRXcrTWxNb1hRdlM3Q3ZsVk9ibWpUOUk5STBRL3hsOFU0VkdIR0tML1lVa1pOcGUxRGMxS28yMHI4c2pNMDl3U0lUb0VmMWFzaDhsd0VWYUZ1Q1duNmt0amhybDFSWWptNGhIczM2UEw2OWhVVlF4clp1ZFU1T3EvS2tSSDRINzhxTWUrWWs1dTYxUTI2MXJPQUQ2cHlGKzBoWEttVit1ZDlOSTYwZ3hweG5QeWFvaE9WeXk2TzltYzhoN1hPK2tsT2JtKzlGMkVuWEZYVGxvTWNSSG1aSFZiTGxQZUkzb25mVWxPYml4OUQxY3NZb3AvY2czREM1WE5LRlBldzdxbnZFNzhwazI2UlBYRHVFOWJHR3JhQzlFb0hxME9PQWxhdURRbk4zVG9xOWxrWTFzWTlveC9obi8yMkRibVpHV3ZIUStGZUloMmhKeXNWMVJWM1RaWmJTek5hWHFidVJrblhxYTh2NGZvWXNqSkJweWsyQ1hXWWVsMFpycU5ic1MvbVc1SEVLSWY0akhNdzNVaHVoQnk4aVZPTm5IbWwvUkErajkxeW02TGMzNkl6dXVCNjBjNUZlbXB4R0xqbi9FUjNCeWk3WE95TWllZmgraFV4UWZvYUZ1bXZPT3hWNWN4NWsySCtLTHltUkloT2pNbjk1YXZaM2VZRzFnUm9rMDV1U0VuRzBLMEdEL1B5WDJsLzNGczhlTjd3a3lrdzFaSllDNE9yYkUzY0gySU51TG1uSHhFUWJycVAxMTBJLzVBK1V5RkQzUHlhQ2tmWS9LaTRTWThqWDlWbFRsNVBFUUxUQjRxRXdybWJzUmY3S09RT0dzSysyVjRxODVRK2ZFVEVLS2ZtUWJ4N2FZZzBkbjVJdnlpeHZRcFhzS0t5Y2hOZ1IvVUtRZU84UkF0eEQzR0M1RXZGQnVxQjdFMkp4OE9Pa1lkQmlJZW9nTnhMM1lvVlN0eFRVN1dEVXBzS2d3NjR4dU5iM3h1eWNuU3RpRkVlMlBQbkx3MjRCaTFHT2lUbjVQM01CL0g1T1RYYlgySTlzTmY4WEtJRTNMN2pHRGdHTS9KbTNpelF6M1grTkhhSVlPT1VZZGhiV3MzVnVSdmh6SEEwQ3VnWWVGNzRsc2Izd25pMVExN1g0WEVrRkRsOVhWYmFFS0k5bWY4SkJTbmhlaW9yVVNzSzhyem1Pb2QxSVhsT1l0bWVTVzNSbEhVdG5FRW5nalJzWDJPK1ZWRi9tOC9IWVFvS09yVWt5cnFYK0xKRVAxMEJGZXFMNC9tNEpvUVhkckh1SWRWNUxraE9ycVBQcFpoanhyOXJyaTZNVHJXV29kOSsraDROckcraVcxbW0wVWZtRE9pMkR0M3ErZ3prMTg4RFJIbnF5OU9JRGRHeDFxaldLcytYRTdOYWZOSjZWWkZlZWY1TEhicE1IMkZFNXM1ZVFzTEZFZTVIeWp1SHAvSEtiTkZHbkx5RHh5ck9GUC9BQjhyczB4TzF2NGZKNU5NOVBKeE9Fa0FBQUFBU1VWT1JLNUNZSUk9Ii8+PC9kZWZzPjwvc3ZnPg==" alt="default alt text" width="110" height="110" 
           class="mx-auto mb-4 w-20
                  sm:w-24
                  md:mb-5
                  xl:mb-6 xl:w-25
                  2xl:w-auto"/>
      <div class="w-full flex flex-col">
        <h2 class="text-[#0F2137] text-lg font-bold leading-snug mb-3
                   xl:text-xl xl:mb-4">Customize & Monitoring</h2>
        <p class="text-base font-normal leading-relaxed
                  md:leading-loose
                  lg:leading-[2]">Get your blood tests delivered at home collect a sample from the your blood tests.</p>
      </div>
    </div>
    
    <div class="flex flex-col items-start text-center px-0
                sm:px-4
                md:px-6
                xl:px-8
                2xl:px-10
                3xl:px-16">
      <img src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTEwIiBoZWlnaHQ9IjExMCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48cGF0aCBvcGFjaXR5PSIuMTAyIiBkPSJNNzUgMEgzNUMxNS42NyAwIDAgMTUuNjcgMCAzNXY0MGMwIDE5LjMzIDE1LjY3IDM1IDM1IDM1aDQwYzE5LjMzIDAgMzUtMTUuNjcgMzUtMzVWMzVjMC0xOS4zMy0xNS42Ny0zNS0zNS0zNXoiIGZpbGw9IiNGRjQzNjEiLz48cGF0aCBkPSJNNTYuMjI3IDg0aC0uMTM3YTI1LjEwNiAyNS4xMDYgMCAwMS01LjY5My0uNjU4Ljk0OC45NDggMCAwMS0uNzA2LTEuMTM4LjkzNC45MzQgMCAwMTEuMTI2LS43MTMgMjMuNDYgMjMuNDYgMCAwMDQuNDg4LjU4NlY4MC4yYS45MzkuOTM5IDAgMTExLjg3OSAwdjEuODdhMjMuMTEyIDIzLjExMiAwIDAwOS44MjUtMi43bC0uOTI2LTEuNjIyYS45NTUuOTU1IDAgMDEuNjkyLTEuNDIuOTMxLjkzMSAwIDAxLjkzNS40NjdsLjkyMyAxLjYxOGEyMy44MDggMjMuODA4IDAgMDA3LjMtNy4zODRsLTEuNi0uOTM0YS45NTYuOTU2IDAgMDEuMjI1LTEuNzQyLjkzNS45MzUgMCAwMS43MTQuMDk1bDEuNi45MzdhMjMuNzc3IDIzLjc3NyAwIDAwMi42NzctMTAuMDg5SDc3LjdhLjk1Ljk1IDAgMDEwLTEuOWgxLjg1NmEyMy43NjggMjMuNzY4IDAgMDAtMi42NzctMTAuMDg3bC0xLjYuOTM2YS45MjQuOTI0IDAgMDEtLjk0IDAgLjk1NS45NTUgMCAwMTAtMS42NDdsMS41OTktLjkzM2EyMy44MSAyMy44MSAwIDAwLTcuMy03LjM4NWwtLjkyMyAxLjYxOGEuOTM0LjkzNCAwIDAxLTEuMjg0LjM0OC45NTYuOTU2IDAgMDEtLjM0NS0xLjNsLjkyNy0xLjYyMmEyMy4xMDkgMjMuMTA5IDAgMDAtOS44MjUtMi43djEuODcxYS45NC45NCAwIDAxLTEuODggMHYtMS44NzdhMzEuNSAzMS41IDAgMDAtLjg2OC4wNTRsLTEuMDA5LjA3OGEyMy44NSAyMy44NSAwIDAwLTIuNjEyLjQ1NC45MzguOTM4IDAgMDEtMS4xMjYtLjcxNC45NDguOTQ4IDAgMDEuNzA2LTEuMTM4Yy45OTgtLjIzIDIuMDEtLjQgMy4wMjktLjUwOXYtMS4xaC0xLjQwOWEyLjM3NSAyLjM3NSAwIDAxMC00Ljc0OWg4LjQ1N2EyLjM3NSAyLjM3NSAwIDAxMCA0Ljc1aC0xLjQwOXYxLjEzMWEyNSAyNSAwIDAxOS42NTMgMy4yMzRjLjAyLjAxMS4wNDEuMDEuMDYuMDIxLjAxOS4wMTIuMDI5LjAzLjA0Ny4wNDJhMjUuNDY5IDI1LjQ2OSAwIDAxNC41MTkgMy4zODhsMi4wMTktMi4wMzktMS4zMjktMS4zNDUgMy45ODctNC4wMyAzLjk4NiA0LjAzLTMuOTg2IDQuMDMtMS4zMjktMS4zNDMtMi4wMTggMi4wNGEyNS43OSAyNS43OSAwIDAxMy4zNSA0LjU2OGMuMDEzLjAxNy4wMy4wMy4wNDEuMDQ3LjAxMS4wMTguMDEuMDQxLjAyLjA2MWEyNS44IDI1LjggMCAwMTAgMjUuNTNjLS4wMS4wMi0uMDA5LjA0LS4wMi4wNi0uMDExLjAxOC0uMDM5LjA0OC0uMDU3LjA3NGEyNS43IDI1LjcgMCAwMS05LjE4NCA5LjI3M2MtLjAxOC4wMTItLjAyOC4wMy0uMDQ3LjA0MWEuODU1Ljg1NSAwIDAxLS4wODguMDM4IDI1IDI1IDAgMDEtMTIuNDIyIDMuMzk0aC0uMDIzYy0uMDA5IDAtLjAxMy4wMTEtLjAxOS4wMTF6bTIwLjQ2MS00Ny44MTRsMS4zMyAxLjM0NSAxLjMyOC0xLjM0NS0xLjMyOC0xLjM0NC0xLjMzIDEuMzQ0em0tMTkuNS0zLjQ2di0yLjg3aDMuMjg5YS40NzUuNDc1IDAgMDAwLS45NUg1Mi4wMmEuNDc1LjQ3NSAwIDEwMCAuOTVoMy4yOHYyLjg3Yy4xMTMtLjAwNi4yMTYgMCAuMzI1LS4wMDguMTU0IDAgLjMwOC0uMDEzLjQ2Mi0uMDEzaC4xNTNjLjMwNC0uMDA1LjYxNi4wMDEuOTQzLjAxNWwuMDA1LjAwNXpNNDEuMjEzIDc1LjQ1M2EuOTUuOTUgMCAxMTAtMS45aDYuNTc3YS45NS45NSAwIDAxMCAxLjloLTYuNTc3em0tNS42MzgtNi42NWEuOTUuOTUgMCAwMTAtMS45aDEyLjIxNmEuOTUuOTUgMCAxMTAgMS45SDM1LjU3NXptMTguODM1LTYuNjkyYTMuNDA4IDMuNDA4IDAgMDEuNC01LjEzbDEyLjE2NS04LjlhLjkzNS45MzUgMCAwMTEuMjE1LjEuOTU4Ljk1OCAwIDAxLjEgMS4yMjdsLTguOCAxMi4zYTMuMzM0IDMuMzM0IDAgMDEtNCAxLjEzNyAzLjMyNCAzLjMyNCAwIDAxLTEuMDg1LS43MzlsLjAwNS4wMDV6bTEuNS0zLjU5NWExLjQ4NSAxLjQ4NSAwIDAwLjk3OSAyLjY4MiAxLjQ2NiAxLjQ2NiAwIDAwMS4wNzUtLjYwOGw1LjM2Ny03LjUtNy40MjEgNS40MjZ6bS0yNS45NzYgMy42MzZhLjk1Ljk1IDAgMDEwLTEuOWgxNy44NTRhLjk1Ljk1IDAgMTEwIDEuOUgyOS45MzR6bTMuNzU5LTYuNjQ5YS45NS45NSAwIDAxMC0xLjloMTQuMDk1YS45NS45NSAwIDAxMCAxLjlIMzMuNjkzem00LjctNi42NWEuOTUuOTUgMCAxMTAtMS45aDkuNGEuOTUuOTUgMCAxMTAgMS45aC05LjR6bTQuNy02LjY1YS45NS45NSAwIDExMC0xLjloNC43YS45NS45NSAwIDAxMCAxLjloLTQuN3oiIGZpbGw9IiNGRjQzNjEiLz48L3N2Zz4=" alt="default alt text" width="110" height="110" 
           class="mx-auto mb-4 w-20
                  sm:w-24
                  md:mb-5
                  xl:mb-6 xl:w-25
                  2xl:w-auto"/>
      <div class="w-full flex flex-col">
        <h2 class="text-[#0F2137] text-lg font-bold leading-snug mb-3
                   xl:text-xl xl:mb-4">Quality & Short-period</h2>
        <p class="text-base font-normal leading-relaxed
                  md:leading-loose
                  lg:leading-[2]">Get your blood tests delivered at home collect a sample from the your blood tests.</p>
      </div>
    </div>
  </div>
    </div>
  </section>
  <div
    class="w-full max-w-full mx-auto px-5 flex items-center justify-between flex-col sm:px-[30px] md:max-w-[780px] lg:max-w-[1020px] xl:max-w-[1200px] 2xl:max-w-[1310px] md:flex-row"
  >
    <div
      class="pl-0 pr-0 order-2 sm:pl-[25px] sm:pr-[25px] md:order-0 lg:pl-[50px] xl:pl-[95px] xl:pr-[75px] 2xl:pr-[95px]"
    >
      <img
        src="https://startup-app-modern.vercel.app/_next/static/images/coreFeature-eeb06038997d171c096c54579e1a2dfe.png"
        alt="Thumbnail"
        width="380"
        height="660"
        class="max-w-full h-auto"
      />
    </div>

    <div
      class="w-full pr-0 pl-auto shrink-0 sm:w-[450px] sm:pr-auto md:w-[350px] lg:w-[500px] xl:w-[570px] xl:pr-[80px]"
    >
      <div
        class="pl-0 mb-[15px] text-center md:text-left lg:pl-[35px] lg:mb-[5px] xl:pl-[55px] 2xl:pl-[30px]"
      >
        <div class="flex flex-col items-start shrink-0">
          <div class="w-full flex flex-col mt-[-5px]">
            <p
              class="text-[12px] text-[#244886] tracking-[2px] uppercase font-bold mb-[10px] leading-[1.5] sm:text-[14px] lg:mb-[15px]"
            >
              Core features
            </p>
            <h2
              class="font-['DM_Sans'] font-bold text-[24px] text-[#0F2137] leading-[1.35] tracking-[-0.5px] mb-[25px] sm:text-[28px] md:text-[32px] md:leading-[1.3] lg:text-[36px] lg:leading-[1.2] xl:text-[42px] 2xl:text-[46px]"
            >
              Smart Jackpots that you may love this anytime &amp; anywhere
            </h2>
          </div>
        </div>
      </div>

      <div
        class="grid gap-y-[15px] grid-cols-1 pb-[35px] px-0 lg:px-[20px] lg:pb-[40px] xl:px-[40px] 2xl:px-0 2xl:pb-0"
      >
        <div
          class="flex items-start bg-white rounded-[10px] transition-all w-full mx-auto px-[17px] pb-[20px] sm:w-[85%] md:p-0 md:w-full lg:p-[20px_15px_17px] 2xl:p-[25px_30px_23px] lg:hover:shadow-[0px_8px_24px_rgba(69,88,157,0.07)]"
        >
          <img
            src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNTciIGhlaWdodD0iNTciIGZpbGw9Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PHBhdGggb3BhY2l0eT0iLjEiIGZpbGwtcnVsZT0iZXZlbm9kZCIgY2xpcC1ydWxlPSJldmVub2RkIiBkPSJNMjQuNTQyLjc5Mmg3LjkxNmMxMy4xMTcgMCAyMy43NSAxMC42MzMgMjMuNzUgMjMuNzV2Ny45MTZjMCAxMy4xMTctMTAuNjMzIDIzLjc1LTIzLjc1IDIzLjc1aC03LjkxNmMtMTMuMTE3IDAtMjMuNzUtMTAuNjMzLTIzLjc1LTIzLjc1di03LjkxNmMwLTEzLjExNyAxMC42MzMtMjMuNzUgMjMuNzUtMjMuNzV6IiBmaWxsPSJ1cmwoI3BhaW50MF9saW5lYXIpIi8+PHBhdGggZmlsbC1ydWxlPSJldmVub2RkIiBjbGlwLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik0zMS4yMTcgMzIuOTYyYS44My44MyAwIDAwLjI1Mi0uNjAzdi0yLjE0NGg4LjkwNnY2LjQzM2MwIC41OS0uMjA4IDEuMDk0LS42MjMgMS41MTRhMi4wMyAyLjAzIDAgMDEtMS40OTguNjNIMTguNzQ3YTIuMDMgMi4wMyAwIDAxLTEuNDk4LS42MyAyLjA3NiAyLjA3NiAwIDAxLS42MjMtMS41MTR2LTYuNDMzaDguOTA2djIuMTQ0YS44My44MyAwIDAwLjI1Mi42MDMuODEuODEgMCAwMC41OTYuMjU1aDQuMjQyYS44MS44MSAwIDAwLjU5Ni0uMjU1em0tMS4wMi0yLjc0N2gtMy4zOTR2MS43MTVoMy4zOTR2LTEuNzE1em05LjU1NS03Ljk0OGEyLjAyOSAyLjAyOSAwIDAwLTEuNDk4LS42M0gzMy41OXYtMi4xNDRhMS4yNSAxLjI1IDAgMDAtLjM3LS45MTIgMS4yMjIgMS4yMjIgMCAwMC0uOTAyLS4zNzVoLTcuNjM0Yy0uMzUzIDAtLjY1NC4xMjYtLjkwMS4zNzVhMS4yNSAxLjI1IDAgMDAtLjM3MS45MTJ2Mi4xNDRoLTQuNjY1YTIuMDMgMi4wMyAwIDAwLTEuNDk4LjYzYy0uNDE2LjQyLS42MjMuOTI0LS42MjMgMS41MTR2NS4xNDdoMjMuNzV2LTUuMTQ3YzAtLjU5LS4yMDgtMS4wOTQtLjYyMy0xLjUxNHptLTcuODYtLjYzaC02Ljc4NXYtMS43MTZoNi43ODZ2MS43MTZ6IiBmaWxsPSIjRkY0NTUwIi8+PGRlZnM+PGxpbmVhckdyYWRpZW50IGlkPSJwYWludDBfbGluZWFyIiB4MT0iMzIuNzg1IiB5MT0iODkuNzg1IiB4Mj0iODkuNzg1IiB5Mj0iMjQuMjE1IiBncmFkaWVudFVuaXRzPSJ1c2VyU3BhY2VPblVzZSI+PHN0b3Agc3RvcC1jb2xvcj0iI0ZGNDE2QyIvPjxzdG9wIG9mZnNldD0iMSIgc3RvcC1jb2xvcj0iI0ZGNEIyQiIvPjwvbGluZWFyR3JhZGllbnQ+PC9kZWZzPjwvc3ZnPg=="
            width="55"
            height="55"
            class="shrink-0 w-[50px] mr-[15px] sm:mr-[20px] sm:w-[55px]"
          />
          <div class="w-full flex flex-col mt-[-5px]">
            <h2
              class="font-['DM_Sans'] font-bold text-[18px] text-[#0F2137] leading-[1.4] mb-[10px] lg:mb-[15px]"
            >
              Smart Features
            </h2>
            <div class="text-[15px] font-normal leading-[1.85] sm:leading-[2]">
              Get your blood tests delivered at let home collect sample from the
              victory of the managements. your blood tests.
            </div>
          </div>
        </div>

        <div
          class="flex items-start bg-white rounded-[10px] transition-all w-full mx-auto px-[17px] pb-[20px] sm:w-[85%] md:p-0 md:w-full lg:p-[20px_15px_17px] 2xl:p-[25px_30px_23px] lg:hover:shadow-[0px_8px_24px_rgba(69,88,157,0.07)]"
        >
          <img
            src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNTciIGhlaWdodD0iNTciIGZpbGw9Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PHBhdGggb3BhY2l0eT0iLjEiIGZpbGwtcnVsZT0iZXZlbm9kZCIgY2xpcC1ydWxlPSJldmVub2RkIiBkPSJNMjQuNTQyLjc5Mmg3LjkxNmMxMy4xMTcgMCAyMy43NSAxMC42MzMgMjMuNzUgMjMuNzV2Ny45MTZjMCAxMy4xMTctMTAuNjMzIDIzLjc1LTI3Ljc1IDIzLjc1aC03LjkxNmMtMTMuMTE3IDAtMjMuNzUtMTAuNjMzLTIzLjc1LTIzLjc1di03LjkxNmMwLTEzLjExNyAxMC42MzMtMjMuNzUgMjMuNzUtMjMuNzV6IiBmaWxsPSJ1cmwoI3BhaW50MF9saW5lYXIpIi8+PHBhdGggZmlsbC1ydWxlPSJldmVub2RkIiBjbGlwLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik00Mi4zOSAyNS4yMjFhLjgzMy44MzMgMCAwMS0uMDIzLjI0NmwtMS44MDYgNy4yNTdhLjgyMy44MjMgMCAwMS0uNzkzLjYyNGwtMTAuODQuMDU1SDE4LjA4MmEuODIyLjgyMiAwIDAxLS43OTctLjYyNWwtMS44MDctNy4yODVhLjgyOC44MjggMCAwMS0uMDIyLS4yNTIgMS43MzMgMS43MzMgMCAwMS41MTgtMy4zODMgMS43MzMgMS43MzMgMCAwMTEuMDk1IDMuMDdsMi4yNjIgMi4yODdhMy4wOCAzLjA4IDAgMDAyLjE3Ni45MSAzLjA4IDMuMDggMCAwMDIuNDUxLTEuMjI0bDMuNzE4LTQuOTQ2YTEuNzMgMS43MyAwIDAxMS4yMTktMi45NTYgMS43MyAxLjczIDAgMDExLjI0NSAyLjkyNmwuMDA0LjAwNCAzLjY5IDQuOTZhMy4wNzggMy4wNzggMCAwMDIuNDU3IDEuMjM2Yy44MTkgMCAxLjU5LS4zMiAyLjE2OC0uOTAxbDIuMjc3LTIuMjg3YTEuNzMgMS43MyAwIDAxMS4wOC0zLjA4IDEuNzMgMS43MyAwIDAxLjU3MiAzLjM2NHptLTIuMDA2IDEwLjc2NmEuODIzLjgyMyAwIDAwLS44Mi0uODI1SDE4LjMyYS44MjMuODIzIDAgMDAtLjgyMi44MjV2MS45NzljMCAuNDU2LjM2OC44MjUuODIyLjgyNWgyMS4yNDNhLjgyMy44MjMgMCAwMC44MjEtLjgyNXYtMS45OHoiIGZpbGw9IiNGRTU4NjgiLz48ZGVmcz48bGluZWFyR3JhZGllbnQgaWQ9InBhaW50MF9saW5lYXIiIHgxPSIzMi43ODUiIHkxPSI4OS43ODUiIHgyPSI4OS43ODUiIHkyPSIyNC4yMTUiIGdyYWRpZW50VW5pdHM9InVzZXJTcGFjZU9uVXNlIj48c3RvcCBzdG9wLWNvbG9yPSIjRkY1ODU4Ii8+PHN0b3Agb2Zmc2V0PSIxIiBzdG9wLWNvbG9yPSIjRjg1N0E2Ii8+PC9saW5lYXJHcmFkaWVudD48L2RlZnM+PC9zdmc+"
            width="55"
            height="55"
            class="shrink-0 w-[50px] mr-[15px] sm:mr-[20px] sm:w-[55px]"
          />
          <div class="w-full flex flex-col mt-[-5px]">
            <h2
              class="font-['DM_Sans'] font-bold text-[18px] text-[#0F2137] leading-[1.4] mb-[10px] lg:mb-[15px]"
            >
              Secure Contents
            </h2>
            <div class="text-[15px] font-normal leading-[1.85] sm:leading-[2]">
              Get your blood tests delivered at let home collect sample from the
              victory of the managements. your blood tests.
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
</script>