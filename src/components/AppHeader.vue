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
                    current: false,
                },
                {
                    text: 'FACILITIES',
                    url: '#',
                    current: false,
                },
                {
                    text: 'MEMBERSHIP',
                    url: '#',
                    current: false,
                },
                {
                    text: 'TESTIMONIALS',
                    url: '#',
                    current: false,
                },
                {
                    text: 'BLOG',
                    url: '#',
                    current: false,
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

        <!--Banner-->
        <div class="banner">
            <h1>NO PAIN NO GAIN</h1>
            <p class="pt-6">Motivation is what gets you started. Habit is what keeps you going.</p>
            <button class="mt-3">Join us today</button>
        </div>
    </header>

    <!--Jumbotron-->
    <div class="jumbotron">
        <p class="main-title">WORLD CLASS Fitness</p>
        <font-awesome-icon class="xmark" v-for="xmark in 2" :icon="['fas', 'xmark']" style="color: #ee6059;" />
        <p class="description">At Avada Gym, everything we do from top to bottom is of the highest quality to ensure we're
            equipped
            to help
            you to reach reach your your goals of a healthy and fit lifestyle. </p>
        <font-awesome-icon class="sortDown" :icon="['fas', 'sort-down']" style="color: #25292b;" />
    </div>
</template>

<style lang="scss" scoped>
header {
    padding: 2.5rem;
    padding-bottom: 300px;
    background-image: url('/Images/home-banner.jpg');
    background-size: cover;

    img {
        cursor: pointer;
    }

    .container {
        display: flex;
        color: white;
        justify-content: space-between;
        align-items: center;
    }

    ul {
        display: flex;
        gap: 10px;
        font-size: small;

        li {
            padding: 0.5rem;
            cursor: pointer;
        }
    }

    .banner {
        color: white;
        text-align: center;

        h1 {
            font-weight: bold;
            font-size: 4.3rem;
            margin-top: 150px;
        }

        p {
            font-weight: lighter;
        }

        button {
            background-color: transparent;
            color: white;
            border: 0.5px solid #EBEAEA;
            font-weight: lighter;
            padding: 5px 20px;
        }
    }
}

.jumbotron {
    background-color: hsl(200deg 7.5% 15.69%);
    color: white;
    text-align: center;
    padding: 100px 150px;
    position: relative;

    .xmark {
        padding: 3rem 0.3rem;
    }

    .sortDown {
        font-size: 9rem;
        position: absolute;
        bottom: -50px;
        left: 50%;
        transform: translateX(-50%);
    }

}
</style>