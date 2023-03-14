<template>
    <div class="calculators">
        <h1 class="text-center" style="color: black; font-size:19px;">calculators</h1>
        <div class="container rankers">
            <div class="container category" v-for="(category, i) in categories" :key="i">
                <div class="top-bar">
                    <p>Top 10 {{ category }}</p>
                </div>
                <div class="content">
                    <p>{{ sliced_info(category_dict[category]) }}</p>
                    <!--Change this to open each indicidual category-->
                    <p class="text-cente"><a href="#">Read More</a></p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data () {
        return {
            categories : ["Insurance Companies", "Saving Accounts", "Mobile Loans Apps", "Mortgage","International Money Transfer"],
            category_dict : {
                "Insurance Companies": "The top 10 insurance companies in Kenya are dominated by big players such as Jubilee Insurance, Britam, and APA Insurance. These companies offer a range of insurance products including health, motor, and life insurance.",
                "Saving Accounts": "In Kenya, the top 10 saving accounts offer competitive interest rates and convenient features such as online banking and mobile banking. Some of the popular banks offering these accounts are Equity Bank, KCB Bank, and Co-operative Bank.",
                "Mobile Loans Apps": "Mobile loans apps have become increasingly popular in Kenya due to their accessibility and ease of use. Some of the top 10 mobile loans apps in Kenya include Tala, Branch, and Zenka, which offer instant loans to users through their mobile phones.",
                "Mortgage": "Owning a home is a dream for many Kenyans, and mortgage providers have made it easier to achieve this dream. The top 10 mortgage providers in Kenya include KCB Bank, HF Group, and Standard Chartered Bank, which offer flexible repayment terms and competitive interest rates.",
                "International Money Transfer": "Kenya has a thriving remittance industry, with many Kenyans living abroad sending money back home. The top 10 international money transfer services in Kenya include Western Union, MoneyGram, and WorldRemit, which offer fast and secure transfer options.",
            },

        }
    },

    methods : {
        sliced_info (n) {
            return (n.slice(0, 80) +" ...");
        },
    }
}
</script>

<style>
    .calculators {
        background-color: #f6f7f8;
        margin-top: -20px;
        padding: 20px;
        margin-bottom: 40px;
    }

    .calculators .rankers{
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        grid-auto-rows: minmax(200px, auto);
        grid-gap: 10px;
    }
    .category {
        background-color: #ffffff;
        box-shadow: -1px 1px 4px rgba(0, 0, 0, 0.2);
        padding: 10px;
        border-radius: 4px;
    }

</style>