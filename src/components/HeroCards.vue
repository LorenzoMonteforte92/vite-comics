<script>
    export default {
        name: 'HeroCards',
        props: {
            cardContent: Object
        },
        

        data(){
            return{
                
            }
        },
        methods: {
            
            }
        }

    
</script>

<template>
    <div class="card" style="width: calc(100% / 6);">
            <div class="ms-card-img" ><img :src="cardContent.thumb" class="card-img-top" alt="..."></div>
        <div class="card-body px-0">
            <div><p class="card-text text-white">{{ cardContent.series }}</p></div>
        </div>
    </div>
</template>

<style scoped lang="scss">
    .card{
        background-color: transparent;
        border: none;
    }

    img{
        height: 100%;
        object-fit: cover;
    }
    .ms-card-img{
        height: 80%
    }
</style>