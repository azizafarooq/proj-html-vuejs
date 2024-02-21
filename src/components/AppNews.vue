<template>
    <section>
        <p class="main-title">PERFOMANCE NEWS</p>
        <font-awesome-icon class="xmark-combo" v-for="xmark in 2" :icon="['fas', 'xmark']" style="color: #ee6059;" />

        <div class="cards">
            <div class="card">
                <img class="card-img-top" src="/images/blog1.jpg" alt="Card image cap">
                <div class="card-body">
                    <h5 class="card-title">Train with free weights or your bodyweight?</h5>
                    <p class="description">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor,
                        lorem ipsum dolor sit amet.
                    </p>
                </div>
            </div>
            <div class="card">
                <img class="card-img-top" src="/images/blog6-600x600.jpg" alt="Card image cap">
                <div class="card-body">
                    <h5 class="card-title">Nutritional advice that will keep you training</h5>
                    <p class="description">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor,
                        lorem ipsum dolor sit amet.</p>
                </div>
            </div>
            <div class="card">
                <img class="card-img-top" src="/images/trainer4-400x297.jpg" alt="Card image cap">
                <div class="card-body">
                    <h5 class="card-title">To be number one, train like you're number two</h5>
                    <p class="description">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor,
                        lorem ipsum dolor sit amet.</p>
                </div>
            </div>
            <div class="card">
                <img class="card-img-top" src="/images/blog4-600x433.jpg" alt="Card image cap">
                <div class="card-body">
                    <h5 class="card-title">Top 5 mistakes every gym member makes</h5>
                    <p class="description">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor,
                        lorem ipsum dolor sit amet.</p>
                </div>
            </div>
            <div class="card">
                <img class="card-img-top" src="/images/trainer3-600x445.jpg" alt="Card image cap">
                <div class="card-body">
                    <h5 class="card-title">The myth of shedding body fat explored</h5>
                    <p class="description">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor,
                        lorem ipsum dolor sit amet.</p>
                </div>
            </div>
            <div class="card">
                <img class="card-img-top" src="/images/trainer1.jpg" alt="Card image cap">
                <div class="card-body">
                    <h5 class="card-title">Train with free weights or your bodyweight?</h5>
                    <p class="description">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor,
                        lorem ipsum dolor sit amet.</p>
                </div>
            </div>
        </div>
    </section>
    <div class="banner">
        <div class="container">
            <div class="text">
                <p class="main-title">Achieve Your Fitness Goals</p>
                <p class="decription">Flexible membership packages to suit all levels of athlete and achieve your fitness
                    goals
                </p>
            </div>
            <div>
                <button>JOIN US</button>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
section {
    background-color: hsl(200deg 7.5% 15.69%);
    padding: 100px 200px;
    text-align: center;

    .cards {
        display: flex;
        gap: 30px;
        justify-content: center;
        flex-wrap: wrap;


        .card,
        img {
            border-radius: 0;
        }

        .card {
            width: calc((100% - 200px - 30px) / 3);
            height: fit-content;
            background-color: #1F2123;
            color: white;

            .card-body {
                color: white;
                text-align: start;
                padding: 20px;

            }
        }
    }
}

.banner {
    background-image: url('/images/home-parallax.jpg');
    padding: 80px 200px;

    .container {
        width: calc(100% - 200px);
        display: flex;
        color: white;
        justify-content: space-between;
        align-items: center;

        .text {
            font-size: 0.8rem;
        }

    }
}
</style>