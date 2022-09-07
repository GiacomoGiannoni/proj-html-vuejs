<template>
  <main>
    <MyOnlineMarketing />
    <MyTricks />
    <MyFeatures />
    <MyTestimonial />
    <MyPost />
  </main>
</template>

<script>
import MyOnlineMarketing from './MainComp/MyOnlineMarketing';
import MyTricks from './MainComp/MyTricks';
import MyFeatures from './MainComp/MyFeatures';
import MyTestimonial from './MainComp/MyTestimonial';
import MyPost from './MainComp/MyPost';

export default {
    name: 'MyMain',
    components: {
        MyOnlineMarketing,
        MyTricks,
        MyFeatures,
        MyTestimonial,
        MyPost
    }
}
</script>

<style lang="scss" scoped>
@import '../styles/general.scss';

main {
    
    background-color: $background-color2;
}

</style>