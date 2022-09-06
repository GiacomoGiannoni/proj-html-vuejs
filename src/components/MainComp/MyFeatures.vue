<template>
    <main>
        <div class="container">
            <div class="row justify-content-center align-items-center">
                <div class="col-8 g-0">
                    <div class="row justify-content-between align-items-center">
                        <div class="col-8">
                            <h3>Popular features that your business needs</h3>
                            <p>Faff about only a quid blower i don't want no agro bleeding chimney <br>pot burke tosser cras nione boot fanny.!</p>
                        </div>
                        <div class="col-3">
                            <button class="btn btn-primary">Explore more Feature</button>
                        </div>
                    </div>
                    <div class="row row_cards row-cols-4 justify-content-center">
                        <div :id="link.contenuto" class="cards d-inline col" v-for="(link, index) in links" :key="index" >
                            <h6 :href="link.url" :class="link.active?'active':''" >{{link.text}}</h6>
                            <i :class="link.classe"></i>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>
    
<script>
export default {
    name: 'MyFeatures',
    data() {
        return {
            links: [
                {
                    contenuto: 'contentBlu',
                    text: 'Customized invoices',
                    url: '#',
                    classe: 'fa-solid fa-chart-line blu',
                    active: true,
                },
                {
                    contenuto: 'contentOrange',
                    text: 'Stock Management',
                    url: '#',
                    classe: 'fa-regular fa-paper-plane orange',
                    active: false,
                },
                {
                    contenuto: 'contentGreen',
                    text: 'Receivable & Payables',
                    url: '#',
                    classe: 'fa-solid fa-user-graduate green',
                    active: false,
                },
                {
                    contenuto: 'contentBlu',
                    text: 'Manage Buying',
                    url: '#',
                    classe: 'fa-solid fa-user-check blu',
                    active: false,
                },
                {
                    contenuto: 'contentOrange',
                    text: 'Powerful & Secure',
                    url: '#',
                    classe: 'fa-solid fa-shield-halved orange',
                    active: false,
                },
                {
                    contenuto: 'contentGreen',
                    text: 'Fastest Return Filing',
                    url: '#',
                    classe: 'fa-solid fa-user-graduate green',
                    active: false,
                },
                {
                    contenuto: 'contentBlu',
                    text: 'Monthly Detailed',
                    url: '#',
                    classe: 'fa-solid fa-file-pen blu',
                    active: false,
                },
                {
                    contenuto: 'contentOrange',
                    text: 'Product Management',
                    url: '#',
                    classe: 'fa-solid fa-list-check orange',
                    active: false,
                }
            ]
        }
    }
}
</script>
    
<style lang="scss" scoped>
@import '@/styles/general.scss';

main {
    background: url("@/assets/img/14.png") no-repeat -50%;
    margin-top: 100px;
    .container {
        margin-top: 100px;
        p {
            margin-top: 20px;
            color: $text-color4;
        }
        .row_cards {
            margin-top:20px;
            .cards {
                width: calc(100% / 4 - 20px);
                margin-left: 20px;
                margin-bottom: 30px;
                padding: 30px;
                box-shadow: 5px 5px 10px 5px $border-color7;
                background-color: $background-color1;
                i {
                    display: block;
                    margin-top: 20px;
                    font-size: 30px;
                };
                .blu {
                    color: $text-color5;
                };
                .orange {
                    color: $text-color3;
                };
                .green {
                    color: $text-color2;
                }
            };
            #contentBlu:hover {
                color: $text-color1;
                box-shadow: 5px 5px 10px 5px  $border-color3;
                background-color: $background-color3;
                .blu {
                    color: $text-color1;
                };
            };
            #contentGreen:hover {
                color: $text-color1;
                box-shadow: 5px 5px 10px 5px  $text-color2;
                background-color: $text-color2;
                .green {
                    color: $text-color1;
                };
            };
            #contentOrange:hover {
                color: $text-color1;
                box-shadow: 5px 5px 10px 5px  $text-color3;
                background-color: $text-color3;
                .orange {
                    color: $text-color1;
                };
            }
        }
    }
}
   
</style>