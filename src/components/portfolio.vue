<template>
    <div class="portfolio section">
        <div class="text">
            <h1 class="title">
                <div class="outline-text">Portfolio</div>
                <span class="hov">M</span>
                <span class="hov">y</span>
                <span class="space"></span>
                <span class="hov">p</span>
                <span class="hov">o</span>
                <span class="hov">r</span>
                <span class="hov">t</span>
                <span class="hov">f</span>
                <span class="hov">o</span>
                <span class="hov">l</span>
                <span class="hov">i</span>
                <span class="hov">o</span>
            </h1>
            <p class="desc">A small gallery of my recent projects</p>
        </div>
        <div @click="menuBackgroundAnim(1)" ref="btn" class="btn">
            <router-link to="/work">
                See more!
            </router-link>
        </div>
        <div class="gallery">
            <div>
                <a href="https://kuru-kuru.vercel.app/" target="_blank">
                    <img src="../assets/herta-kuru_box.png" alt="" />
                </a>
            </div>
            <div>
                <a
                    href="https://kebelet-iphone.vercel.app/"
                    target="_blank"
                >
                    <img src="../assets/kebelet-iphone_box.png" alt="" />
                </a>
            </div>
            <div>
                <a
                    href="https://evelynxd.github.io/firework-2023/"
                    target="_blank"
                >
                    <img src="../assets/fireworks-2023_box.png" alt="" />
                </a>
            </div>
            <div>
                <a
                    href="https://evelyn-terminal.vercel.app/"
                    target="_blank"
                >
                    <img src="../assets/terminal-portfolio_box.png" alt="" />
                </a>
            </div>
            <div>
                <a
                    href="https://evelynxd.vercel.app/"
                    target="_blank"
                >
                    <img src="../assets/firts-portfolio_box.png" alt="" />
                </a>
            </div>
            <div>
                <a href="https://evelynxd.github.io/Snake-/" target="_blank">
                    <img src="../assets/snake_box.png" alt="" />
                </a>
            </div>
            <div>
                <a href="https://statued.vercel.app/" target="_blank">
                    <img src="../assets/statued_box.png" alt="" />
                </a>
            </div>
            <div>
                <a
                    href="https://github.com/GunawanAhmad/Sisfo-Klinik-Full-Stack"
                    target="_blank"
                >
                    <img src="../assets/kliniku_box.png" alt="" />
                </a>
            </div>
        </div>
    </div>
</template>
<script>
import TransitionMixin from "../mixins/transition";

export default {
    mixins: [TransitionMixin],
};
</script>

<style scoped src="../styles/work.css"></style>
