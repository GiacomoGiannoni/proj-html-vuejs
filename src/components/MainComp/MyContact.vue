<template>
    <main>
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-6 align-items-center">
                    <h2 class="d-flex justify-content-center">Contact with our team</h2>
                    <span class="d-flex justify-content-center first mb-3">If your are planning on developing a product landing.</span> 
                </div>
            </div>
            <div class="row justify-content-center mt-5 mb-5">
                <div class="col-4">
                    <img class="dimensioni" src="@/assets/img/StaticMapService.GetMapIma.png" alt="mappa">                
                </div>
                <div class="col-4">
                    <img class="logo-dim mb-5" src="@/assets/img/35.png" alt="logo">
                    <h5 class="mb-3">9840 Shore St.Fond Du Lac, WI 54935</h5>
                    <span class="d-block">0 1223 456 789</span>
                    <span class="d-block">mail@sofbox.com</span>
                    <div class="mt-4 mb-5">
                        <button class="btn btn-light"><i class="fa-brands fa-facebook-f blu"></i></button>
                        <button class="btn btn-light"><i class="fa-brands fa-twitter blu"></i></button>
                        <button class="btn btn-light"><i class="fa-brands fa-github blu"></i></button>
                        <button class="btn btn-light"><i class="fa-brands fa-instagram blu"></i></button>
                    </div>
                    <h4 class="mb-4">Get in touch</h4>
                    <div class="row justify-content-between MyForm">
                        <div class="col-5">
                            <input type="text" class="form-control" placeholder="Your name" aria-label="First name">
                        </div>
                        <div class="col-5 mb-3">
                            <input type="email" class="form-control" placeholder="Your email">
                        </div>
                        <div class="col-12 mb-3">
                            <input type="text" class="form-control" placeholder="Your subject" aria-label="First name">
                        </div>
                        <div class="col-12 mb-3">
                            <textarea class="form-control" id="exampleFormControlTextarea1" placeholder="Your message" rows="5"></textarea>
                        </div>
                        <div class="col-5">
                            <button class="btn btn-primary blu">Send Message</button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>
    
<script>
export default {
    name: 'MyContact',
}
</script>
    
    
<style lang="scss" scoped>
@import '@/styles/general.scss';

main {
    .container {
        margin-top: 100px;
        span {
            color: $text-color4;
        }
        .btn-light {
            background-color: $background-color1;
            border-color: $background-color5;
            margin-right: 5px;
            .blu {
                color: $text-color5;
            }
        }
        .MyForm {
            border-color: border-color2;
            .btn-primary {
                background-color: $background-color3;
            }
        }
        .dimensioni {
            width: 400px;
        }
        .logo-dim {
            width: 90px;
        }
    }
}
</style>