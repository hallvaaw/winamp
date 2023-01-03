<template>
    <h1 class="text-gray-100 text-center text-2xl font-['Verdana']">Education</h1>
    <section class="grid grid-cols-6">
        <div class="col-span-2">
            <h1 class="bg-slate-600 border border-b-gray-800 border-l-slate-600 border-t-slate-600 border-r-slate-900 text-gray-100 font-['Verdana'] px-6 pt-1">Title</h1>
            <div class="bg-gray-900 border-x-4 border-slate-600 px-4 py-2 text-sm xl:text-base">
                <h2 @mouseover="onHover(eduEntries[0])" @mouseleave="onLeave(eduEntries[0])" class="text-green-500 font-['Verdana']" :class="eduEntries[0].hover == true ? 'bg-indigo-900' : '' ">{{ eduEntries[0].Title }}</h2>
                <h2 @mouseover="onHover(eduEntries[1])" @mouseleave="onLeave(eduEntries[1])" class="text-green-500 font-['Verdana']" :class="eduEntries[1].hover == true ? 'bg-indigo-900' : '' ">{{ eduEntries[1].Title }}</h2>
            </div>
        </div>
        <div class="col-span-3">
            <h1 class="bg-slate-600 border border-b-gray-800 border-l-slate-600 border-t-slate-600 border-r-slate-900 text-gray-100 font-['Verdana'] px-6 pt-1">Details</h1>
            <div class="bg-gray-900 border-x-4 border-slate-600 px-4 py-2 text-sm xl:text-base">
                <h2 @mouseover="onHover(eduEntries[0])" @mouseleave="onLeave(eduEntries[0])" class="text-green-500 font-['Verdana']" :class="eduEntries[0].hover == true ? 'bg-indigo-900' : '' ">{{ eduEntries[0].Details }}</h2>
                <h2 @mouseover="onHover(eduEntries[1])" @mouseleave="onLeave(eduEntries[1])" class="text-green-500 font-['Verdana']" :class="eduEntries[1].hover == true ? 'bg-indigo-900' : '' ">{{ eduEntries[1].Details }}</h2>
            </div>
        </div>
        <div>
            <h1 class="bg-slate-600 border border-b-gray-800 border-l-slate-600 border-t-slate-600 border-r-slate-900 text-gray-100 font-['Verdana'] px-6 pt-1">Time</h1>
            <div class="bg-gray-900 border-x-4 border-slate-600 px-4 py-2 text-sm xl:text-base">
                <h2 @mouseover="onHover(eduEntries[0])" @mouseleave="onLeave(eduEntries[0])" class="text-green-500 font-['Verdana'] py-2 xl:py-1.5" :class="eduEntries[0].hover == true ? 'bg-indigo-900' : '' ">{{ eduEntries[0].Time }}</h2>
                <h2 @mouseover="onHover(eduEntries[1])" @mouseleave="onLeave(eduEntries[1])" class="text-green-500 font-['Verdana'] py-2 xl:py-1.5" :class="eduEntries[1].hover == true ? 'bg-indigo-900' : '' ">{{ eduEntries[1].Time }}</h2>
            </div>
        </div>
    </section>
    <div class="bg-slate-800 h-3"></div>
    <div class="bg-slate-700 h-4"></div>
    <h1 class="text-gray-100 text-center text-2xl font-['Verdana']">Work Experience</h1>
    <section class="grid grid-cols-6">
        <div class="col-span-2">
            <h1 class="bg-slate-600 border border-b-gray-800 border-l-slate-600 border-t-slate-600 border-r-slate-900 text-gray-100 font-['Verdana'] px-6 pt-1">Title</h1>
            <div v-for="job in jobEntries" class="bg-gray-900 border-x-4 border-slate-600 px-4 p-1 text-sm xl:text-base">
                <h2 @mouseover="onHover(job)" @mouseleave="onLeave(job)" class="text-green-500 font-['Verdana'] py-1.5 xl:py-2" :class="job.hover == true ? 'bg-indigo-900' : '' ">{{ job.Title }}</h2>
            </div>
        </div>
        <div class="col-span-3">
            <h1 class="bg-slate-600 border border-b-gray-800 border-l-slate-600 border-t-slate-600 border-r-slate-900 text-gray-100 font-['Verdana'] px-6 pt-1">Details</h1>
            <div v-for="job in jobEntries" class="bg-gray-900 border-x-4 border-slate-600 px-4 p-1 text-sm xl:text-base">
                <h2 @mouseover="onHover(job)" @mouseleave="onLeave(job)" class="text-green-500 font-['Verdana'] py-3 xl:py-3" :class="job.hover == true ? 'bg-indigo-900' : '' ">{{ job.Details }}</h2>
            </div>
        </div>
        <div>
            <h1 class="bg-slate-600 border border-b-gray-800 border-l-slate-600 border-t-slate-600 border-r-slate-900 text-gray-100 font-['Verdana'] px-6 pt-1">Time</h1>
            <div v-for="job in jobEntries" class="bg-gray-900 border-x-4 border-slate-600 px-4 p-1 text-sm xl:text-base">
                <h2 @mouseover="onHover(job)" @mouseleave="onLeave(job)" class="text-green-500 font-['Verdana'] py-7 xl:py-5" :class="job.hover == true ? 'bg-indigo-900' : '' ">{{ job.Time }}</h2>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'CVPage',
    data() {
        return {
            eduEntries: [
                {Title: "Master's degree in molecular biology.", Details: "Automation of high throughput image analysis techniques in microscopy.", Time: "2019-2020", hover: false},
                {Title: "Bachelor's degree in biology", Details: "Molecular and computational biology", Time: "2015-2018", hover: false}],
            jobEntries: [
                {Title: "Doctoral candidate in computational biology.", Details: "Computational analysis of gene regulation in development and disease.", Time: "2020-t.d", hover: false},
                {Title: "Scientific assistant in Python programming.", Details: "Making curriculum and coding challenges in Python for a course in computational biology.", Time: "2020", hover: false},
                {Title: "Teaching assistant in Python programming.", Details: "Tutoring, reviewing code and live coding in Python.", Time: "2019", hover: false},
                {Title: "Scientific assistant in R programming.", Details: "Making curriculum, coding challenges and exercises for a course in statistics.", Time: "2019", hover: false},
                {Title: "Summer intern in computational biology.", Details: "Data sorting, analysis and visualization.", Time: "2019", hover: false},
                {Title: "Scientific assistant in R programming.", Details: "Making curriculum, coding challenges and exercises for a course in statistics.", Time: "2018", hover: false}
            ],
            hoverState: false
        }
    },
    methods: {
        onHover(e) {
            e.hover = true
        },
        onLeave(e) {
            e.hover = false
        }
    }
}
</script>
