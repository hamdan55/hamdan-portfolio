<template>
    <section class="w-full flex flex-wrap justify-center items-center mt-24 lg:mt-0 container-spx py-16 md:py-20 lg:py-24" id="experience">
        <div class="flex flex-wrap justify-start items-center cursor-default">
            <h2 v-scroll-reveal="{ delay: 100, mobile: true, origin: 'bottom', easing: 'cubic-bezier(0.5, 0, 0, 1)', distance: '80px'}" class="w-full text-gray-700 text-3xl md:text-4xl font-semibold leading-tight text-center mb-12">
                My Experience
            </h2>
            <div class="w-full h-full flex flex-wrap">
                <div class="w-full max-w-7xl flex flex-wrap justify-center items-stretch mx-auto">
                    <div class="my-4 p-3 w-full md:w-1/2 lg:w-1/3 flex flex-wrap justify-between items-stretch select-none" v-scroll-reveal="{ delay: 400, mobile: true, origin: 'bottom', easing: 'cubic-bezier(0.5, 0, 0, 1)', distance: '80px'}">
                        <div class="bg-white shadow-lg rounded-lg p-6">
                            <div class="w-full flex flex-wrap flex-col items-start justify-center">
                                <p class="text-xl font-secondary text-gray-800">Senior Full Stack Engineer</p>
                                <p class="text-lg text-blue-500">Septem Systems PVT Limited</p>
                                <p class="text-base font-secondary text-gray-500 font-mono mt-3">Dec 2021 - Present</p>
                            </div>
                            <ul class="text-gray-800 pt-6 list-disc pl-4 text-base font-light">
                              <li>
                                Accomplished Senior Full Stack Engineer with over 2 years of experience in developing and delivering robust software solutions.
                              </li>
                              <li>
                                Proficient in both front-end and back-end technologies, leveraging a comprehensive skill set to drive successful project outcomes.
                              </li>
                              <li>
                                Strong expertise in designing and implementing scalable architectures, optimizing performance, and ensuring code quality.
                              </li>
                              <li>
                                Proven track record of leading cross-functional teams and collaborating effectively with stakeholders to achieve project objectives.
                              </li>
                              <li>
                                Experienced in utilizing Agile methodologies to drive efficient development cycles and deliver high-quality software products.
                              </li>
                              <li>
                                Strong problem-solving and analytical skills, with a keen eye for detail and a passion for delivering exceptional user experiences                              </li>
                              <li>
                                Excellent communication and interpersonal abilities, fostering effective collaboration and teamwork.
                              </li>
                              <li>
                                Committed to delivering excellence and driving innovation through continuous learning and professional development.                              </li>
                              <li>
                                Consistently recognized for consistently delivering projects on time and within budget, exceeding client expectations.                 </li>           </ul>
                        </div>
                    </div>

                    <div class="my-4 p-3 w-full md:w-1/2 lg:w-1/3 flex flex-wrap justify-between items-stretch select-none" v-scroll-reveal="{ delay: 400, mobile: true, origin: 'bottom', easing: 'cubic-bezier(0.5, 0, 0, 1)', distance: '80px'}">
                        <div class="bg-white shadow-lg rounded-lg p-6">
                            <div class="w-full flex flex-wrap flex-col items-start justify-center">
                                <p class="text-xl font-secondary text-gray-800">FrontEnd Developer</p>
                                <p class="text-lg text-blue-500">TBox Solutions PVT Limited</p>
                                <p class="text-base font-secondary text-gray-500 font-mono mt-3">Jan 2021 - Jan 2022</p>
                            </div>
                            <ul class="text-gray-800 pt-6 list-disc pl-4 text-base font-light">
                                <li>Versatile FrontEnd Developer: Creating Engaging User Experiences.</li>
                                <li>Passionate FrontEnd Developer with Expertise in Modern Web Technologies.</li>
                                <li>Crafting Seamless User Interfaces: FrontEnd Development Specialist.</li>
                                <li>Driving Innovation through FrontEnd Excellence and Cutting-Edge Design.</li>
                                <li>Delivering High-Performance Web Solutions: FrontEnd Development Expert.</li>
                                <li>Mastering the Art of FrontEnd Development: Building Beautiful and Responsive Websites.
                                </li>
                                <li>Collaborative FrontEnd Developer: Bridging Design and Functionality for Seamless Web Experiences.</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
import { SlideXRightTransition } from 'vue2-transitions'

export default {
    components: {
        SlideXRightTransition,
    },
    data(){
        return{
            current_company: 0
        }
    },
    methods: {
        change_company(val){
            this.current_company = val;
        }
    },
}
</script>
<style lang="scss" scoped>
.w-26 {
    width: 6.5rem;
}

.text-nav {
 @apply z-20 text-center self-center text-gray-900 transition-all duration-300 ease-out text-base font-secondary tracking-wider py-2 px-3 rounded-md leading-4;
 width: 6.5rem;
    &:focus{
        @apply outline-none select-none bg-transparent;
        -webkit-tap-highlight-color: transparent;
    }

    &:hover {
        @apply text-gray-600;
    }
}

.btn-anim-1{
    transition: all 0.4s ease-in-out;
    @apply text-left items-center justify-center py-2;

    &:hover{
        background-color: rgba(99, 179, 237, 0.191);
    }
}

li{
    @apply mb-2.5;

    // &::before{
    //     content:'';
    //     @apply inline-flex w-2 h-0.5 bg-blue-600 absolute -left-4 top-3 transform;
    // }
}
</style>
