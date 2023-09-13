<script>

    let faq = [
       'What kinds of homes does Goose build?',
       'Does Goose build customized residences?',
       'What benefits does Goose offer with properties?',
       'What are the available payment options?',
       'Does Goose provide warranty with a property?'
    ];
</script>

<div class="py-4 px-3 mt-[70px] border-2 border-green-900 rounded-xl mb-5">
    <h1 class="text-center font-semibold text-4xl mx-2 mb-[40px]">Frequently Asked Questions</h1>

    <div class="flex border mb-5 bg-[#EEE]">

        <div class="w-[60%] bg-[#EEE] py-5 my-auto">
            {#each faq as ques}
            <div class="flex border border-blue-900 mx-5 justify-between py-5 px-4 mb-2 bg-white rounded-lg">
                <p class="font-semibold">{ques}</p>
                <img src="/assets/arrow-down.jpg" alt="" />
            </div>
            {/each}
        </div>

        <div class="w-[40%]">
           <img src="/assets/faq.jpg" />
        </div>

    </div>
</div>