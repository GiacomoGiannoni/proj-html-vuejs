<template>
  <main>
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-4">
          <h3>Get tips tricks on how to skyrocket your sales</h3>
          <p>faff about only a quid blower i don't want no agro bleeding chimney pot burke tosser cras nice one boot fanny.!</p>
          <div class="row ombra">
            <div class="col_img col-2">
              <img src="@/assets/img/510.png" alt="">
            </div>
            <div class="col_text col-9">
              <h6>Reporting Analysis</h6>
              <p>It is a long estabilished fact that a reader will be distracted by the readable content a page when looking at its layout.</p>
            </div>
          </div>
          <div class="row ombra">
            <div class="col_img col-2">
              <img src="@/assets/img/511.png" alt="">
            </div>
            <div class="col_text col-9">
              <h6>Reporting Analysis</h6>
              <p>It is a long estabilished fact that a reader will be distracted by the readable content a page when looking at its layout.</p>
            </div>
          </div>
        </div>
        <div class="col-4">
          <img src="@/assets/img/509.jpeg" alt="trick-img">
        </div>
      </div>
    </div>
  </main>
</template>
  
<script>
export default {
    name: 'MyTricks',
  }
</script>
  
<style lang="scss" scoped>
@import '@/styles/general.scss';
main {
  background-color: $background-color1!important;
  padding: 100px;
  .container {
    p {
      color: $text-color4;
      margin-top:20px;
    };
    .row {
      margin-top:20px;
      .ombra:hover {
        box-shadow: 5px 10px 10px $border-color7;
        h6 {
          color: $text-color5;
        }
      }
      .col_img {
        padding: 10px;
      };
      .col_text {
        margin-left: 10px;
      }
    }
  }
}
  
</style>