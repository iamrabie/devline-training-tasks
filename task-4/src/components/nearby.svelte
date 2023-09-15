<script>

    let cafe = [
        {
            cafe:'Queen’s Café',
            img:'/assets/cafe-1.png'
        },
        {
            cafe:'Pizza Heaven',
            img:'/assets/cafe-2.png'
        },
        {
            cafe:'The Hungry Parrots',
            img:'/assets/cafe-3.png'
        },
        {
            cafe:'Dip and Sip',
            img:'/assets/cafe-4.png'
        },
    ];
</script>

<div>
    <div class="w-[90%] mx-auto py-5 flex flex-col">

        <!-- CONTAINER 1 -->
        <div class="flex flex-col py-3">
            <h1 class="text-center py-4 text-3xl font-semibold mb-5">Nearby</h1>
            <div class="flex w-[fit-content] mx-auto mt-2">
                <button class="font-semibold sm:px-[36px] px-[46px] py-2 rounded-3xl sm:mx-1 mx-3 bg-black text-white">Food</button>
                <button class="font-semibold sm:px-[36px] px-[46px] py-2 rounded-3xl sm:mx-1 mx-3 bg-[#EEE]">Shopping</button>
                <button class="font-semibold sm:px-[36px] px-[46px] py-2 rounded-3xl sm:mx-1 mx-3 bg-[#EEE]">Entertaiment</button>
                <button class="font-semibold sm:px-[36px] px-[46px] rounded-3xl mx-3 sm:mx-1 py-2 bg-[#EEE]">Packages</button>
            </div>
        </div>
        <!-- CONTAINER 1 -->

        <!-- CONTAINER 2 -->
        <div class="sm:flex sm:flex-col md:flex md:flex-col lg:flex lg:flex-row flex mt-5">

            <!-- div 1 -->
            <div class="sm:w-[100%] w-[45%]">
                <img src="/assets/nearby-img.png" alt="" class="sm:w-[100%] lg:h-full" />
            </div>

            <!-- div 2 -->
            <div class="sm:w-[100%] w-[55%] sm:px-1 sm:mt-5 sm:mt-0 md:mt-4 xl:mt-5 px-4 flex flex-col">
               {#each cafe as cafes}
               <div class="border flex md:mb-1 lg:mb-1 xl:mb-3 py-1 px-2 rounded-xl">
                  <img src={cafes.img} alt="" />
                  <div class="flex  flex-col md:w-3/4 w-2/4 my-auto px-3">
                    <p class="font-semibold text-lg pty-1">{cafes.cafe}</p>
                    <div class="flex text-sm text-gray-600 pt-[4px]">
                        <p class="pr-2">Cafe</p>
                        <p class="pl-2">in 3 minutes</p>
                    </div>
                  </div>
                  <div class="my-auto">
                    <button class="md:px-[0px] md:w-[160px] lg:w-[140px] px-[26px] bg-[#eee] py-2 font-semibold rounded-3xl">Locate on map</button>
                  </div>
               </div>
               {/each}
               <div class="w-[fit-content] mx-auto flex mt-5">
                 <button class="px-[26px] bg-[#eee] md:py-2 xl:py-2 py-1 font-semibold rounded-3xl mr-3">Previous Page</button>
                 <button class="px-[26px] bg-[#eee] md:py-2 xl:py-2 py-1 font-semibold rounded-3xl ml-3">Next Page</button>
               </div>
            </div>
            <!-- div 2 ends here -->

        </div>
        <!--  CONTAINER 2 -->
    </div>
</div>