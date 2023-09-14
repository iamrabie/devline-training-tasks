<script>

    let faq = [
       'What kinds of homes does Goose build?',
       'Does Goose build customized residences?',
       'What benefits does Goose offer with properties?',
       'What are the available payment options?',
       'Does Goose provide warranty with a property?'
    ];
</script>

<div class="py-4 px-3 mt-[70px] rounded-xl mb-5">
    <h1 class="text-center font-semibold sm:text-2xl md:text-2xl lg:text-4xl text-4xl mx-2 mb-[40px]">Frequently Asked Questions</h1>

    <div class="sm:flex sm:flex-col md:flex md:flex-row flex border mb-5 bg-[#EEE]">

        <div class="sm:w-[100%]  md:w-[60%] sm:mb-5 w-[60%] md:py-1 md:my-auto bg-[#EEE] py-5 my-auto">
            {#each faq as ques}
            <div class="sm:text-sm  sm:py-4 sm:mb-3 sm:px-5 md:text-[13px] lg:text-base  lg:py-4 md:py-2 md:mb-2 md:px-5 flex border border-slate-700 mx-5 justify-between py-5 px-4 mb-2 bg-white rounded-lg">
                <p class="font-semibold">{ques}</p>
                <img src="/assets/arrow-down.jpg" alt=""/>
            </div>
            {/each}
        </div>

        <div class="sm:w-[100%] md:w-[40%] w-[40%]">
           <img src="/assets/faq.jpg" class="sm:w-[100%]"/>
        </div>

    </div>
</div>