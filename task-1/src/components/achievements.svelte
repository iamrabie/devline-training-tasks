<script>
    import Navbar from '../components/navbar.svelte';
  
    let array = [
      {
          img:'/assets/calendar_month.jpg',
          text:'8 years'
      },
      {
          img:'/assets/map.jpg',
          text:'8 locations'
      },
      {
          img:'/assets/home.jpg',
          text:'33 properties'
      },
      {
          img:'/assets/mood.jpg',
          text:'165 clients'
      }
  
    ];
  
</script>
  
<!-- main container -->
<div class="bg-[#002661] h-[250px] flex flex-col py-5">

    <!-- inner container -->
    <div class="mx-auto sm:w-[95%] md:w-[79%] lg:w-[59%] xl:w-[48%]">
  
     <!--  main heading and text -->
      <div class="text-white text-center md:py-5 py-4">
          <h1 class="sm:text-2xl text-4xl">Our achievements </h1>
          <p class="text-sm py-3">We have been one of the most prominent real estate developers in Seattle for over 8 years.</p>
       </div>
  
      <!-- achievements section -->
      <div class="pt-3 sm:mt-5 mt-2 flex justify-between sm:flex-column">
        {#each array as array_items}
          <div class="flex bg-white w-36 justify-center py-2 rounded-lg shadow">
            <img src={array_items.img} alt=""/>
            <p class="px-1">{array_items.text}</p>
           </div>
        {/each}
       </div>
      
    </div>
</div>
  