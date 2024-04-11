<script>
    export default {
        name: 'AppFooterBottom',

        data(){
            return{
                links:[
                    {
                        img: `footer-facebook.png`
                    },
                    {
                        img: `footer-twitter.png`
                    },
                    {
                        img: `footer-youtube.png`
                    },
                    {
                        img: `footer-pinterest.png`
                    },
                    {
                        img: `footer-periscope.png`
                    },
                ]
            }
        },
        methods: {
            
            }
        }

    
</script>

<template>
    <section>
        <div class="container">
            <div class="row py-3">
                <div class="col-6">
                    <button class="fw-bold text-white p-2" >SIGN-UP NOW!</button>
                </div>
                <div class="col-6 d-flex justify-content-end">
                        <div class=" lh-lg fs-5 color-primary fw-bold" >FOLLOW US</div>
                        <div>
                            <ul class="d-flex gap-3" >
                                <li
                                v-for="singleLink in links"><a href="#"></a><img :src="`src/assets/img/${singleLink.img}` " alt=""></li>
                            </ul>
                        </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;

.color-primary{
    color: $brand-primary-color;
}

section{
    background-color: $brand-secondary-color;
}

button{
    background-color: transparent;
    color: white;
    border: 1px solid $brand-primary-color;
}
</style>