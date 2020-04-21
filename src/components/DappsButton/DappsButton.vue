<template>
  <div>
    <img :alt="data.name" :src="data.img" />
    <div>{{ data.name }}</div>
    <div>{{ data.description }}</div>
    <div>
      <div v-for="hashTag in data.hashTags" :key="hashTag.id">
        {{ hashTag }}
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    data: {
      default: function () {
        return {};
      },
      type: Object
    }
  },
  data() {
    return {};
  }
};
</script>
