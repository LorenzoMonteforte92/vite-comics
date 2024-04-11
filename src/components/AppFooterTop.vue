<script>
    export default {
        name: 'AppFooterTop',

        data(){
            return{
                
            }
        },
        methods: {
            
            }
        }

    
</script>

<template>
    <footer class="overflow-hidden position-relative" >
        <div class="container">
            <div class="row">
                <div class="col-4 d-flex flex-wrap gap-5 pt-5">
                    <div>
                        <h4>DC COMICS</h4>
                    </div>
                    <div>
                        <h4>DC</h4>
                    </div>
                    <div>
                        <h4>DC SITES</h4>
                    </div>
                    <div>
                        <h4>SHOP</h4>
                    </div>
                </div>
            </div>
        </div>
        <img class="position-absolute" src="../assets/img/dc-logo-bg.png" alt="">
    </footer>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;

footer{
    background-image: url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    height: 500px;
        h4{
            color: white;
        }
}

// .col-8{
//     background-image: url('../assets/img/dc-logo-bg.png');
//     background-repeat: no-repeat;
//     background-size: cover;
// }

img{
    right: 0px;
    transform: scale(1.4);
    top: -7%;
}

</style>