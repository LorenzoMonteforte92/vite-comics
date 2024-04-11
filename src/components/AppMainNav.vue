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
                <nav class="col-12 py-4">
                    <ul class="d-flex justify-content-center align-items-center" >
                        <li 
                        class="d-flex justify-content-center align-items-center"
                        v-for="singleLink in links">
                            <div class="d-flex justify-content-center align-items-center gap-3" >
                                <img :src="`src/assets/img/buy-${singleLink.img}` " alt="">
                                <p class="text-center pt-3" >{{singleLink.text}}</p>
                            </div>
                            
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
    width: 20%;
    height: 20%;
}

p{
    color: white;
}

</style>