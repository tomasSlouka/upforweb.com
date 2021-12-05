<template>
    <div class="component relative" id="sms">

        <div class="header grid relative align-items-center">
            <img src="@/assets/img/arrow_back_black_24dp.svg" alt="" class='absolute' />
            <div class="name justify-self-center grid align-items-center">NCZI</div>
        </div>

        <div class='mt20 grid gap-20'>
            <div class="message justify-self-end">
                <div class='grid gap-2 col-2 auto justify-content-end time'>
                    <div>5.12. 9:14</div>
                    <div><img src="@/assets/img/sim_card_black_24dp.svg" alt="" class='grayscale' /></div>
                </div>
                <div class="body">
                    NCZI: ANNA SLOUKOVA Ing, 1965, COVID-19 PASS: D41-290-122, Typ: PCR, odber zo dna 4.12.2021 je NEGATIVNY. V pripade zmeny zdravotneho stavu volajte vseobecneho lekara.
                </div>
            </div>

            <!-- <div class="message justify-self-start">
                <div class='grid gap-2 col-2 auto justify-content-start time'>
                    <div><img src="@/assets/img/sim_card_black_24dp.svg" alt="" class='grayscale' /></div>
                    <div>6.11. 9:14</div>
                </div>
                <div class="body">
                    NCZI: ANNA SLOUKOVA Ing, 1965, COVID-19 PASS: D41-290-122, Typ: PCR, odber zo dna 7.11.2021 je NEGATIVNY. V pripade zmeny zdravotneho stavu volajte vseobecneho lekara.
                </div>
            </div> -->
        </div>

        <div class='write absolute p20'>
            <div class="grid gap-10">
                <div class="plus grid align-items-center justify-items-center justify-self-start align-self-end"><img src="@/assets/img/add_black_24dp.svg" alt="" /></div>
                <div contenteditable="true" class='input justify-self-stretch'>Textová správa</div>
                <div class="send grid align-items-center justify-items-center justify-self-end align-self-end"><img src="@/assets/img/arrow_upward_black_24dp.svg" alt="" /></div>
            </div>
        </div>

    </div>
</template>

<script>
export default {

    // props: ['domainList'],
    data() {
        return {
        }
    },
    methods: {
    }
}
</script>

<style scoped>

#sms {
    font-family: 'Roboto', sans-serif;
    font-size: 16px;
    padding: 21px;
    min-height: 100vh;
}
.name {
    font-weight: 600;
    font-size: 18px;
}
.message {
    max-width: 90%;
}
.message .time {
    font-size: 14px;
    color: #797979;
}
.message img {
    height: 12px;
}

.message .body {
    padding: 20px;
    border-radius: 20px;
    background-color: #F6F6F6;
}

.write {
    bottom: 0px;
    left: 0px;
    min-width: 100vw;
}
.write > div {
    grid-template-columns: 40px 1fr 40px
}
.plus {
    background-color: #F3F3F3;
    /* max-width: 75px; */
    /* max-height: 75px; */
    border-radius: 75px;
    padding: 10px;
}
.plus img {
    height: 18px;
}

.input {
    background-color: #F1F1F1;
    padding: 21px;
    border-radius: 20px;
}
.send {
    background-color: #F3F3F3;
    /* max-width: 75px; */
    /* max-height: 75px; */
    border-radius: 75px;
    padding: 10px;
}
.send img {
    height: 18px;
}
</style>
