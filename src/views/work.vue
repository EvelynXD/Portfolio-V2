<template>
    <div class="work view-page">
        <div class="text">
            <h1 class="title">
                <div class="outline-text">Projects</div>
                <span class="hov">M</span>
                <span class="hov">y</span>
                <span class="space"></span>
                <span class="hov">p</span>
                <span class="hov">r</span>
                <span class="hov">o</span>
                <span class="hov">j</span>
                <span class="hov">e</span>
                <span class="hov">c</span>
                <span class="hov">t</span>
                <span class="hov">s</span>
            </h1>
        </div>

        <div class="work-list">
            <div class="work" v-for="(work, index) in myProjects" :key="index">
                <div class="information">
                    <h2 class="work-number">0{{ index + 1 }}.</h2>
                    <h1 class="work-title">
                        {{ work.title }}
                    </h1>
                    <img
                        :src="require(`@/assets/${work.img}`)"
                        alt=""
                        class="mobile-img"
                    />
                    <p class="description">
                        {{ work.description }}
                    </p>
                    <div class="tools">
                        <p>
                            Code Tools:
                            <span>{{ work.codeTools.join(", ") }}</span>
                        </p>
                        <p class="design">
                            Design: <span>{{ work.design }}</span>
                        </p>
                    </div>
                    <div class="links">
                        <a
                            target="_blank"
                            class="btn"
                            :href="work.link"
                            :class="work.link === '' ? 'disabled' : ''"
                            >Visit</a
                        >
                        <a
                            target="_blank"
                            class="btn"
                            :href="work.source"
                            :class="work.source === '' ? 'disabled' : ''"
                            >Source Code</a
                        >
                    </div>
                </div>
                <div class="img">
                    <img :src="require(`@/assets/${work.img}`)" alt="" />
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            isExpand: false,
            icon: "fas fa-expand",
            isDetail: false,
            myProjects: [
                {
                    title: "Fireworks 2023",
                    description:
                        "Happy New Year!",
                    source:
                        "https://github.com/EvelynXD/firework-2023",
                    link: "https://evelynxd.github.io/firework-2023/",
                    img: "fireworks-2023.png",
                    codeTools: ["HTML", "CSS", "Javascript"],
                    design: "Design by Evelyn",
                },
                {
                    title: "Kebelet Iphone",
                    description:
                        "This Kebelet Iphone is for people who have high prestige, but if you want to try it, you can.",
                    source:
                        "https://github.com/EvelynXD/Kebelet-Iphone",
                    link:
                        "https://kebelet-iphone.vercel.app/",
                    img: "kebelet-iphone.png",
                    codeTools: ["HTML", "CSS", "PHP"],
                    design: "Design by Evelyn",
                },
                {
                    title: "Herta Kuru",
                    description:
                        "The website for Herta, the cutest genius Honkai: Star Rail character out there.",
                    source: "https://github.com/EvelynXD/kuru-kuru",
                    link: "https://kuru-kuru.vercel.app/",
                    img: "herta-kuru.png",
                    codeTools: ["HTML", "CSS", "Javascript"],
                    design: "Design by Haviza Aufa",
                },
                {
                    title: "First Profile",
                    description:
                        "My first portfolio",
                    source:
                        "https://github.com/EvelynXD/first-profile",
                    link:
                        "https://evelynxd.vercel.app/",
                    img: "firts-portfolio.png",
                    codeTools: ["React JS"],
                    design: "Design by Me",
                },
                {
                    title: "Terminal Portfolio",
                    description:
                        "Terminal Portfolio is a portfolio website that is made to look like a terminal.",
                    source:
                        "https://github.com/EvelynXD/terminal",
                    link: "https://evelyn-terminal.vercel.app/",
                    img: "terminal-portfolio.png",
                    codeTools: [
                        "TypeScript",
                        "React JS",
                        "Next JS",
                        "Tailwind CSS",
                    ],
                    design: "Design by Evelyn",
                },
                {
                    title: "Game Snake",
                    description:
                        "This project can be accessed through a web browser and has been optimized for a responsive display, which means the game can be played on various devices, both desktop and mobile devices.",
                    source: "https://github.com/EvelynXD/Snake-",
                    link: "https://evelynxd.github.io/Snake-/",
                    img: "snake.png",
                    codeTools: ["HTML", "CSS", "Javascript"],
                    design: "Design by Evelyn",
                },
                {
                    title: "Statued (Landing Page)",
                    description:
                        "Online shop for statue customization with 3d look.",
                    source: "https://github.com/GunawanAhmad/Statued",
                    link: "https://statued.vercel.app/",
                    img: "statued.png",
                    codeTools: [
                        "HTML",
                        "Tailwind CSS",
                        "Javascript",
                        "Three Js",
                    ],
                    design: "Design by Igun",
                },
                {
                    title: "Web Application for Online Consultation (Kliniku)",
                    description:
                        "Kliniku is an online consultation platform where people can fill in an online form about their health issue to send for a doctor. The doctor can respond and give them medical advice.",
                    source:
                        "https://github.com/EvelynXD/Sisfo-Klinik-Full-Stack",
                    link: "",
                    codeTools: ["VueJS", "MongoDB", "NodeJs", "ExpressJS"],
                    design: "Design by Faris Azizy",
                    img: "kliniku.png",
                },
            ],
        };
    },
    mounted() {},
    methods: {},
};
</script>

<style scoped src="../styles/work.css"></style>
