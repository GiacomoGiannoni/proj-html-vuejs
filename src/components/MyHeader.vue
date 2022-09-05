<template>
  <header>
    <nav class="navbar">
        <div class="container justify-content-evenly">
            <img class="navbar-brand logo" src="@/assets/img/logo-2.png">
            <div class="d-flex">
                <ul>
                    <li v-for="(link, index) in links" :key="index" >
                        <a :href="link.url" :class="link.active?'active':''" >{{link.text}}</a>
                    </li>
                    <li>
                        <a href="#"><i class="search fa-solid fa-magnifying-glass"></i></a>
                        <a href="#"><i class="fa-solid fa-cart-shopping"></i></a>
                    </li>
                    <li>
                        <button type="button" class="btn btn-primary bottone">Get Started</button>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
    <MyJumbotron />
  </header>
</template>

<script>

import MyJumbotron from './MyJumbotron.vue';import '@/components/MyJumbotron.vue';

export default {
    name: 'MyHeader',
    components: {
    MyJumbotron,
},
    data() {
        return {
            links: [
                {
                    text: 'Home',
                    url: '#',
                    active: true,
                },
                {
                    text: 'About us',
                    url: '#',
                    active: false,
                },
                {
                    text: 'Feature',
                    url: '#',
                    active: false,
                },
                {
                    text: 'Testimonials',
                    url: '#',
                    active: false,
                },
                {
                    text: 'Contact US',
                    url: '#',
                    active: false,
                },

            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../styles/general.scss';
    .logo {
        height: 50px;
    }
    ul {
        display: flex;
        align-content: center;
        list-style: none;
        height: 100%;
        li{
            display: flex;
            align-items: center;
            list-style: none;
            height: 100%;
            a {
                color: $text-color8;
                text-decoration: none;
                height: 100%;
                line-height: 50px;
                margin: 0 10px;
                &.active, &:hover {
                    border-bottom: 3px solid $text-color5;
                    color: $text-color5; 
                }
                .search {
                    margin-left: 20px;
                }
            }
            
            .bottone {
                display: flex;
                align-items: center;
                justify-content: center;
                margin: 5px;
            }
        }
    }
</style>