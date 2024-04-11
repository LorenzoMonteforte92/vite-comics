<script>
    export default {
        name: 'AppMainNav',

        data(){
            return{
                links:[
                    {
                        img: 'comics-digital-comics.png',
                        text: `DIGITAL COMICS`,
                    },
                    {
                        img: 'comics-merchandise.png',
                        text: `DC MERCHANDISE`,
                    },
                    {
                        img: 'comics-subscriptions.png',
                        text: `SUBSCRIPTION`,
                    },
                    {
                        img: 'comics-shop-locator.png',
                        text: `SHOP LOCATOR`,
                    },
                    {
                        img: 'dc-power-visa.svg',
                        text: `DC POWER VISA`,
                    }
                ]
            }
        },
        methods: {
            
            }
        }

//sistemare stampa delle immagini    
</script>

<template>
    <section>
        <div class="container">
            <div class="row">
                <nav class="col-12 py-2">
                    <ul class="d-flex justify-content-center align-items-center gap-5" >
                        <li 
                        class="d-flex justify-content-center align-items-center"
                        v-for="singleLink in links">
                            <div class="d-flex justify-content-center align-items-center" >
                                <img :src="`../assets/img/buy-${singleLink.img}` " alt="">
                            </div>
                            <p class="text-center pt-3" >{{singleLink.text}}</p>
                        </li>
                    </ul>   
                </nav>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;

section{
    background-color: $brand-primary-color;
}

img{
    width: 100%;
    height: 100%;
}

p{
    color: white;
}

</style>