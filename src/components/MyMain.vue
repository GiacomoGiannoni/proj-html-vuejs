<template>
  <main>
    <MyOnlineMarketing />
    <MyTricks />
    <MyFeatures />
    <MyTestimonial />
  </main>
</template>

<script>
import MyOnlineMarketing from './MainComp/MyOnlineMarketing';
import MyTricks from './MainComp/MyTricks';
import MyFeatures from './MainComp/MyFeatures';
import MyTestimonial from './MainComp/MyTestimonial';

export default {
    name: 'MyMain',
    components: {
        MyOnlineMarketing,
        MyTricks,
        MyFeatures,
        MyTestimonial,
    }
}
</script>

<style lang="scss">
@import '../styles/general.scss';

</style>