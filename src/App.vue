<template>
    <Header/>

    <main class="royalty">
        <section class="welcome" :class="{'has-animation': welcomeContAnimate}" data-motion="1">
            <svg class="welcome-img" width="631" height="494" viewBox="0 0 631 494" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M407.697 180.133C375.895 166.022 311.583 -12.4842 289.674 9.38802C267.766 31.2603 235.256 180.133 214.761 180.133C194.267 180.133 -2.20279 127.216 8.39807 145.561C18.9989 163.905 173.771 282.438 173.065 309.955C172.358 337.472 106.633 484.228 127.128 484.228C147.623 484.228 284.02 357.228 311.583 358.639C339.145 360.05 508.759 500.456 522.186 484.228C535.614 468 447.274 329.711 455.754 309.955C464.235 290.2 646.57 145.561 620.421 145.561C594.272 145.561 439.5 194.244 407.697 180.133Z" stroke="#82FF8E" stroke-width="15" stroke-linecap="round"/>
            </svg>
            <div class="wrapper">
                <h1 class="welcome-title to-left">Empowering Every Creator Connecting Every Fan</h1>
                <div class="welcome-main">
                    <div class="welcome-main-body to-top">
                        <p class="welcome-main-body-text">With Royalty, content creators can turn ad revenue into digital tokens, giving fans the opportunity to directly support and invest in their favorite creators.</p>
                        <a href="#" class="welcome-main-body-link">Connect Wallet</a>
                    </div>
                    <div class="card-group">
                        <Card v-for="card in cards" :key="card.title" :card="card"/>
                    </div>
                </div>
            </div>
        </section>

        <div class="double-cont" :data-motion="5">
            <svg class="double-cont-img" width="938" height="1118" viewBox="0 0 938 1118" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M496.66 25.769C520.653 59.8775 545.379 92.9276 569.489 126.867C666.68 263.681 759.318 405.268 846.087 555.602C869.76 596.617 891.181 638.825 911.217 682.931C914.988 691.233 913.803 691.964 907.484 685.748C870.872 649.737 834.684 613.194 797.355 579.148C649.877 444.642 497.96 330.151 341.735 237.269C305.196 215.546 267.288 200.405 231.014 177.775C221.642 171.928 246.107 199.629 254 209.995C295.817 264.914 338.472 318.304 380.594 372.676C466.963 484.162 547.419 606.476 626.395 728.882C644.522 756.977 672.282 792.46 684.714 826.785C686.753 832.414 682.013 828.526 680.073 827.093C652.438 806.687 625.295 782.687 597.969 761.002C420.165 619.9 241.242 495.598 57.4911 389.792C55.586 388.695 20.3811 364.549 25.2431 375.742C35.0588 398.34 53.0392 417.882 65.9877 436.371C113.359 504.013 158.144 575.576 202.536 647.154C271.248 757.95 335.503 873.167 401.612 986.832C422.83 1023.31 445.039 1058.76 468.963 1091.55" stroke="#F4F4F4" stroke-width="50" stroke-linecap="round"/>
            </svg>

            <section class="earn" data-motion="2">
                <div class="wrapper">
                    <h2 class="earn-title to-top">Everyone can earn in the
                        <span class="text-bg">
                        <svg class="text-bg-img" width="" height="68" viewBox="0 0 486 68" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M30.9844 37.1671C83.2288 37.1671 135.549 38.198 187.78 36.8C248.399 35.1775 309.032 31.2523 369.64 30.559C389.689 30.3296 409.652 31.6916 429.546 32.211C438.371 32.4414 447.294 35.5151 455.984 35.5151" stroke="#82FF8E" stroke-width="60" stroke-linecap="round"/>
                        </svg>
                        new creator
                    </span>
                        economy
                    </h2>
                    <p class="earn-description to-top">Trade tokens on Royalty’s open marketplace platform with ease!</p>
                </div>
                <div class="earn-coin-cont">
                    <img
                        v-for="coin in 10"
                        :key="'coin' + coin"
                        class="earn-coin"
                        src="./assets/img/earn-coin.png"
                        alt="coin"
                        width="150"
                        height="300">
                </div>
            </section>

            <section class="creators" data-motion="3">
                <svg class="creators-img" width="289" height="278" viewBox="0 0 289 278" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M48.5167 7.75179C120.444 15.5638 112.069 157.179 112.069 157.179C112.069 157.179 248.064 98.949 278.834 155.208C309.604 211.467 50.6347 285.734 42.0719 266.51C7.60466 189.13 -16.0714 0.736847 48.5167 7.75179Z" stroke="#82FF8E" stroke-width="15" stroke-linecap="round"/>
                </svg>
                <div class="wrapper">
                    <div class="card-group">
                        <CardLg v-for="card in cardsLg" :key="card.title" :card="card"/>
                    </div>
                </div>
            </section>
        </div>


        <section class="experts" data-motion="4">
            <div class="wrapper">
                <h3 class="experts-title to-top">Created by experts in
                    <span class="text-bg">
                        <svg class="text-bg-img" width="" height="67" viewBox="0 0 333 67" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M30.9844 36.6339C64.4208 36.6339 97.9057 37.6648 131.334 36.2668C170.13 34.6443 208.935 30.7191 247.724 30.0258C260.555 29.7964 273.332 31.1584 286.064 31.6778C291.712 31.9082 297.422 34.9819 302.984 34.9819" stroke="#82FF8E" stroke-width="60" stroke-linecap="round"/>
                        </svg>
                        Youtube
                    </span>
                </h3>
                <p class="experts-description to-top">Royalty is the blockchain branch of AIR Media-Tech, one the world’s largest creator ecosystems. AIR Media-Tech is dedicated to increasing the reach and revenue of digital content creators across the world.</p>
            </div>

            <div class="experts-line-cont">
                <div class="experts-line">
                    <div class="experts-line-item">
                        <img src="./assets/img/experts-3.jpg" alt="Partner image" class="experts-line-item-img" width="193" height="132">
                        <div class="experts-line-item-main">
                            <p class="experts-line-item-main-title">12 years</p>
                            <p class="experts-line-item-main-description">Of empowering content creators</p>
                        </div>
                    </div>
                    <div class="experts-line-item">
                        <img src="./assets/img/experts-2.jpg" alt="Partner image" class="experts-line-item-img" width="193" height="132">
                        <div class="experts-line-item-main">
                            <p class="experts-line-item-main-title">1 trillion</p>
                            <p class="experts-line-item-main-description">Total views</p>
                        </div>
                    </div>
                    <div class="experts-line-item">
                        <img src="./assets/img/experts-1.jpg" alt="Partner image" class="experts-line-item-img" width="193" height="132">
                        <div class="experts-line-item-main">
                            <p class="experts-line-item-main-title">3,000+</p>
                            <p class="experts-line-item-main-description">Partner channels</p>
                        </div>
                    </div>
                    <div class="experts-line-item">
                        <img src="./assets/img/experts-3.jpg" alt="Partner image" class="experts-line-item-img" width="193" height="132">
                        <div class="experts-line-item-main">
                            <p class="experts-line-item-main-title">12 years</p>
                            <p class="experts-line-item-main-description">Of empowering content creators</p>
                        </div>
                    </div>
                    <div class="experts-line-item">
                        <img src="./assets/img/experts-2.jpg" alt="Partner image" class="experts-line-item-img" width="193" height="132">
                        <div class="experts-line-item-main">
                            <p class="experts-line-item-main-title">1 trillion</p>
                            <p class="experts-line-item-main-description">Total views</p>
                        </div>
                    </div>
                    <div class="experts-line-item">
                        <img src="./assets/img/experts-1.jpg" alt="Partner image" class="experts-line-item-img" width="193" height="132">
                        <div class="experts-line-item-main">
                            <p class="experts-line-item-main-title">3,000+</p>
                            <p class="experts-line-item-main-description">Partner channels</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </main>
