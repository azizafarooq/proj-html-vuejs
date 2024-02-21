<template>
    <footer>
        <div class="container">
            <a href="#"> Copyright 2012 - 2020
            </a>
            |
            <a href="#"> Avada Theme by Theme Fusione
            </a>
            |
            <a href="#"> All Right Reserved
            </a>
            |
            <a href="#"> Powered By Wordpress
            </a>
        </div>
        <div class="icons">
            <font-awesome-icon class="social-links" :icon="['fab', 'facebook-f']" />
            <font-awesome-icon class="social-links" :icon="['fab', 'twitter']" />
            <font-awesome-icon class="social-links" :icon="['fab', 'instagram']" />
        </div>
    </footer>
</template>
<style lang="scss" scoped>
footer {
    background-color: #1A1C1E;
    padding: 50px 200px;
    color: #8D8D8D;
    display: flex;
    gap: 30px;

    .container {
        display: flex;
        gap: 10px;

        a {
            color: #8D8D8D;
            font-size: 15px;
        }
    }

    .icons {
        display: flex;
        gap: 10px;

        .social-links {
            color: white;
            width: 20px;
            height: 20px;
            padding: 10px;
            border-radius: 5px;
            cursor: pointer;
            background-color: #ee6059;
        }
    }
}
</style>