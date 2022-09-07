<template>
    <main>
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-6 align-items-center">
                    <h2 class="d-flex justify-content-center">Latest Posts</h2>
                    <span class="d-flex justify-content-center first mb-3">If your are planning on developing a product landing.</span> 
                </div>
            </div>
            <div class="row row-cols-3 justify-content-center mt-5">
                <div class="col-3">
                    <div class="card h-100" v-for="(link, index) in links" :key="index">
                        <img src="@/assets/img/19.jpg" class="card-img-top p-2 position-relative" alt="...">
                        <div class="position-absolute mt-3 ms-3 date">
                            <span>{{link.date}}</span>
                        </div>
                        <div class="card-body">
                            <h5 class="card-title">{{link.title}}</h5>
                            <p class="card-text">{{link.text}}</p>
                        </div>
                    </div>
                </div>
                <div class="col-3">
                    <div class="card h-100" v-for="(link, index) in links" :key="index">
                        <img src="@/assets/img/18.jpg" class="card-img-top p-2 position-relative" alt="...">
                        <div class="position-absolute mt-3 ms-3 date">
                            <span>{{link.date}}</span>
                        </div>
                        <div class="card-body">
                            <h5 class="card-title">{{link.title}}</h5>
                            <p class="card-text">{{link.text}}</p>
                        </div>
                    </div>
                </div>
                <div class="col-3">
                    <div class="card h-100" v-for="(link, index) in links" :key="index">
                        <img src="@/assets/img/17.jpg" class="card-img-top p-2 position-relative" alt="...">
                        <div class="position-absolute mt-3 ms-3 date">
                            <span>{{link.date}}</span>
                        </div>
                        <div class="card-body">
                            <h5 class="card-title">{{link.title}}</h5>
                            <p class="card-text">{{link.text}}</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>
    
<script>
export default {
    name: 'MyPost',
    data() {
        return {
            links: [
                {
                    title: 'Life Lack Meaining',
                    text: 'It is a long established fact that a reader will be distracted by the readable.',
                    date: 'November, 28, 2019',
                },
            ]
        }
    }
}
</script>
    
    
<style lang="scss" scoped>
@import '@/styles/general.scss';

main {
    .container {
        margin-top: 100px;
    }
    .card-text {
        color: $text-color4;
    }
    .date {
        font-size: 12px;
        border-radius: 2px;
        padding: 3px;
        color: $text-color4;
        background-color: $background-color1;
    }
}
</style>