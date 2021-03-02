<template>
    <div id="Home">
        <div class="videoContainer">
            <video autoplay muted loop id="homeVideo" src="../assets/img/pexels-pavel-danilyuk-5495781.mp4"></video>
            <p>資 訊 安 全 <br />情 報 服 務 平 台</p>
        </div>

        <div class="leftHeader">
            <div @click="navbarToggle()" :class="{ open: navbarIsOpen }" class="navbar-btn">
                <div class="navbar-btn-line"></div>
            </div>
            <div class="planner">
                <p>莊文勝教授 /</p>
                <p>黃閔弘 /</p>
                <p>龔詠鴻</p>
            </div>
            <h2>NKUST</h2>
            <nav :class="{ navbarOpen: navbarIsOpen }">
                <div class="leftnav">
                    <h1>NKUST</h1>
                    <h2>IM</h2>
                    <h3>指 導 教 授：莊 文 勝</h3>
                    <h3>製 作 人 員：黃 閔 弘</h3>
                    <h3>製 作 人 員：龔 詠 鴻</h3>
                    <div class="navIconContainer">
                        <a class="navIcon" href="https://github.com/minhonglolz/nkust_topic.git" target="_bland"><img src="../assets/img/github-icon.png" alt=""/></a>
                        <a class="navIcon vueIcon" href="https://v3.vuejs.org/" target="_bland"><img src="../assets/img/logo.png" alt=""/></a>
                    </div>
                </div>
                <div class="rightnav">
                    <img src="../assets/img/hackerimg.png" alt="" />
                    <p>此 網 站 僅 供 應 學 術 研 究 !</p>
                </div>
            </nav>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Home',
    props: {
        msg: String,
    },
    data() {
        return {
            navbarIsOpen: false,
        };
    },
    methods: {
        navbarToggle() {
            this.navbarIsOpen = !this.navbarIsOpen;
        },
    },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
