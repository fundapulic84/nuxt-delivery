<template>
  <nuxt-link :to="'/articles/' + id">
    <article>
      <div>
        <div
          class="thumbnail"
          :style="{ backgroundImage: 'url(' + thumbnail + ')' }"
        ></div>
        <h2>{{ title }}</h2>
        <p>{{ description }}</p>
      </div>
    </article>
  </nuxt-link>
</template>

<script>
export default {
  props: ['thumbnail', 'title', 'id', 'text', 'description'],
}
</script>

<style scoped>
a {
  text-decoration: none;
  color: black;
}
article {
  box-sizing: border-box;
  width: 80%;
  padding: 8px;
  border: 1px solid #ccc;
  box-shadow: 0 2px 2px #aaa;
  margin: 10px;
}
.thumbnail {
  background-position: center;
  background-size: cover;
  width: 100%;
  height: 200px;
}
</style>
