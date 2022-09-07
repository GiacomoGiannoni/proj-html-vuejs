<template>
    <main>
        <div class="container">
          <div class="d-flex justify-content-center">
              <div>
                  <img src="@/assets/img/24.png" alt="imgMain1">
              </div>
              <div>
                  <h5>Online Marketing</h5>
                  <p>It is a long established fact that a <br> reader will be distracted.</p>
                  <ul>
                      <li v-for="(link, index) in links" :key="index">
                          <span>{{link.text}}</span>
                      </li>
                  </ul>
              </div>
              <div>
                  <img src="@/assets/img/24.png" alt="imgMain1">
              </div>
              <div>
                  <h5>Online Marketing</h5>
                  <p>It is a long established fact that a <br> reader will be distracted.</p>
                  <ul>
                      <li v-for="(link, index) in links" :key="index">
                          <span>{{link.text}}</span>
                      </li>
                  </ul>
              </div>
              <div>
                  <img src="@/assets/img/24.png" alt="imgMain1">
              </div>
              <div>
                  <h5>Online Marketing</h5>
                  <p>It is a long established fact that a <br> reader will be distracted.</p>
                  <ul>
                      <li v-for="(link, index) in links" :key="index">
                          <span>{{link.text}}</span>
                      </li>
                  </ul>
              </div>
          </div>
      </div>
    </main>
</template>

<script>
export default {
    name: 'MyOnlineMarketing',
    data() {
        return {
            links: [
                {
                    text: 'SEO',
                },
                {
                    text: 'SEM',
                },
                {
                    text: 'Website Strategy',
                },
                {
                    text: 'Social Management',
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '@/styles/general.scss';
main { 
    background-color: $background-color1!important;
    .container {
        margin-top: 100px;
        img {
            width: 50px;
            margin: 0px 20px;
        };
        p {
            color: $text-color4;
        };
        ul {
            list-style-type: "\2713";
            margin-left: 10px;
            padding-left: 0px;
            color: $text-color5;
            font-weight: bold;
            span {
                margin-left: 10px;
                color: $text-color8;
                font-weight: bold;
                font-size: 12px;
            }
        }
    }
}

</style>