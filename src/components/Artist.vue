<template lang="pug">
    li
      h2: a(v-bind:href="artist.url" target="_blank") {{ artist.name }}
      img(v-bind:src="artist.image[2]['#text']")
</template>

<script>
export default {
  name: 'artist',
  props: ['artist']
}
</script>

<style lang="stylus" scoped>/* scoped les agrega un data para que no se pisen los estilos entre si */
li
  diplay block
  margin 10px 0
</style>
