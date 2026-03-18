<template>
    <header class="sticky top-0 z-50 bg-[#190430]">
        <nav class="flex justify-center items-center gap-5 h-16 px-[200px] text-white">
        <div class="flex gap-9">
            <a href="#home" @click.prevent="scrollTo('home')"
            :class="{ 'glow-text': activeSection === 'home' }">Home</a>
            <a href="#about" @click.prevent="scrollTo('about')"
            :class="{ 'glow-text': activeSection === 'about' }">About</a>
            <a href="#skills" @click.prevent="scrollTo('skills')"
            :class="{ 'glow-text': activeSection === 'skills' }">Skills</a>
            <a href="#projects" @click.prevent="scrollTo('projects')"
            :class="{ 'glow-text': activeSection === 'projects' }">Projects</a>
        </div>
        </nav>
    </header>

    <section id="home" class="relative bg-[url('/test2(1).jpg')] bg-cover bg-center">
        <div id="hero-container"
            class="relative flex justify-center items-center lg:gap-[100px] lg:py-10 lg:px-10 lg:h-[600px]
                    md:gap-[50px] md:pt-6 md:pb-6 md:h-[500px]
                    sm:gap-[50px] sm:pt-6 sm:pb-6 sm:h-[500px]">

        <div class="relative flex flex-col items-center md:items-center lg:items-start">
            <!-- Pulsating Glow 
            <div class="absolute top-1/2 left-1/2 lg:w-[280px] lg:h-[280px] md:h-[180px] md:w-[180px] -translate-x-1/2 -translate-y-1/2 
            bg-[#a35cf0] rounded-xl blur-xl opacity-90"></div> -->

            <!-- Image on top -->
            <img src="/test4.jpg" alt="My Photo"
                class="relative lg:h-[300px] lg:w-[300px] md:h-[200px] md:w-[200px] sm:h-[150px] sm:w-[150px] rounded-xl fade-in-image">
        </div>

        <div class="flex flex-col">

            <div class="relative flex flex-col m-0 text-container opacity-0">
                <h1 class="lg:text-[60px] md:text-[30px] sm:text-[30px] font-bold text-white leading-[1.1] glowing-text">
                HELLO THERE! 
                </h1>
            </div>

            <div class="relative flex flex-col m-0 text-container1 opacity-0">
                <span class="block lg:text-[20px] md:text-[10px] sm:text-[10px] text-white mt-2 leading-[1]">I'm Aljubehr Sahiol, I build digital experiences</span>
            </div>

        </div>
        </div>
    </section>

    <section id="about" class="flex flex-col items-center bg-gradient-to-b from-[#1a0433] to-[#280D66] pb-32 text-white">
        <!-- Centered heading -->
        <h2 class="font-bold text-3xl md:text-2xl lg:text-4xl text-center text-white mt-16 mb-12 glowing-text">
            ABOUT ME
        </h2>

        <!-- Card -->
        <div class="bg-[#7c17e8] max-w-5xl lg:p-16 md:p-10 sm:p-12 sm:m-5 text-center text-white rounded-2xl">
            <div class="flex items-center gap-6">
            <p class="lg:text-lg md:text-md sm:text-sm flex-1 text-justify">
                Hi, I’m Aljubehr Banguis Sahiol. I create digital experiences that people enjoy, whether it’s 
                building websites and apps, designing clean interfaces, or sharing ideas through videos. I’m passionate about 
                turning concepts into real, usable solutions that make life easier or more enjoyable.
            </p>

            <img src="/logo12.png" alt="My Photo" class="sm:h-[150px] sm:w-[150px] md:h-[150px] md:w-[150px] lg:h-[300px] lg:w-[300px] rounded-xl">

            <p class="lg:text-lg md:text-md sm:text-sm flex-1 text-justify">
                I love exploring new technologies, experimenting with creative formats, and finding ways to combine functionality 
                and creativity in everything I do. I’m always looking for new challenges that help me grow and improve my skills.
            </p>
            </div>
        </div>
    </section>

    <section id="skills" class="pt-40 pb-40 bg-[#280D66] flex justify-center">
        <div class="max-w-6xl w-full px-6 text-white">

        <!-- Title -->
        <h2 class="text-3xl lg:text-4xl font-bold text-center mb-12 glowing-text">
            MY SKILLS
        </h2>

        <!-- Skills Grid -->
        <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-5 gap-6">

            <div class="relative group w-full h-40 bg-[#7c16e9] rounded-2xl overflow-hidden flex items-center justify-center">
                <img src="/test-html.jpeg" alt="HTML" class="absolute inset-0 w-full h-full object-cover opacity-0 group-hover:opacity-100 transition-opacity duration-300"/>
                <div class="absolute inset-0 bg-[#0c0217]/80 opacity-0 group-hover:opacity-80 transition-opacity duration-300"></div>
                <span class="z-10 text-lg font-semibold transition-all duration-300 group-hover:text-white">
                    HTML
                </span>
            </div>

            <div class="relative group w-full h-40 bg-[#7c16e9] rounded-2xl overflow-hidden flex items-center justify-center">
                <img src="/test-css.jpeg" alt="CSS" class="absolute inset-0 w-full h-full object-cover opacity-0 group-hover:opacity-100 transition-opacity duration-300"/>
                <div class="absolute inset-0 bg-[#0c0217]/80 opacity-0 group-hover:opacity-80 transition-opacity duration-300"></div>
                <span class="z-10 text-lg font-semibold transition-all duration-300 group-hover:text-white">
                    CSS
                </span>
            </div>

            <div class="relative group w-full h-40 bg-[#7c16e9] rounded-2xl overflow-hidden flex items-center justify-center">
                <img src="/test-javas.jpg" alt="CSS" class="absolute inset-0 w-full h-full object-cover opacity-0 group-hover:opacity-100 transition-opacity duration-300"/>
                <div class="absolute inset-0 bg-[#0c0217]/80 opacity-0 group-hover:opacity-80 transition-opacity duration-300"></div>
                <span class="z-10 text-lg font-semibold transition-all duration-300 group-hover:text-white">
                    JAVASCRIPT
                </span>
            </div>

            <div class="relative group w-full h-40 bg-[#7c16e9] rounded-2xl overflow-hidden flex items-center justify-center">
                <img src="/test-php.jpeg" alt="CSS" class="absolute inset-0 w-full h-full object-cover opacity-0 group-hover:opacity-100 transition-opacity duration-300"/>
                <div class="absolute inset-0 bg-[#0c0217]/80 opacity-0 group-hover:opacity-80 transition-opacity duration-300"></div>
                <span class="z-10 text-lg font-semibold transition-all duration-300 group-hover:text-white">
                    PHP
                </span>
            </div>

            <div class="relative group w-full h-40 bg-[#7c16e9] rounded-2xl overflow-hidden flex items-center justify-center">
                <img src="/test-videdi.jpg" alt="CSS" class="absolute inset-0 w-full h-full object-cover opacity-0 group-hover:opacity-100 transition-opacity duration-300"/>
                <div class="absolute inset-0 bg-[#0c0217]/80 opacity-0 group-hover:opacity-80 transition-opacity duration-300"></div>
                <span class="z-10 text-lg font-semibold transition-all duration-300 group-hover:text-white">
                    VIDEO EDITING
                </span>
            </div>

        </div>
        </div>
    </section>

    <section id="projects" class="flex flex-col items-center justify-center pt-24 pb-80 text-white bg-gradient-to-b from-[#280D66] to-[#1a0433]">
        
        <h2 class="text-3xl lg:text-4xl font-bold text-center glowing-text mb-14">
        MY PROJECTS
        </h2>

        <!-- Projects Container -->
        <div class="max-w-7xl w-full px-[100px] grid md:grid-cols lg:grid-cols-2 gap-10">

            <!-- Project Card -->
            <div class="group relative rounded-xl overflow-hidden shadow-lg">
                
                <img 
                src="/portfolio.jpg"
                class="w-full h-64 object-cover transition-transform duration-500 group-hover:scale-110"
                />

                <!-- Overlay -->
                <div class="absolute inset-0 bg-[#0c0217]/80 backdrop-blur-lg opacity-0 
                            group-hover:opacity-100 transition duration-500 
                            flex flex-col justify-center items-center text-center p-6">
                
                <h3 class="text-xl font-semibold mb-2">
                    Portfolio Website
                </h3>

                <p class="text-sm mb-4">
                    Personal portfolio built with Nuxt and Tailwind.
                </p>

                <div class="flex gap-4">
                    <a href="#" class="px-4 py-2 bg-purple-600 rounded-lg hover:bg-purple-700">
                    Code
                    </a>
                </div>

                </div>
            </div>

            <!-- Project Card -->
            <div class="group relative rounded-xl overflow-hidden shadow-lg">
                
                <img 
                src="/irecipe.jpg"
                class="w-full h-64 object-cover transition-transform duration-500 group-hover:scale-110"
                />

                <!-- Overlay -->
                <div class="absolute inset-0 bg-[#0c0217]/80 backdrop-blur-lg opacity-0 
                            group-hover:opacity-100 transition duration-500 
                            flex flex-col justify-center items-center text-center p-6">
                
                <h3 class="text-xl font-semibold mb-2">
                    Irecipe
                </h3>

                <p class="text-sm mb-4">
                    Full stack recipe web built with JavaScript, PHP, and MySQL.
                </p>

                <div class="flex gap-4">
                    <a href="https://github.com/zrephy08/Irecipe" class="px-4 py-2 bg-purple-600 rounded-lg hover:bg-purple-700">
                    Code
                    </a>
                </div>

                </div>
            </div>

            <!-- Project Card -->
            <div class="group relative rounded-xl overflow-hidden shadow-lg">
                
                <img 
                src="/soapstock.jpg"
                class="w-full h-64 object-cover transition-transform duration-500 group-hover:scale-110"
                />

                <!-- Overlay -->
                <div class="absolute inset-0 bg-[#0c0217]/80 backdrop-blur-lg opacity-0 
                            group-hover:opacity-100 transition duration-500 
                            flex flex-col justify-center items-center text-center p-6">
                
                <h3 class="text-xl font-semibold mb-2">
                    Soapstock
                </h3>

                <p class="text-sm mb-4">
                    Full stack laundromat web stock inventory built with JavaScript, PHP, and MySQL.
                </p>

                <div class="flex gap-4">
                    <a href="https://github.com/zrephy08/soapstock" class="px-4 py-2 bg-purple-600 rounded-lg hover:bg-purple-700">
                    Code
                    </a>
                </div>

                </div>
            </div>

                    <!-- Project Card -->
            <div class="group relative rounded-xl overflow-hidden shadow-lg">
                
                <img 
                src="/youtube1.jpg"
                class="w-full h-64 object-cover transition-transform duration-500 group-hover:scale-110"
                />

                <!-- Overlay -->
                <div class="absolute inset-0 bg-[#0c0217]/80 backdrop-blur-lg opacity-0 
                            group-hover:opacity-100 transition duration-500 
                            flex flex-col justify-center items-center text-center p-6">
                
                <h3 class="text-xl font-semibold mb-2">
                    Zrephy
                </h3>

                <p class="text-sm mb-4">
                    Youtube channel where I record videos about games.
                </p>

                <div class="flex gap-4">
                    <a href="https://www.youtube.com/@Zrephy068" class="px-4 py-2 bg-purple-600 rounded-lg hover:bg-purple-700">
                    Link
                    </a>
                </div>

                </div>
            </div>

        </div>

    </section>

    <footer class="bg-[#0c0217] text-white py-10 flex justify-center">
        
        <div class="max-w-6xl w-full px-6 text-center">

        <!-- Logo / Name -->
        <h3 class="text-xl font-semibold mb-4">
            Aljubehr Sahiol
        </h3>

        <!-- Social Links -->
        <div class="flex justify-center gap-6 mb-6">
            <a href="https://github.com/zrephy08" class="hover:text-purple-400 transition">GitHub</a>
            <a href="mailto:aljubehr01@gmail.com" class="hover:text-purple-400 transition">Email</a>
        </div>

        <!-- Divider -->
        <div class="border-t border-purple-900 my-6"></div>

        <!-- Copyright -->
        <p class="text-sm text-gray-400">
            © 2026 Aljubehr Sahiol. All rights reserved.
        </p>

        </div>

    </footer>

</template>

<script setup>
import { ref, onMounted, onUnmounted } from 'vue'

const activeSection = ref('home')

// Handle scroll to highlight links dynamically
const sections = ['home', 'about', 'skills', 'projects']

const handleScroll = () => {
    const scrollY = window.scrollY + 100 // offset for navbar
    let found = 'home'

    for (const sec of sections) {
        const el = document.getElementById(sec)
        if (el && scrollY >= el.offsetTop) {
        found = sec
        }
    }

    activeSection.value = found
}

// Smooth scroll function
const scrollTo = (id) => {
    const el = document.getElementById(id)
    if (el) {
        const navHeight = document.querySelector('header').offsetHeight
        const top = window.scrollY + el.getBoundingClientRect().top - navHeight

        window.scrollTo({
        top,
        behavior: 'smooth',
        })
    }
}

onMounted(() => {
  window.addEventListener('scroll', handleScroll)
})

onMounted(() => {
  // Remove hash if page loads with it
  if (window.location.hash) {
    history.replaceState(null, '', ' ')
  }
})

onUnmounted(() => {
  window.removeEventListener('scroll', handleScroll)
})
</script>

<style scoped>
    /* Glow pulsating animation */
    @keyframes pulseGlow {
    0%, 100% {
        transform: translate(-50%, -50%) scale(0.8);
        opacity: 0.7;
    }
    50% {
        transform: translate(-50%, -50%) scale(1);
        opacity: 1;
    }
    }
    .glow-pulse {
    animation: pulseGlow 5s ease-in-out infinite;
    }

    @keyframes textPulseGlow {
    0%, 100% {
        text-shadow: 0 0 4px #a35cf0, 0 0 8px #a35cf0, 0 0 12px #a35cf0;
        color: #ffffff;
    }
    50% {
        text-shadow: 0 0 5px #a35cf0, 0 0 15px #a35cf0, 0 0 20px #a35cf0;
        color: #ffffff;
    }
    }

    /* Delayed start for the glow */
    .delayed-glow {
    animation-delay: 3s; /* wait until both texts are done */
    animation-fill-mode: backwards; /* ensures it starts after delay */
    }

    /* Simple fade-in for image */
    @keyframes fadeIn {
    0% { opacity: 0; }
    100% { opacity: 1; }
    }
    .fade-in-image {
    opacity: 0;
    animation: fadeIn 1.5s ease-out forwards;
    }

    /* Text animation: fade-in after image */
    @keyframes textFadeIn {
    0% { opacity: 0; transform: translateX(50px); }
    100% { opacity: 1; transform: translateX(0); }
    }
    .text-container {
    animation: textFadeIn 1s ease-out 1s forwards;
    }
    .text-container1 {
    animation: textFadeIn 1s ease-out 2s forwards;
    }

    .glowing-text {
    animation: textPulseGlow 3s ease-in-out infinite;
    }
    /* Static glow for active nav link */
    .glow-text {
        text-shadow: 0 0 12px #a35cf0, 0 0 16px #a35cf0;
        color: #ffffff;
        transition: text-shadow ease;
    }
</style>