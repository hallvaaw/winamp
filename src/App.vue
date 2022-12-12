<template>
    <main class="bg-slate-800">
        <header class="container flex flex-row border-b-2 border-b-gray-900 mx-auto text-center justify-center">
            <div class="flex flex-col my-4">
                <div class="bg-amber-200 border-2 border-b-[1px] rounded-t-xl rounded-b border-gray-900 px-[296px] h-2"></div>
                <div class="bg-amber-300 border-2 border-t-[1px] rounded-b-xl rounded-t border-gray-900 px-[296px] h-2"></div>
            </div>
            <h1 class="text-slate-300 text-2xl font-bold tracking-wider font-['Verdana'] pt-2">HALLVARD A. WÆHLER</h1>
            <div class="flex flex-col my-4">
                <div class="bg-amber-200 border-2 border-b-[1px] rounded-t-xl rounded-b border-gray-900 px-[296px] h-2"></div>
                <div class="bg-amber-300 border-2 border-t-[1px] rounded-b-xl rounded-t border-gray-900 px-[296px] h-2"></div>
            </div>
        </header>
        <div class="container flex flex-col border-t-[1px] border-t-gray-400 mx-auto">
            <section id="top" class="flex flex-col bg-slate-700">
                <div class="flex flex-row bg-slate-700 justify-between">
                    <div class="bg-gray-400 h-36 w-56 p-12"></div>
                    <div class="w-88 text-center">
                        <h2 class="text-2xl font-bold tracking-wider font-['Verdana'] items-center">I am a bioinformatician and developer</h2>
                    </div>
                    <div class="items-center justify-right">
                        <div class="bg-gray-900 border-2 border-gray-600 border-t-gray-900 border-l-gray-900 text-green-500 tracking-widest font-['Verdana'] text-xl py-2 pr-16 pl-1"><marquee>WELCOME TO MY HOMEPAGE</marquee></div>
                        <div class="text-right py-6">
                            <button class="border-4 border-b-gray-500 border-x-gray-600 border-t-gray-200 rounded bg-gray-300 tracking-widest font-['Verdana'] p-1 pr-2 my-2 active:border-l-gray-200 active:border-t-gray-500 active:border-b-0 active:border-t-6"><a href="https://github.com/hallvaaw" target="_blank" rel="noopener noreferrer">GITHUB</a></button>
                            <button class="border-4 border-b-gray-500 border-x-gray-600 border-t-gray-200 rounded bg-gray-300 tracking-widest font-['Verdana'] p-1 pr-2 my-2 active:border-r-gray-200 active:border-t-gray-500 active:border-b-0 active:border-t-6"><a href="https://www.linkedin.com/in/hallvard-austin-wæhler/" target="blank_" rel="noopener noreferrer">LINKEDIN</a></button>
                        </div>
                    </div>
                </div>
                <div class="bg-slate-800 border-2 border-gray-600 border-t-gray-900 border-l-gray-900 h-8 mt-6 mx-16"></div>
        <div class="container flex flex-row border-b-2 border-b-gray-900 mx-auto text-center justify-center">
            <div class="flex flex-col my-4">
                <div class="bg-amber-200 border-2 border-b-[1px] rounded-t-xl rounded-b border-gray-900 px-[296px] h-1.5"></div>
                <div class="bg-amber-300 border-2 border-t-[1px] rounded-b-xl rounded-t border-gray-900 px-[296px] h-1.5"></div>
            </div>
            <h1 class="text-slate-300 text-2xl font-bold tracking-wider font-['Verdana'] pt-2">ABOUT</h1>
            <div class="flex flex-col my-4">
                <div class="bg-amber-200 border-2 border-b-[1px] rounded-t-xl rounded-b border-gray-900 px-[296px] h-1.5"></div>
                <div class="bg-amber-300 border-2 border-t-[1px] rounded-b-xl rounded-t border-gray-900 px-[296px] h-1.5"></div>
            </div>
        </div>
                <div class="flex flex-row justify-left bg-slate-700">
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
                </div>
            </section>
        <div class="container flex flex-row border-b-2 border-b-gray-900 mx-auto text-center justify-center">
            <div class="flex flex-col my-4">
                <div class="bg-amber-200 border-2 border-b-[1px] rounded-t-xl rounded-b border-gray-900 px-[330px] h-1.5"></div>
                <div class="bg-amber-300 border-2 border-t-[1px] rounded-b-xl rounded-t border-gray-900 px-[330px] h-1.5"></div>
            </div>
            <h1 class="text-slate-300 text-2xl font-bold tracking-wider font-['Verdana'] pt-2">MORE THINGS</h1>
            <div class="flex flex-col my-4">
                <div class="bg-amber-200 border-2 border-b-[1px] rounded-t-xl rounded-b border-gray-900 px-[330px] h-1.5"></div>
                <div class="bg-amber-300 border-2 border-t-[1px] rounded-b-xl rounded-t border-gray-900 px-[330px] h-1.5"></div>
            </div>
        </div>
            <section id="bottom" class="flex flex-col bg-slate-800">
                <div class="border-2 border-gray-800 border-b-gray-200 border-r-gray-200 bg-gray-900">
                    <p class="text-amber-100 tracking-widest font-['Verdana']">1. HOME</p>
                    <p class="text-green-500 tracking-widest font-['Verdana']">2. ABOUT</p>
                    <p class="text-green-500 tracking-widest font-['Verdana']">3. CV</p>
                    <p class="text-green-500 tracking-widest font-['Verdana']">4. OTHER</p>
                </div>
                <div></div>
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
