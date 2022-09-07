<template>
    <footer>
        <hr>
        <div class="container mt-5 position-relative mb-4">
            <div class="row justify-content-center">
                <div class="col-8">
                    <div class="row justify-content-around align-items-baseline">
                        <div class="col-3">
                            <img class="logo-dim mb-2" src="@/assets/img/35.png" alt="logo">
                            <p class="mb-5">It is a long estabilished fact that a reader will be distracted by the readable content.</p>
                            <p>Copyright @ 2018 <a href="#">Sofbox</a></p>
                        </div>
                        <div id="lista" class="col-3">
                            <ul v-for="(link, index) in links" :key="index">
                                <li>
                                    <h6>{{link.title}}</h6>
                                </li>
                                <li>
                                    <a>{{link.text1}}</a>
                                </li>
                                <li>
                                    <a>{{link.text2}}</a>
                                </li>
                                <li>
                                    <a>{{link.text3}}</a>
                                </li>
                                <li>
                                    <a>{{link.text4}}</a>
                                </li>
                                <li>
                                    <a>{{link.text5}}</a>
                                </li>
                            </ul>
                        </div>
                        <div id="lista" class="col-3">
                            <ul v-for="(link, index) in links2" :key="index">
                                <li>
                                    <h6>{{link.title}}</h6>
                                </li>
                                <li>
                                    <a>{{link.text1}}</a>
                                </li>
                                <li>
                                    <a>{{link.text2}}</a>
                                </li>
                                <li>
                                    <a>{{link.text3}}</a>
                                </li>
                                <li>
                                    <a>{{link.text4}}</a>
                                </li>
                                <li>
                                    <a>{{link.text5}}</a>
                                </li>
                            </ul>
                        </div>
                        <div id="lista" class="col-3">
                            <ul v-for="(link, index) in links3" :key="index">
                                <li>
                                    <h6>{{link.title}}</h6>
                                </li>
                                <li>
                                    <a>{{link.text1}}</a>
                                </li>
                                <li>
                                    <a>{{link.text2}}</a>
                                </li>
                                <li>
                                    <a>{{link.text3}}</a>
                                </li>
                                <li>
                                    <a>{{link.text4}}</a>
                                </li>
                                <li>
                                    <a>{{link.text5}}</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
            <div class="position-absolute bottom-0 end-0">
                <a href="#"><i class="fa-solid fa-chevron-up arrow"></i></a>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'MyFooter',
    data() {
        return {
            links: [
                {
                    title: 'Menu',
                    text1: 'About Us',
                    text2: 'Theme',
                    text3: 'Features',
                    text4: 'Pricing',
                    text5: 'Blog',
                },
            ],
            links2: [
                {
                    title: 'About Us',
                    text1: 'About Sofbox',
                    text2: 'Roadmap',
                    text3: 'How it work',
                    text4: 'Team',
                    text5: 'News',
                }
            ],
            links3: [
                {
                    title: 'Quick Links',
                    text1: 'About us',
                    text2: 'Theme',
                    text3: 'Features',
                    text4: 'Pricing',
                    text5: 'Blog',
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '@/styles/general.scss';

footer {
    background-color: $background-color1;
    hr {
        margin-top: 100px;
    }
    .logo-dim {
        width: 90px;
    }
    p {
        color: $text-color4;
        a {
            color: $text-color5;
            text-decoration: none;
        }
    }
    #lista {
        ul {
            list-style: none;
            a {
                color: $text-color4;
                text-decoration: none;
            }
        }
    }
    .arrow {
        background-color: $text-color4;
        color: $text-color1;
        padding: 10px;
        border-radius:50%;
        text-decoration: none;
    }
}
</style>