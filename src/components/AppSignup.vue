

<template>
    <section>
        <div class="container">
            <img src="/images/home_img-compressor.jpg" alt="">
            <div class="signUp">
                <h4>Sign Up For A Free Training Session!</h4>
                <!--Inserire il v-model-->
                <form>
                    <div class="form-group">
                        <label for="exampleInputEmail1">Name</label>
                        <input type="text" class="form-control" id="exampleInputEmail1" placeholder="Your Name">
                    </div>
                    <div class="form-group">
                        <label for="exampleInputPassword1">Email</label>
                        <input type="email" class="form-control" id="exampleInputPassword1" placeholder="email@example.com">
                    </div>
                    <button type="button" class="btn btn-secondary btn-lg btn-block">START NOW!</button>
                </form>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
section {
    background-color: hsl(210deg 6.06% 12.94%);
    color: white;

    .container {
        padding: 100px;
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 20px;


        img,
        .signUp {
            width: calc(50% - 100px - 20px);
        }

        label {
            color: hsl(0deg 0.58% 66.47%);
        }

        input {
            border-radius: 0;
            border: 1px solid hsl(0deg 0.58% 66.47%);
            background-color: hsl(210deg 6.06% 12.94%);
            color: white;
        }

        ::placeholder {
            color: hsl(0deg 0.58% 66.47%);
        }

        button {
            margin-top: 20px;
            background-color: #ee6059;
            border-radius: 0;
            border: 1px solid #ee6059;
            color: white;
            width: 100%;
        }
    }
}
</style>