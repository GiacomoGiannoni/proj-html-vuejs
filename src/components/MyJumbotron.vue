<template>
    <div class="container">
        <div class="row justify-content-start">
            <div class="colonna col-4">
                <h2>The Biggest platform for your growth.</h2>
                <p>There are many variations of passages of Lorem Ipsum avaible, but the majority have suffered alteration in some form</p>
                <button type="button" class="btn btn-primary bottone">Road More</button>
            </div>
            <div class="colonnadx col-4">
                <img src="@/assets/img/27-1.png" alt="img-jumbotron">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MyJumbotron',
}
</script>

<style lang="scss" scoped>
@import '../styles/general.scss';

.container {
    background-color:$background-color2;
    margin-top: 20px;
    height: 450px;

    .colonna {
        margin-left: 125px;

        h2 {
            font-size: 43px;
            margin: 30px 0px 0px 0px;
        }
        
        p {
            margin: 10px 0px 0px 0px;
            color: $text-color4;
        }
        
        .bottone {
            margin: 40px 0px 0px 0px;
        }  

        .bottone:hover {
            background-color: $background-color4;
            border-color: $background-color4;
        }
    }
    .colonnadx {
        position: relative;
        img {
            position: absolute;
            margin-top: 30px;
        }
    }
}
</style>