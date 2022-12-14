<template>
    <main class="bg-slate-800 pt-4 mb-80">
        <header class="container flex flex-row mx-auto text-center justify-center px-64">
            <div class="flex flex-col my-4">
                <div class="bg-amber-200 border-2 border-b-[1px] rounded-t-xl rounded-b border-gray-900 px-40 h-2"></div>
                <div class="bg-amber-300 border-2 border-t-[1px] rounded-b-xl rounded-t border-gray-900 px-40] h-2"></div>
            </div>
            <h1 class="text-slate-300 text-2xl font-bold tracking-wider font-['Verdana'] pt-2">HALLVARD A. WÆHLER</h1>
            <div class="flex flex-col my-4">
                <div class="bg-amber-200 border-2 border-b-[1px] rounded-t-xl rounded-b border-gray-900 px-40 h-2"></div>
                <div class="bg-amber-300 border-2 border-t-[1px] rounded-b-xl rounded-t border-gray-900 px-40 h-2"></div>
            </div>
        </header>
        <div class="container flex flex-col mx-auto px-64">
            <section id="top" class="flex flex-col bg-slate-700">
                <div class="flex flex-row bg-slate-700 justify-between">
                    <div class="w-88 text-center pt-6">
                        <h2 class="text-gray-200 text-4xl font-bold tracking-wider font-['Verdana'] justify-left text-left pl-6">I am a bioinformatician and developer.</h2>
                    </div>
                    <div class="items-center justify-right">
                        <div class="bg-gray-900 border-2 border-gray-600 border-t-gray-900 border-l-gray-900 text-green-500 tracking-widest font-['Verdana'] text-xl py-2 pl-1"><marquee>WELCOME TO MY HOMEPAGE</marquee></div>
                        <div class="text-left">
                            <button class="border-4 border-b-gray-500 border-x-gray-600 border-t-gray-200 rounded bg-gray-300 tracking-widest font-['Verdana'] p-1 pr-2 my-2 active:border-l-gray-200 active:border-t-gray-500 active:border-b-0 active:border-t-6"><a href="https://github.com/hallvaaw" target="_blank" rel="noopener noreferrer">GITHUB</a></button>
                            <button class="border-4 border-b-gray-500 border-x-gray-600 border-t-gray-200 rounded bg-gray-300 tracking-widest font-['Verdana'] p-1 pr-2 my-2 active:border-r-gray-200 active:border-t-gray-500 active:border-b-0 active:border-t-6"><a href="https://www.linkedin.com/in/hallvard-austin-wæhler/" target="blank_" rel="noopener noreferrer">LINKEDIN</a></button>
                        </div>
                    </div>
                </div>
                <div class="bg-slate-800 border-2 border-gray-600 border-t-gray-900 border-l-gray-900 h-8 mx-16 my-8"></div>
        <div class="container flex flex-row bg-slate-800 border-2 border-x-4 border-gray-600 border-t-gray-900 border-x-slate-600 mx-auto text-center justify-center pb-2">
            <div class="flex flex-col my-4">
                <div class="bg-amber-200 border-2 border-b-[1px] rounded-t-xl rounded-b border-gray-900 px-40 h-1.5"></div>
                <div class="bg-amber-300 border-2 border-t-[1px] rounded-b-xl rounded-t border-gray-900 px-40 h-1.5"></div>
            </div>
            <h1 class="text-slate-300 text-2xl font-bold tracking-wider font-['Verdana'] pt-2">ABOUT</h1>
            <div class="flex flex-col my-4">
                <div class="bg-amber-200 border-2 border-b-[1px] rounded-t-xl rounded-b border-gray-900 px-40 h-1.5"></div>
                <div class="bg-amber-300 border-2 border-t-[1px] rounded-b-xl rounded-t border-gray-900 px-40 h-1.5"></div>
            </div>
        </div>
                <div class="flex flex-row justify-left bg-slate-700 mb-6">
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
                </div>
            </section>
        <div class="container flex flex-row border-y-2 border-x-4 border-x-slate-600 border-b-gray-600 border-t-gray-900 mx-auto text-center justify-center pb-2">
            <div class="flex flex-col my-4">
                <div class="bg-amber-200 border-2 border-b-[1px] rounded-t-xl rounded-b border-gray-900 px-48 h-1.5"></div>
                <div class="bg-amber-300 border-2 border-t-[1px] rounded-b-xl rounded-t border-gray-900 px-48 h-1.5"></div>
            </div>
            <h1 class="text-slate-300 text-2xl font-bold tracking-wider font-['Verdana'] pt-2">MORE THINGS</h1>
            <div class="flex flex-col my-4">
                <div class="bg-amber-200 border-2 border-b-[1px] rounded-t-xl rounded-b border-gray-900 px-48 h-1.5"></div>
                <div class="bg-amber-300 border-2 border-t-[1px] rounded-b-xl rounded-t border-gray-900 px-48 h-1.5"></div>
            </div>
        </div>
            <section id="bottom" class="flex flex-col bg-slate-800 min-h-screen">
                <div class="bg-gray-900 border-2 border-gray-600 border-t-gray-900 border-l-gray-900 mb-6">
                    <p class="text-amber-100 tracking-widest font-['Verdana']"><a href="#">1. HOME</a></p>
                    <p class="text-green-500 tracking-widest font-['Verdana']"><a href="#">2. ABOUT</a></p>
                    <p class="text-green-500 tracking-widest font-['Verdana']"><a href="#">3. CV</a></p>
                    <p class="text-green-500 tracking-widest font-['Verdana']"><a href="#">4. OTHER</a></p>
                </div>
            </section>
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
    }
}
</script>
