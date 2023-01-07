<template>
    <main class="relative bg-slate-800 pt-4 mb-80 max-h-screen">
        <header class="container flex flex-row mx-auto text-center justify-center px-6 xl:px-64">
            <div class="flex flex-col my-4">
                <div class="bg-amber-200 border-2 border-b-[1px] rounded-t-xl rounded-b border-gray-900 px-10 xl:px-36 h-2"></div>
                <div class="bg-amber-300 border-2 border-t-[1px] rounded-b-xl rounded-t border-gray-900 px-10 xl:px-36 h-2"></div>
            </div>
            <h1 class="text-slate-300 font-bold tracking-wider font-['Verdana'] pt-2 text-xl xl:text-2xl px-1.5 xl:px-0">HALLVARD A. WÆHLER</h1>
            <div class="flex flex-col my-4">
                <div class="bg-amber-200 border-2 border-b-[1px] rounded-t-xl rounded-b border-gray-900 px-10 xl:px-36 h-2"></div>
                <div class="bg-amber-300 border-2 border-t-[1px] rounded-b-xl rounded-t border-gray-900 px-10 xl:px-36 h-2"></div>
            </div>
        </header>
        <div class="container flex flex-col mx-auto px-4 xl:px-64">
            <section id="top" class="flex flex-col bg-slate-700">
                <div class="flex flex-row bg-slate-700 justify-between">
                    <div class="w-88 text-center pt-6">
                        <h2 class="text-slate-300 font-bold tracking-wider font-['Verdana'] justify-left text-left pl-6 text-xl xl:text-4xl">I am a bioinformatician and developer.</h2>
                    </div>
                    <div class="items-center justify-right">
                        <div class="bg-gray-900 border-2 border-gray-600 border-t-gray-900 border-l-gray-900 text-green-500 tracking-widest font-['Verdana'] text-lg xl:text-xl py-2 pl-1"><marquee>WELCOME TO MY HOMEPAGE</marquee></div>
                        <div class="text-left">
                            <button class="border-4 border-b-gray-500 border-x-gray-600 border-t-gray-200 rounded bg-gray-300 tracking-widest font-['Verdana'] text-sm xl:text-md p-1 pr-2 mt-2 active:border-l-gray-200 active:border-t-gray-500 active:border-b-0 active:border-t-6"><a href="https://github.com/hallvaaw" target="_blank" rel="noopener noreferrer">GITHUB</a></button>
                            <button class="border-4 border-b-gray-500 border-x-gray-600 border-t-gray-200 rounded bg-gray-300 tracking-widest font-['Verdana'] text-sm xl:text-md p-1 pr-2 mb-2 active:border-r-gray-200 active:border-t-gray-500 active:border-b-0 active:border-t-6"><a href="https://www.linkedin.com/in/hallvard-austin-wæhler/" target="blank_" rel="noopener noreferrer">LINKEDIN</a></button>
                        </div>
                    </div>
                </div>
                <div class="bg-slate-800 border-2 border-gray-600 border-t-gray-900 border-l-gray-900 h-8 mx-16 my-8"></div>
            </section>
            <section id="middle" class="bg-slate-700">
                <div v-if="CVComp == true">
                    <CVPage />
                </div>
                <div v-else>
                    <AboutPage />
                </div>
            </section>
        <div class="container flex flex-row border-y-2 border-x-4 border-x-slate-600 border-b-gray-600 border-t-gray-900 mx-auto text-center justify-center pb-2">
            <div class="flex flex-col my-4">
                <div class="bg-amber-200 border-2 border-b-[1px] rounded-t-xl rounded-b border-gray-900 px-[75px] xl:px-44 h-1.5"></div>
                <div class="bg-amber-300 border-2 border-t-[1px] rounded-b-xl rounded-t border-gray-900 px-[75px] xl:px-44 h-1.5"></div>
            </div>
            <h1 class="text-slate-300 font-bold tracking-wider font-['Verdana'] pt-2 text-lg xl:text-2xl">MORE THINGS</h1>
            <div class="flex flex-col my-4">
                <div class="bg-amber-200 border-2 border-b-[1px] rounded-t-xl rounded-b border-gray-900 px-[75px] xl:px-44 h-1.5"></div>
                <div class="bg-amber-300 border-2 border-t-[1px] rounded-b-xl rounded-t border-gray-900 px-[75px] xl:px-44 h-1.5"></div>
            </div>
        </div>
            <section id="bottom" class="flex flex-col bg-slate-800">
                <div class="bg-gray-900 border-2 border-x-4 border-gray-600 border-t-gray-900 border-l-gray-900 mb-6">
                    <div class="text-green-500 tracking-widest font-['Verdana'] pl-2 hover:cursor-pointer" :class="AboutComp == true ? 'text-amber-100' : 'text-green-500'">1. HOME</div>
                    <div @click="openAboutComp()" class="text-green-500 tracking-widest font-['Verdana'] pl-2 hover:cursor-pointer">2. ABOUT</div>
                    <div @click="openCVComp()" class="text-green-500 tracking-widest font-['Verdana'] pl-2 hover:cursor-pointer" :class="CVComp == true ? 'text-amber-100' : 'text-green-500'">3. CV</div>
                    <div class="text-green-500 tracking-widest font-['Verdana'] pl-2 hover:cursor-pointer">4. OTHER</div>
                </div>
            </section>
        </div>
        <div>
        </div>
    </main>
</template>

<script>
import AboutPage from './components/AboutPage.vue'
import CVPage from './components/CVPage.vue'

export default {
    name: 'App',
    components: {
        AboutPage,
        CVPage
    },
    data() {
        return {
            CVComp: false,
            AboutComp: true
        }
    },
    methods: {
        openCVComp() {
            this.CVComp = true
            this.AboutComp = false
        },
        openAboutComp() {
            this.AboutComp = true
            this.CVComp = false
        }
    }
}
</script>
