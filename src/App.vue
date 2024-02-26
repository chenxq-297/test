<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
import XueQiuQueryParams from 'snowballdb-util'
// console.log(XueQiuQueryParams,'XueQiuQueryParams');
const monitorStatisticsConfig = new XueQiuQueryParams({
  "sourceType": "DATASET",
  "accessKey": "7439aacb-7b07-42c2-9299-4982cc6f4045",
  "severName": "设备监控企业统计列表（新）",
  "dataServiceId": "1201565674214227968",
  "encrypted": false,
})
console.log(monitorStatisticsConfig,'XueQiuQueryParams');

</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />
    </div>
  </header>

  <main>
    <TheWelcome />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
