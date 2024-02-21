<script>
export default {
    data() {
        return {
        }
    }
}
</script>

<template>
    <footer>
        <section class="footer-primary">
            <div>
                <p>COME FIND US</p>
                <ul>
                    <li>12345 North Main Street</li>
                    <li>New York, NY 555555</li>
                    <li>Phone: 1.800.555.6789</li>
                    <li>Email: info@yourdomain.com</li>
                </ul>
            </div>
            <div>
                <p>RECENTS POSTS</p>
                <ul>
                    <li><font-awesome-icon :icon="['fas', 'angle-right']" /> Train with free weight or your body weight?
                    </li>
                    <hr>
                    <li><font-awesome-icon :icon="['fas', 'angle-right']" /> Nutritional advice that will keep you training
                    </li>
                    <hr>
                </ul>
            </div>
            <div>
                <p>OPENING TIMES</p>
                <ul class="schedule">
                    <li>Weekdays Monday - Friday</li>
                    <li class="date">9:00 - 19:00</li>
                    <li>Weekdays Saturday - Sunday</li>
                    <li class="date">9:00 - 21:00</li>
                </ul>
            </div>
            <div>
                <img src="/images/gym_ad-compressor.jpg" alt="">
            </div>
        </section>
    </footer>
</template>

<style lang="scss" scoped>
footer {
    background-color: #1F2123;
    padding: 150px 200px;


    .footer-primary {
        color: #565F62;
        display: flex;
        justify-content: space-around;
        gap: 30px;

        li {

            color: #999999;
            line-height: 30px;
            cursor: pointer;
            font-size: 10px;
        }


        .schedule {
            li {
                cursor: auto;
            }

            .date {
                color: #565F62;
            }

        }

        img {
            cursor: pointer;
        }
    }
}
</style>