</template>

<script setup>
import Header from './components/Header.vue'
import Card from './components/Card.vue'
import CardLg from './components/CardLg.vue'
import {onMounted, onUnmounted, reactive, ref} from 'vue';

const welcomeContAnimate = ref(false);

const motionState = reactive({ motionSections: null });

const handleMotionScroll = () => {
    motionState.motionSections = document.querySelectorAll("[data-motion]");

    motionState.motionSections.forEach((motion) => {
        const top = motion.getBoundingClientRect().top;

        if (top < window.innerHeight - 200) motion.classList.add("has-animation");
    });
};

onMounted(() => {
    handleMotionScroll();

    window.addEventListener("scroll", handleMotionScroll);
});

onUnmounted(() => {
    window.removeEventListener("scroll", handleMotionScroll);
});

const cards = reactive([
    {
        title: 'Monatik',
        subs: '1 Mil subscribers',
        marketPrice: '1,4 RC',
        time: '1Y : 2M : 3H',
        imgUrl: 'src/assets/img/card1-bg.jpg',
    },
    {
        title: 'Diana Show',
        subs: '1 Mil subscribers',
        marketPrice: '1,4 RC',
        time: '1Y : 2M : 3H',
        imgUrl: 'src/assets/img/card2-bg.jpg',
    },
    {
        title: 'Anna Trincher ',
        subs: '1 Mil subscribers',
        marketPrice: '1,4 RC',
        time: '1Y : 2M : 3H',
        imgUrl: 'src/assets/img/card3-bg.jpg',
    }
])

const cardsLg = reactive([
    {
        title: 'Creators',
        description: 'Creators earn through token sales, engaging with existing fans and drawing in new supporters.',
        imgUrl: 'src/assets/img/card1-lg-bg.jpg',
    },
    {
        title: 'Fans',
        description: 'Fans receive regular payments for holding their tokens. Payments are drawn from ad revenue of their favorite social media creators.',
        imgUrl: 'src/assets/img/card2-lg-bg.jpg',
    }
])

</script>
