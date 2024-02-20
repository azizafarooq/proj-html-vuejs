<script>
export default {
    data() {
        return {
            items: [
                {
                    icon: 'link-slash',
                    title: 'Strength and Conditioning',
                    description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.',
                },
                {
                    icon: 'bicycle',
                    title: 'Fitness and Cardio',
                    description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.',
                },
                {
                    icon: 'cloud',
                    title: 'Felxibility and Rest',
                    description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.',
                },
                {
                    icon: 'heart-pulse',
                    title: 'Health and Diet',
                    description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.',
                },

            ]
        }
    }
}
</script>
<template>
    <section>
        <!-- Icone dinamiche-->
        <div class="items" v-for="item in  items ">
            <font-awesome-icon class="icons" :icon="['fas', item.icon]" style="color: #ee6059;" />
            <p class="title">{{ item.title }}</p>
            <font-awesome-icon class="xmark" :icon="['fas', 'xmark']" style="color: #ee6059;" />
            <p class="description">{{ item.description }}</p>

        </div>
    </section>
</template>
<style lang="scss" scoped>
section {
    padding: 100px 150px;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 30px;
    background-image: url('/images/gym_bkgd_bw-compressor.jpg');
    background-size: cover;

    .items {
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 10px;
        width: calc((100% - 150px - 30px - 50px) / 4);

        .icons {
            width: 50px;
            height: 50px;
            padding: 20px;
            border-radius: 50%;
            border: 3px solid #ee6059;
            margin-bottom: 10px;
        }

        .description {
            text-align: center;
        }
    }
}
</style>