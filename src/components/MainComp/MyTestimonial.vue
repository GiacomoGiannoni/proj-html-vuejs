<template>
    <main>
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-6 align-items-center">
                    <h2 class="d-flex justify-content-center">Our Testimonials</h2>
                    <span class="d-flex justify-content-center first">If your are planning on developing a product landing app or website,</span> 
                    <span class="d-flex justify-content-center">tacke a look at this beautiful-crafted</span>
                </div>
            </div>
            <div class="row row-cols-2 g-4 justify-content-center ">
                <div class="col-4">
                    <div class="cards text-center">
                        <img src="@/assets/img/26.jpeg" class="image m-3" alt="Julia-Aann-img">
                        <div>
                            <h5 class="m-3">Julia Aann</h5>
                            <span>-  COO Sofbox</span>
                            <p class="m-3">At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur accus adip adip.</p>
                        </div>
                    </div>
                </div>
                <div class="col-4">
                    <div class="cards text-center">
                        <img src="@/assets/img/27.jpeg" class="image m-3" alt="Mac-Znder-img">
                        <div>
                            <h5 class="m-3">Mac Znder</h5>
                            <span>-  Manager Sofbox</span>
                            <p class="m-3">At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur accus adip adip.</p>
                        </div>
                    </div>
                </div>
            </div>
            <div id="dot" class="me-3">
                <span id="colore">.</span>
                <span>.</span>
            </div>
        </div>
    </main>
</template>
    
<script>
export default {
    name: 'MyTestimonial',
}
</script>
    
    
<style lang="scss" scoped>
@import '@/styles/general.scss';

main {
    background: url("@/assets/img/15.png") no-repeat left top;
    .container {
        span {
            color: $text-color4;
        }
        .first {
            margin-top: 20px;
        }
        .cards {
            margin-top: 100px;
            width: 400px;
            height: 300px;
            background-color: $background-color1;
            background-image: url('@/assets/img/quote.png') $background-color5;
            background-size: contain;
            background-repeat: no-repeat;
            background-position: center;
            background-size: 200px;
            border-radius: 10px;
            box-shadow: 1px 1px 10px $border-color4;
            h5 {
                display: inline-block;
            };
            span {
                color: $text-color4;
                font-size: 13px;
            };
            p {
                color: $text-color4;
            }
            .image {
                width: 80px;
                margin: auto;
                border: 1px solid $border-color1;
                border-radius: 50%;
            };
        }
    }
    #dot {
        display: flex;
        justify-content: center;
        align-content: center;
        span {
            font-size: 80px;
            color: $text-color8;
        };
        #colore {
            color: $text-color5;
        }
    }
};
</style>