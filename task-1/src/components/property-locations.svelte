<script>
    let properties = [
    {
        img:'/assets/property1.png',
        name:'Northwest Seattle',
        props :1,
        available:4
    },
    {
        img:'/assets/property2.png',
        name:'Northwest Seattle',
        props :10,
        available:5
    },
    {
        img:'/assets/property3.png',
        name:'Greenlake-Fremont-Wallingford',
        props :20,
        available:5
    },
    {
        img:'/assets/property2.png',
        name:'Queen Anne-Magnolia',
        props :10,
        available:5
    },
    {
        img:'/assets/property2.png',
        name:'Central District',
        props :12,
        available:8
    },
    {
        img:'/assets/property1.png',
        name:'West Seattle-Delridge',
        props :10,
        available:5
    },
    {
        img:'/assets/property2.png',
        name:'Southeest Seattle',
        props :5,
        available:3
    }

  ];

</script>

<!-- main container -->
<div class="py-5">
    <!-- main heading -->
    <h1 class="text-center sm:text-2xl md:text-3xl lg:text-3xl xl:text-3xl font-semibold sm:py-2 sm:my-3 md:py-5 md:mt-5 md:mb-4 lg:py-5 lg:mt-5 lg:mb-4 xl:py-5 xl:mt-5 xl:mb-4">Our property locations</h1>

    <!--  projects container -->
    <div class="w-[92%] mx-auto sm:grid-cols-1 grid md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-3 sm:gap-4 gap-8 justify-center">

        <!--   project card -->
        {#each properties as property}
        <div class="flex flex-col w-[fit-content] sm:p-2 p-3 bg-white rounded-md border border-gray-300 mx-auto">
            <img src={property.img} class="w-[380px] h-[224px]" />
            <h1 class="sm:text-lg text-2xl font-bold mt-2">{property.name}</h1>

            <div class="flex w-64 justify-between text-sm mt-1 mb-1">
                <div class="flex">
                    <img src="/assets/home.jpg" class="pr-1"/>
                    <p class="pt-1">{property.props} properties</p>
                </div>
                <div class="flex">
                    <img src="/assets/map.jpg" class="pr-1"/>
                    <p class="pt-1">{property.available} availability</p>
                </div>
                
            </div>

            <div class="flex w-[fit-content] bg-[#EEE] rounded-2xl pl-5 pr-3 py-1 mt-5 mb-4">
                <button class="sm:text-sm text-base">See properties</button>
                <img src="/assets/arrow_forward.png"  class="text-sm px-1 pt-1"/>
            </div>
        </div>
        {/each}
    </div>
</div>