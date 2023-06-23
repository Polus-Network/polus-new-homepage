<template>
<div style="background: rgba(255, 255, 255, 0.04); background-attachment: fixed; background-position: center; background-size: cover;" class="min-h-screen overflow-y-hidden gradient-animation relative ">
    <div style="border-radius: 536px;
opacity: 0.4000000059604645;
background: #F03383;
filter: blur(310.5px); width: 536px;
height: 510px;" class="absolute"></div>

    <div class="max-w-8xl mx-auto text-center">
        <div class="section">
            <div class="md:h-screen">
                <div class="max-w-3xl mx-auto pt-12 md:pt-36 text-center space-y-4" data-aos="fade-down" data-aos-anchor-placement="center-bottom" data-aos-duration="1000">
                    <h1 class="font-bold text-3xl text-white">How it works?</h1>
                    <p class="text-gray-200 text-sm">Become a Shareholder of Polus AI and Unlock Your Potential with PLS
                        Tokens! Introducing Polus Network's revolutionary investment ecosystem where you can invest in
                        the future of AI and earn rewards like never before. With our PLS token, built on the BEP-20
                        chain, you have the unique opportunity to become a shareholder of Polus AI, the driving force
                        behind groundbreaking advancements in artificial intelligence.</p>
                </div>
                <div class="grid grid-cols-1 md:grid-cols-2 max-w-8xl mx-auto text-center items-center justify-center lg:justify-between px-4 py-12 md:h-screen" data-aos="fade-up" data-aos-anchor-placement="center-bottom">
                    <div class="md:order-2 md:pl-24">
                        <img :src="AIImage" alt="">
                    </div>
                    <div class="max-w-lg mx-auto my-12 md:my-2 text-start space-y-4 md:order-1">
                        <h1 class="font-bold text-3xl text-white">Acquire PLS Tokens</h1>
                        <p class="text-gray-200 text-sm">Get started by acquiring PLS tokens through our secure and
                            user-friendly platform. As the primary token of Polus Network, PLS represents your ownership
                            stake in Polus AI, allowing you to directly participate in the success and growth of the
                            company. The acquisition of PLS tokens is your gateway to unlocking the full potential of
                            our investment ecosystem.</p>
                    </div>
                </div>
            </div>
        </div>
        <div class="section relative overflow-x-hidden" data-aos="zoom-in-up" data-aos-anchor-placement="center-bottom" data-aos-duration="1000">
            <div class="grid grid-cols-1 md:grid-cols-2 items-center justify-center lg:justify-between px-4 py-12 md:h-screen">
                <div class="md:order-2 md:pl-24">
                    <img :src="PLSImage" alt="">
                </div>
                <div class="max-w-lg mx-auto my-12 md:my-2 text-start space-y-4 md:order-1">
                    <h1 class="font-bold text-3xl text-white">Stake Your Shares</h1>
                    <p class="text-gray-200 text-sm">Once you hold PLS tokens, you can stake them in our carefully
                        crafted investing plans. By staking your portion of shares, you contribute to the development
                        and expansion of Polus AI's AI projects. Your participation fuels our innovative endeavors,
                        propelling the growth of AI technology and driving tangible impact across various industries.
                    </p>
                </div>
            </div>
            <div style="border-radius: 536px;
opacity: 0.4000000059604645;
background: #F03383;
filter: blur(300.5px); width: 236px;
height: 210px;" class="absolute  top-80"></div>
        </div>
        <div class="section relative overflow-x-hidden" data-aos="fade-up" data-aos-anchor-placement="center-bottom" data-aos-duration="1000">
            <div class="grid grid-cols-1 md:grid-cols-2 items-center justify-center lg:justify-between px-4 py-12 md:h-screen">
                <div class="md:order-2 md:pl-24">
                    <img :src="ReapBenifits" alt="">
                </div>
                <div style="border-radius: 434px;
background: #372AF8;
filter: blur(292.5px); width: 234px;
height: 246px;
flex-shrink: 0;" class="absolute  top-80"></div>
                <div class="max-w-lg mx-auto my-12 md:my-2 text-start space-y-4 md:order-1">
                    <h1 class="font-bold text-3xl text-white">Earn BRAIN Tokens</h1>
                    <p class="text-gray-200 text-sm">As a valued shareholder, you are entitled to rewards for your
                        contribution. By staking your PLS tokens, you earn rewards in the form of our native BRAIN
                        tokens. These rewards reflect the success and profitability of Polus AI's projects, allowing you
                        to benefit directly from the advancements and breakthroughs achieved by our talented team of AI
                        experts.</p>
                </div>
            </div>
        </div>
        <div class="section" data-aos="zoom-in-up   " data-aos-anchor-placement="center-bottom" data-aos-duration="1000">
            <div class="grid grid-cols-1 md:grid-cols-2 items-center justify-center lg:justify-between px-4 py-12 md:h-screen">
                <div class="md:order-2 md:pl-24">
                    <img :src="BrainImage" alt="">
                </div>
                <div style="border-radius: 366px;
opacity: 0.699999988079071;
background: #F03383;
filter: blur(234.5px); width: 266px;
height: 292px;
flex-shrink: 0;" class="absolute"></div>
                <div class="max-w-lg mx-auto my-12 md:my-2 text-start space-y-4 md:order-1">
                    <h1 class="font-bold text-3xl text-white">Stake Your Shares</h1>
                    <p class="text-gray-200 text-sm">Once you hold PLS tokens, you can stake them in our carefully
                        crafted investing plans. By staking your portion of shares, you contribute to the development
                        and expansion of Polus AI's AI projects. Your participation fuels our innovative endeavors,
                        propelling the growth of AI technology and driving tangible impact across various industries.
                    </p>
                </div>
            </div>
        </div>
    </div>
</div>
</template>

<script setup>
import AIImage from '../assets/Frame45.svg';
import PLSImage from '../assets/Frame51.svg';
import BrainImage from '../assets/Frame60.svg';
import ReapBenifits from '../assets/Frame55.svg';
</script>
