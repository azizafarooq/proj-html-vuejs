<script>
export default {
    data() {
        return {
        }
    }
}
</script>

<template>
    <section>
        <p class="main-title">REAL WORLD RESULTS</p>
        <font-awesome-icon class="xmark-combo" v-for="xmark in 2" :icon="['fas', 'xmark']" style="color: #ee6059;" />
        <div class="cards">
            <div class="card">
                <img class="card-img-top" src="/images/review_1-compressor.jpg">
                <div class="description"> "The trainers at Avada GYm have helped me reach my fitness goals beyond anything I
                    could of hoped for. I love it!"
                    <div class="name"><strong> -Tara smith</strong></div>
                </div>
            </div>
            <div class="card">
                <img class="card-img-top" src="/images/review_2-compressor.jpg">
                <div class="description"> "The trainers at Avada GYm have helped me reach my fitness goals beyond anything I
                    could of hoped for. I love it!"
                    <div class="name"></div><strong> -Tara smith</strong>
                </div>
            </div>
            <div class="card">
                <img class="card-img-top" src="/images/review_3-compressor-2.jpg">
                <div class="description"> "The trainers at Avada GYm have helped me reach my fitness goals beyond anything I
                    could of hoped for. I love it!"
                    <div class="name"></div><strong> -Tara smith</strong>
                </div>
            </div>

            <div class="card">
                <img class="card-img-top" src="/images/review_4-compressor-2.jpg">
                <div class="description"> "The trainers at Avada GYm have helped me reach my fitness goals beyond anything I
                    could of hoped for. I love it!"
                    <div class="name"><strong> -Tara Smith </strong> </div>
                </div>
            </div>
        </div>


        <!--Inserire dinamicamente e fare il modale-->
        <div class="images-links">
            <p class="main-title"> HIGH PERFOMANCE FACILITIES</p>
            <font-awesome-icon class="xmark-combo" v-for="xmark in 2" :icon="['fas', 'xmark']" style="color: #ee6059;" />
            <div class="images">
                <img src="/images/home-image1.jpg" alt="">
                <img src="/images/home-image2.jpg" alt="">
                <img src="/images/home-image3.jpg" alt="">
                <img src="/images/home-image4.jpg" alt="">
                <img src="/images/home-image54.jpg" alt="">
                <img src="/images/home-image6.jpg" alt="">
            </div>
        </div>


    </section>
</template>

<style lang="scss" scoped>
section {
    background-color: hsl(200deg 7.5% 15.69%);
    padding: 100px 150px;
    text-align: center;

    .cards {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        align-items: center;
        gap: 20px;

        .card {
            flex-direction: row;
            width: calc((100% - 150px - 20px) / 2);
            border-radius: 0;
            background-color: hsl(210deg 6.06% 12.94%);
            padding: 20px;
            gap: 10px;
            font-style: italic;

            .description,
            .name {
                text-align: left;
                font-size: 0.8rem;
            }

            img {
                width: 150px;
                height: 150px;
                border-radius: 0;
            }
        }
    }

    .images-links {
        padding-top: 200px;
    }

    .images {
        display: flex;
        gap: 20px;
        flex-wrap: wrap;
        justify-content: center;

        img {
            width: calc((100% - 150px - 20px) / 3);
            cursor: pointer;
        }


    }

}
</style>