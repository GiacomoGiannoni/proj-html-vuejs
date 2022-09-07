<template>
  <main>
    <MyOnlineMarketing />
    <MyTricks />
    <MyFeatures />
    <div>
        <MyTestimonial />
        <MyPost />
        <MyContact />
    </div>
  </main>
</template>

<script>
import MyOnlineMarketing from './MainComp/MyOnlineMarketing';
import MyTricks from './MainComp/MyTricks';
import MyFeatures from './MainComp/MyFeatures';
import MyTestimonial from './MainComp/MyTestimonial';
import MyPost from './MainComp/MyPost';
import MyContact from './MainComp/MyContact';

export default {
    name: 'MyMain',
    components: {
        MyOnlineMarketing,
        MyTricks,
        MyFeatures,
        MyTestimonial,
        MyPost,
        MyContact,
    }
}
</script>

<style lang="scss" scoped>
@import '../styles/general.scss';

div {  
    background: linear-gradient(to bottom, #f2f7ff 0%, #ffffff 100%);
}

</style>