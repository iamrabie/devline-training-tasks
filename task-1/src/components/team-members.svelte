<script>

      let team_members = [
        {
            image:'/assets/team-member1.png',
            name:'Amin Shariat',
            role:'land aquicision'
        },
        {
            image:'/assets/team-member2.png',
            name:'Andrew McLane',
            role:'land aquicision'
        },
        {
            image:'/assets/team-member3.png',
            name:'Kianna Dicus',
            role:'Marketing and Office Manager'
        }
       ];

</script>

<!-- main container -->
<div class="flex flex-col py-2 md:bg-white bg-[#FAFAFA]">

    <!-- heading -->
    <h1 class="sm:text-2xl text-4xl font-semibold text-center sm:py-3 py-5 mt-1">Meet the team</h1>
  
    <!-- team members container -->
    <div class="sm:my-1 py-5 my-3">
  
       <!-- inner div that holds content; team member's image, name etc -->
       <div class="sm:flex-none sm:w-[fit-content] md:flex xl:flex md:justify-between xl:justify-between md:w-[98%] xl:w-[92%] mx-auto">
  
        <!--  each loop for itearing the team members -->
        {#each team_members as member}
          <div class="flex flex-col w-[fit-content] sm:py-2 py-4 sm:px-2 px-4 sm:mb-4 bg-white rounded-md">
            <img src={member.image} class="sm:w-[300px] md:w-[270px] lg:w-[340px] sm:h-[365px] md:h-[280px] lg:h-[405px]" alt="" />
            <h1 class="sm:text-lg text-2xl font-bold mt-1">{member.name}</h1>
            <p class="sm:text-[15px] text-[18px] p-0">{member.role}</p>
          </div>
        {/each}
       </div>
  
    </div>
  
</div>
  

