<script>
import { store } from '../store';
export default {
    data() {
        return {
            store
        }
    },
    methods: {
        closeModal() {
            this.store.modal.show = false
        }
    }
}
</script>
<template>
    <div class="layover">
        <div class="card" style="width: 26rem;">

            <div class="icons">
                <div class="icon-overlay"></div>
                <font-awesome-icon @click="closeModal()" :icon="['fas', 'xmark']" />
                <font-awesome-icon class="icon" :icon="['fas', 'link-slash']" />
                <font-awesome-icon class="icon" :icon="['fas', 'magnifying-glass']" />
            </div>
            <div class="card-body">
                <h5 class="title">Train with free weights or body weight?</h5>
                <p class="description">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor, lorem
                    ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.layover {
    position: fixed;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;

    background-color: rgba(71, 68, 68, 0.516);

    display: flex;
    justify-content: center;
    align-items: center;

    img,
    .card {
        border-radius: 0;
    }

    .card {
        background-color: #25292B;
        color: white;
        padding: 20px 20px;
        position: relative;

        .title {
            font-size: 1.5rem;
        }

        .icons {
            position: relative;
            background-image: url("/images/blog1-800x415.jpg");
            background-size: cover;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 100px;
            gap: 20px;

            .icon {
                cursor: pointer;
                font-size: 2rem;
                z-index: 2;
            }

            .icon-overlay {
                position: absolute;
                top: 0;
                left: 0;
                width: 100%;
                height: 100%;
                background-color: hsla(3.03deg, 58.62%, 60.2%, 0.69);
                z-index: 1;
            }

            .fa-xmark {
                font-size: 2rem;
                position: absolute;
                right: 0;
                top: 0;
                padding: 0.5rem 1rem;
                cursor: pointer;
                z-index: 3;
            }

        }

        .card-body {
            background-color: #1E2123;
        }
    }
}
</style>