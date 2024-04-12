<script>
    import HeroCards from './HeroCards.vue';
    export default {
        name: 'AppHero',
        
        components: {
            HeroCards
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
    <section>
        <div class="container">
            <div class="row">
                <div class="col-12 text-white">
                    <HeroCards></HeroCards>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
    @use '../style/partials/variables' as *;

    section{
        background-color: #1C1C1C;
    }


    // togliere
    .container{
        height: 150px;
    }
</style>