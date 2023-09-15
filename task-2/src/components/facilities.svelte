<script>

  let facilities = [
    {
        heading:'Developing existing Residential Lots',
        text:'We buy existing residential lots, often demolish these, and build multifamily residences.'
    },
    {
        heading:'Earnest Money to Sellers',
        text:'Sellers who work with us earn non-refundable earnest money to guarantee our performance while we wait for permit'
    },
    {
        heading:'Enhancing the Seattle Neighborhoods',
        text:'Goose Development has been sourcing and developing projects focusing on enhancing the character, community, and appeal of Seattle neighborhoods.'
    },
    {
        heading:'We Build the Best Structure Possible',
        text:'We and our partners handle the entire process from land acquisition to finishing touches throughout all our properties that ensures maximizing both community and stakeholder benefits.'
    },
  ];
</script>

<div class="py-5 py-4 px-3">
    <h1 class="font-semibold text-4xl text-center py-5 mb-4 sm:text-xl md:text-2xl ">We provide attractive facilities for our clients.</h1>
    <div class="sm:flex sm:flex-col md:flex md:flex-col xl:flex xl:flex-row flex">
        <div class="sm:w-[100%] md:w-[100%] w-[50%] pt-3">
            {#each facilities as facility}
              <h1 class="font-semibold w-3/4 bold text-xl">{facility.heading}</h1>
              <p class="text-base sm:w-[100%] w-3/4 leading-6 py-3">{facility.text}</p>
           {/each}
        </div>
        <div class="sm:w-[100%] md:w-[100%] w-[50%] sm:mt-2">
           <img src="/assets/facility.png" alt="" class="sm:mx-0 sm:w-[100%] mx-auto" />
        </div>
    </div>
</div>