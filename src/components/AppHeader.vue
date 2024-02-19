<script>
export default {
    data() {
        return {
            links: [
                {
                    text: 'HOME',
                    url: '#',
                    current: true,
                },
                {
                    text: 'ABOUT US',
                    url: '#',
                    current: true,
                },
                {
                    text: 'FACILITIES',
                    url: '#',
                    current: true,
                },
                {
                    text: 'MEMBERSHIP',
                    url: '#',
                    current: true,
                },
                {
                    text: 'TESTIMONIALS',
                    url: '#',
                    current: true,
                },
                {
                    text: 'BLOG',
                    url: '#',
                    current: true,
                },

            ],
        };
    },
};
</script>

<template>
    <header>
        <!--Logo-->
        <img src="../assets/Images/gym_logo_1x.png" alt="">

        <!--Menù dinamico-->
        <ul>
            <li v-for="link in links">{{ link.text }}</li>
        </ul>
    </header>
</template>

<style lang="scss" scoped>
//Sistemare css
header {
    display: flex;
    justify-content: space-between;

    ul {
        display: flex;
        gap: 10px;
    }
}
</style>