<template>
  <div class="rating">
    <span v-for="i in maxStars" :key="i" @click="setRating(i)" :class="{ 'filled': i <= rating }">&#9733;</span>
  </div>
</template>

<script>
export default {
  props: {
    value: {
      type: Number,
      default: 0
    },
    maxStars: {
      type: Number,
      default: 5
    }
  },
  data() {
    return {
      rating: this.value
    };
  },
  methods: {
    setRating(stars) {
      this.rating = stars;
      this.$emit('input', stars);
    }
  }
};
</script>

<style scoped>
.rating {
  font-size: 24px;
  color: white; /* Thiết lập màu chữ tương tự như 'color="white"' trong <v-rating> */
}

.filled {
  color: #fed136;
}
</style>