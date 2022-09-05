<template>
  <main>
    <MyOnlineMarketing />
    <MyTricks />
  </main>
</template>

<script>
import MyOnlineMarketing from './MainComp/MyOnlineMarketing';
import MyTricks from './MainComp/MyTricks';

export default {
    name: 'MyMain',
    components: {
    MyOnlineMarketing,
    MyTricks
    }
}
</script>

<style lang="scss">
@import '../styles/general.scss';

</style>