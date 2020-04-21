<template>
  <div>
    <v-carousel hide-delimiters>
      <Banner1 />
      <Banner2 />
    </v-carousel>
  </div>
</template>

<script>
import Banner1 from './Banner1';
import Banner2 from './Banner2';

export default {
  components: { Banner1, Banner2 },
  data() {
    return {};
  }
};
</script>

<style lang="scss" scoped></style>
