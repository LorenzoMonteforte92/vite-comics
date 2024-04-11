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
            makeItemActive (clickedItem) {
                this.links[clickedItem].active = !this.links[clickedItem].active
            }
            }
        }

    //fare che la barra blu sia sotto il link

    //fare che la classe active torni falsa dopo il click su un'altro elemento 
</script>

<template>
    <header>
        <div class="container">
            <div class="row py-2">
                <div class="col-3">
                    <img src="../assets/img/dc-logo.png" alt="DC comics logo">
                </div>
                <div class="col-9 d-flex justify-content-center align-items-center">
                    <nav>
                        <ul class="m-0 d-flex justify-content-center align-items-center gap-4 pt-3" >
                            <li v-for="singleLink, index in links"
                            class="ms-height-max"
                            :class="{ 'active-element' : singleLink.active}"
                            @click="makeItemActive(index)"
                            >
                                <a href="#">{{ singleLink.text }}</a>
                            </li>
                        </ul>
                    </nav>
                </div>
            </div>
        </div>
    </header>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;
    a {
        color: $brand-secondary-color;
    }

    .active-element{
        
        border-bottom: solid 5px #0282F9;
            a{
                color: #0282F9;
            }
    }
</style>