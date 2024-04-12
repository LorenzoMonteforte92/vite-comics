<script>
    export default {
        name: 'AppFooterTop',

        data(){
            return{
               dcComicsLinks: [
                    {
                        text:'Characters' 
                    },
                    {
                        text:'Comix'
                    },
                    {
                        text:'Movies'
                    },
                    {
                        text:'TV'
                    },
                    {
                        text:'Games'
                    },
                    {
                        text:'Videos'
                    },
                    {
                        text:'News'
                    },
               ],
               
               dcLinks: [
                    {
                        text:'Terms Of Use' 
                    },
                    {
                        text:'Privacy policy (New)'
                    },
                    {
                        text:'Ad Choices'
                    },
                    {
                        text:'Advertising'
                    },
                    {
                        text:'Jobs'
                    },
                    {
                        text:'Subscriptions'
                    },
                    {
                        text:'Talent Workshops'
                    },
                    {
                        text:'CPSC Certificates'
                    },
                    {
                        text:'Ratings'
                    },
                    {
                        text:'Shop Help'
                    },
                    {
                        text:'Contact Us'
                    },
               ],

               siteLinks: [
                    {
                        text:'DC' 
                    },
                    {
                        text:'MAD Magazine'
                    },
                    {
                        text:'DC Kids'
                    },
                    {
                        text:'DC Universe'
                    },
                    {
                        text:'DC Power Visa'
                    },
               ],

               shopLinks: [
                    {
                        text:'Shop DC' 
                    },
                    {
                        text:'Shop DC Collectables'
                    },
               ],
            }
        },
        methods: {
            
            }
        }

    
</script>

<template>
    <section >
        <div class="container">
            <div class="row pt-5">
                <div class="col-2">
                    <div>
                        <h4>DC COMICS</h4>
                        <ul>
                            <li v-for="singleLink in dcComicsLinks">
                            <a href="#">{{ singleLink.text }}</a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <h4>SHOP</h4>
                        <ul>
                            <li v-for="singleLink in shopLinks">
                            <a href="#">{{ singleLink.text }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="col-2">
                    <div>
                        <h4>DC</h4>
                        <ul>
                            <li v-for="singleLink in dcLinks">
                            <a href="#">{{ singleLink.text }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="col-2">
                    <div>
                        <h4>SITES</h4>
                        <ul>
                            <li v-for="singleLink in siteLinks">
                            <a href="#">{{ singleLink.text }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;

section{
    background-image: url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    height: 500px;
        
        h4{
            color: white;
        }
}

ul{
    padding: 0;

    li{
        padding-bottom: 5px;
    }

    a {
    color: #959595;
    }
}

.container{
    background-image: url('../assets/img/dc-logo-bg.png');
    background-repeat: no-repeat;
    background-position: 100%;
    height: 100%;
}

</style>