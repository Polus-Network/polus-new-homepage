<script setup>
import Navbar from './components/Header.vue'
import VideoEle from './components/Video.vue'
import videoimage from './assets/Rectangle 204.png';
import Fullpage from './components/Fullpage.vue'
import Wrapimage from './assets/Frame63.png';
import Accordianimage from './assets/Layer11.png';
import FooterLogo from './assets/Group.svg';

import {
    defineComponent,
    h
} from 'vue'
</script>

<template>
<div class="">
    <section>
        <Navbar />

        <!-- HERO SECTION -->

        <div class="max-w-3xl mx-auto py-14 px-4" data-aos="fade-down" data-aos-anchor-placement="center-bottom" data-aos-duration="1000">
            <div class="text-center space-y-4">
                <h1 class="text-white text-4xl md:text-7xl font-semibold">Earn Smarter with
                    <p class="gradient-text"><span class="text-transparent text-4xl md:text-7xl">AI Technology</span></p>
                </h1>
                <p class="font-xs text-gray-400 md:px-16">Imagine a world where you can invest in AI projects, support
                    cutting-edge innovations, and earn substantial returns. With Polus Network, this dream becomes a
                    reality.</p>
                <button class="bg-gray-50 px-6 py-2 rounded-3xl border text-gray-800">Get Started</button>
            </div>
        </div>
    </section>
                                                <!-- video section -->
    <section>
        <div class=" mt-12">
            <VideoEle />
        </div>

                                                <!-- text about us -->
        <div class="max-w-3xl mx-auto py-12 px-4  md:py-36 text-center space-y-4" data-aos="fade-up" data-aos-anchor-placement="center-bottom">
            <h1 class="font-bold text-3xl text-white">About us</h1>
            <p class=" text-gray-200 text-sm">Polus Network is brought to you by “Polus AI” built with the sole purpose
                of providing everyone an opportunity of investing in AI development and earn with it. At Polus Network,
                we believe that artificial intelligence (AI) holds immense potential to transform the world. Our mission
                is to make AI development accessible to all and provide a unique opportunity for individuals like you to
                be part of this technological revolution. World is getting advanced with every single day and u should
                too. So, with Polus Network came a solution for everyone to earn using AI. Our company is properly
                regulated and audited so you can invest in us with your ease of mind.</p>
        </div>

    </section>

                                                    <!-- FEATURE SECTION -->
    <section>
        <Fullpage />

    </section>
                                                    <!--    FAQs SECTION   -->
    <section>
        <div class="">
            <div style=" background: linear-gradient(90deg, #111827,#162951 ,#111827);" class="max-w-3xl mx-auto py-12 px-4 md:py-16 text-center space-y-4" data-aos="fade-up">
                <h1 class="font-bold text-3xl text-white">Why choose Polus Network?</h1>
                <p class=" text-gray-200 leading-7">As an investor in Polus Network, you become a shareholder of Polus AI, the
                    company driving the AI development. This unique feature allows you to participate in the success and
                    profitability of Polus AI's projects. By staking your shares and earning rewards, you can directly benefit
                    from the growth of the AI industry. Moreover, Polus Network offers a user-friendly and intuitive platform,
                    making it accessible for investors of all levels of experience. Whether you're a seasoned investor or new to
                    the world of AI, Polus Network provides a seamless and convenient investment experience.
                    By choosing Polus Network, you align yourself with a platform dedicated to AI investments, shareholder
                    benefits, user-friendly experience, community collaboration, and a commitment to trust and transparency.
                    Embrace the potential of AI and invest with confidence in Polus Network.</p>
            </div>
        </div>
    </section>
                                        <!-- ACCORDIAN SECTION -->
    <section>
        <div style="background: rgba(255, 255, 255, 0.04);" class="brightness-20 relative overflow-hidden">
            <div style="border-radius: 536px;
                                                opacity: 0.4000000059604645;
                                                background: #F03383;
                                                filter: blur(234.5px); width: 536px;
                                                height: 510px;" class="absolute"></div>

            <div class="max-w-7xl px-2 md:px-8 mx-auto rounded py-12 relative z-20">
                <div class="max-w-3xl mr-auto" id="accordion-collapse" data-accordion="collapse" data-aos="zoom-in-up" data-aos-anchor-placement="center-bottom" data-aos-duration="1000">
                                                <div style="
                            background: rgba(255, 255, 255, 0.04);
                            box-shadow: 0px 0px 14px 0px rgba(255, 255, 255, 0.09) inset;
                            backdrop-filter: blur(7.5px);" class="my-8 border-2 border-gray-600   z-50 p-2" :class="activeAccordion !== index ? 'rounded-full' : 'rounded-3xl'" v-for="(item, index) in accordionItems" :key="index">
                        <h2>
                            <button type="button" class="flex items-center  justify-between p-2 md:p-5 w-full font-medium text-left  border-b-0 text-white  rounded-xl" :class="{ 'rounded-b-xl': activeAccordion === index }" :data-accordion-target="`#accordion-collapse-body-${index + 1}`" :aria-expanded="activeAccordion === index" :aria-controls="`accordion-collapse-body-${index + 1}`" @click="toggleAccordion(index)">
                                <span>{{ item.title }}</span>
                                <svg data-accordion-icon class="w-6 h-6 shrink-0" :class="{ 'rotate-180': activeAccordion === index }" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
                                    <path fill-rule="evenodd" d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z" clip-rule="evenodd"></path>
                                </svg>
                            </button>
                        </h2>
                        <div class="mt-2" :id="`accordion-collapse-body-${index + 1}`" :class="activeAccordion !== index ? 'hidden rounded-md' : ''">
                            <div class="p-5  rounded-md">
                                <p class="mb-2 text-white ">{{ item.content }}</p>
                            </div>
                        </div>
                    </div>
                </div>

            </div>
            <div class="w-fit rounded-full">
                <img class="absolute top-20 right-60 z-0" :src="Accordianimage" alt="">
            </div>
        </div>
    </section>
                                                <!-- FOOTER -->
   

        <footer style=" background: linear-gradient(90deg, #111827);" class="py-8 sm:py-12 lg:py-16 px-4 relative overflow-hidden">
            <div class=" max-w-7xl  mx-auto">
                <div class="grid grid-cols-1 gap-8 md:grid-cols-2">
                    <div class="space-y-8">
                        <img class="" :src="FooterLogo" alt="">
                        <p class="text-3xl font-semibold text-white">Invest in AI, Invest in Future, Invest with Polus Network</p>
                    </div>
                    <div class="flex justify-start mt-16 sm:justify-end sm:mt-0">
                        <div class="space-y-8 sm:flex sm:flex-row sm:space-y-0 sm:space-x-8">
                            <div>
                                <h3 class="text-sm font-semibold leading-6 text-white"></h3>
                                <ul role="list" class="mt-6 space-y-4">
                                    <li v-for="item in navigation.solutions" :key="item.name">
                                        <a :href="item.href" class="leading-6 text-gray-300 hover:text-white">{{ item.name }}</a>
                                    </li>
                                </ul>
                            </div>
                            <div>
                                <h3 class="text-sm font-semibold leading-6 text-white"></h3>
                                <ul role="list" class="mt-6 space-y-4">
                                    <li v-for="item in navigation.support" :key="item.name">
                                        <a :href="item.href" class="leading-6 text-gray-300 hover:text-white">{{ item.name }}</a>
                                    </li>
                                </ul>
                            </div>

                        </div>

                    </div>

                </div>

            </div>
            <div class="pt-8 flex justify-between max-w-7xl mx-auto">
                <p class="text-sm leading-5 text-gray-200">&copy; Terms of Use . Privacy and Policy</p>
                <span class="text-sm leading-5 text-gray-200">Copyright © 2023 Its_Mirza</span>
            </div>
            <div style="border-radius: 12px;
                      background: linear-gradient(73deg, rgba(217, 100, 135, 0.57) 0%, #773CD0 13.02%, #3665DD 25%, #822EE0 36.46%, #DC21BE 48.96%, #D723E0 59.38%, #A51EE4 74.48%, #DE36D3 86.46%, rgba(233, 130, 55, 0.71) 100%);
                      filter: blur(50px);
                " class="h-12 w-full absolute -bottom-0 "></div>
        </footer>


</div>
</template>

<script>

document.addEventListener('DOMContentLoaded', function () {
  const textElement = document.querySelector('.gradient-text');

  textElement.classList.add('animate');

  textElement.addEventListener('animationend', function () {
    textElement.classList.remove('animate');
  });
});

const navigation = {
  solutions: [
    { name: 'About us', href: '#' },
    { name: 'How it works', href: '#' },
    { name: 'Why Choose PLS', href: '#' },
    { name: 'FAQs', href: '#' },
  ],
  support: [
    { name: 'Instagram', href: '#' },
    { name: 'Facebook', href: '#' },
    { name: 'LinkedIn', href: '#' },
    { name: 'Twitter', href: '#' },
  ],

}

// ----------------------------------------------------------------------
export default {
  data() {
    return {
      activeAccordion: null,
      accordionItems: [
        {
          title: '01.What is Artificial Intelligence?',
          content: 'Flowbite is an open-source library of interactive components built on top of Tailwind CSS including buttons, dropdowns, modals, navbars, and more.'
        },
        {
          title: '02.How to Invest on Polus Network?',
          content: 'Flowbite is first conceptualized and designed using the Figma software so everything you see in the library has a design equivalent in our Figma file.'
        },
        {
          title: '03.Why you should invest in Polus Network?',
          content: 'The main difference is that the core components from Flowbite are open source under the MIT license, whereas Tailwind UI is a paid product. Another difference is that Flowbite relies on smaller and standalone components, whereas Tailwind UI offers sections of pages.'
        },
        {
          title: '04.What do Polus Network offer?',
          content: 'The main difference is that the core components from Flowbite are open source under the MIT license, whereas Tailwind UI is a paid product. Another difference is that Flowbite relies on smaller and standalone components, whereas Tailwind UI offers sections of pages.'
        },
        {
          title: '05.Where is your investment used?',
          content: 'The main difference is that the core components from Flowbite are open source under the MIT license, whereas Tailwind UI is a paid product. Another difference is that Flowbite relies on smaller and standalone components, whereas Tailwind UI offers sections of pages.'
        },
        {
          title: '06.How to reach us out?',
          content: 'The main difference is that the core components from Flowbite are open source under the MIT license, whereas Tailwind UI is a paid product. Another difference is that Flowbite relies on smaller and standalone components, whereas Tailwind UI offers sections of pages.'
        }
      ]
    };
  },
  methods: {
    toggleAccordion(index) {
      if (this.activeAccordion === index) {
        this.activeAccordion = null;
      } else {
        this.activeAccordion = index;
      }
    }
  }
};
</script>

<style scoped>
.gradient-text {
    text-decoration: none;
    position: relative;
    border: none;
    font-size: 70px;
    font-family: inherit;
    color: #fff;
    line-height: 1em;
    text-align: center;
    background: linear-gradient(90deg, #F5C9E7, #6F66FF, #ffeb3b, #EEC07B);
    background-size: 300%;
    z-index: 1;
    background-clip: text;
}

.gradient-text.animate {
    animation: ani 15s 2; /* Added '2' to play the animation twice */
    border: none;
}

@keyframes ani {
    0% {
        background-position: 0%;
    }

    100% {
        background-position: 400%;
    }
}

</style>
