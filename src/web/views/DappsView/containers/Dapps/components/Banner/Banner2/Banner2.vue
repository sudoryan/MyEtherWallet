<template>
  <v-carousel-item :src="img">Banner2</v-carousel-item>
</template>

<script>
import SpaceDog from '@/assets/images/backgrounds/dapps/space-dog.png';

export default {
  components: {},
  data() {
    return { img: SpaceDog };
  }
};
</script>

<style lang="scss" scoped></style>
