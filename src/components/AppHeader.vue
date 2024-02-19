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
        <div class="container">
            <!--Logo-->
            <img src="/Images/gym_logo_1x.png" alt="">

            <!--Menù dinamico-->
            <ul>
                <li v-for="link in links">{{ link.text }}</li>
            </ul>
        </div>

    </header>
</template>

<style lang="scss" scoped>
//Sistemare css
header {
    background-color: #1E2123;
    padding: 3rem;

    .container {
        display: flex;
        color: white;
        justify-content: space-between;
        align-items: center;
    }

    ul {
        display: flex;
        gap: 10px;
    }
}
</style>