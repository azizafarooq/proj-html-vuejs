<script>
export default {
    data() {
        return {
        }
    }
}
</script>

<template>
    <main>
        <p class="main-title">MEET OUR TRAINERS</p>
        <font-awesome-icon class="xmark-combo" v-for="xmark in 2" :icon="['fas', 'xmark']" style="color: #ee6059;" />
        <div class="cards">
            <div class="card">
                <img class="card-img-top" src="/images/trainer1-400x297.jpg" alt="Card image cap">
                <div class="card-body">
                    <h5 class="card-title">Anna Baker</h5>
                    <h5 class="card-title">Personal Trainer</h5>
                    <p class="description">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor,
                        lorem ipsum dolor sit amet.
                    </p>
                    <p class="card-icons">
                        <font-awesome-icon class="social-links" :icon="['fab', 'facebook-f']" />
                        <font-awesome-icon class="social-links" :icon="['fab', 'twitter']" />
                        <font-awesome-icon class="social-links" :icon="['fab', 'instagram']" />
                    </p>
                </div>
            </div>
            <div class="card">
                <img class="card-img-top" src="/images/trainer3-400x297.jpg" alt="Card image cap">
                <div class="card-body">
                    <h5 class="card-title">Card title</h5>
                    <h5 class="card-title">Personal Trainer</h5>
                    <p class="description">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor,
                        lorem ipsum dolor sit amet.</p>
                    <p class="card-icons">
                        <font-awesome-icon class="social-links" :icon="['fab', 'facebook-f']" />
                        <font-awesome-icon class="social-links" :icon="['fab', 'twitter']" />
                        <font-awesome-icon class="social-links" :icon="['fab', 'instagram']" />
                    </p>
                </div>
            </div>
            <div class="card">
                <img class="card-img-top" src="/images/trainer4-400x297.jpg" alt="Card image cap">
                <div class="card-body">
                    <h5 class="card-title">Card title</h5>
                    <h5 class="card-title">Personal Trainer</h5>
                    <p class="description">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor,
                        lorem ipsum dolor sit amet.</p>
                    <p class="card-icons">
                        <font-awesome-icon class="social-links" :icon="['fab', 'facebook-f']" />
                        <font-awesome-icon class="social-links" :icon="['fab', 'twitter']" />
                        <font-awesome-icon class="social-links" :icon="['fab', 'instagram']" />
                    </p>
                </div>
            </div>
        </div>

        <button>VIEW ALL TRAINERS</button>
        <font-awesome-icon class="sortDown" :icon="['fas', 'sort-down']" style="color:  #1F2123;" />
    </main>
</template>

<style lang="scss" scoped>
main {
    background-color: #1F2123;
    padding: 100px 200px;
    text-align: center;
    position: relative;

    .cards {
        display: flex;
        gap: 30px;
        justify-content: center;

        .card,
        img {
            border-radius: 0;
        }

        .card {
            width: calc((100% - 200px - 30px) / 3);
            background-color: hsl(200deg 7.5% 15.69%);
            color: white;

            .card-body {
                color: white;
                text-align: start;
                padding: 30px;
            }

            .card-icons {
                display: flex;
                gap: 10px;


                .social-links {
                    width: 20px;
                    height: 20px;
                    padding: 10px;
                    border-radius: 5px;
                    cursor: pointer;
                    background-color: #1F2123;
                }
            }

        }

    }

    button {
        margin-top: 3rem;
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