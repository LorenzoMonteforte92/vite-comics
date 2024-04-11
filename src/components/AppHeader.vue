<script>
    export default {
        name: 'AppHeader',

        data(){
            return{
                links:[
                    {
                        text: `CHARACTERS`,
                        active: false
                    },
                    {
                        text: `COMICS`,
                        active: false
                    },
                    {
                        text: `MOVIES`,
                        active: false
                    },
                    {
                        text: `TV`,
                        active: false
                    },
                    {
                        text: `GAMES`,
                        active: false
                    },
                    {
                        text: `COLLECTIBLES`,
                        active: false
                    },
                    {
                        text: `VIDEOS`,
                        active: false
                    },
                    {
                        text: `FANS`,
                        active: false
                    },
                    {
                        text: `NEWS`,
                        active: false
                    },
                    {
                        text: `SHOP`,
                        active: false
                    },
                ]
            }
        },
        methods: {
            
            }
        }

    
</script>

<template>
    <div class="row justify-content-between">
        <div class="col-2"></div>
        <div class="col-7">
        <nav>
            <ul>
                <li><a href="#">ciao</a></li>
                <li><a href="#">ciao</a></li>
            </ul>
        </nav>
    </div>
    </div>
</template>

<style scoped lang="scss">
    @use '../partials/variables';
    a {
        color: $brand-secondary-color;
    }
</style>