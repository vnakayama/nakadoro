<template>
  <v-app>
    <h1>
      {{ error.statusCode }}
    </h1>
    <p v-if="error.statusCode === 404">
      {{ pageNotFound }}
    </p>
    <p v-else>
      {{ otherError }}
    </p>
    <NuxtLink to="/">
      Home page
    </NuxtLink>
  </v-app>
</template>

<script>
export default {
  layout: 'default',
  props: {
    error: {
      type: Object,
      default: null
    }
  },
  data () {
    return {
      pageNotFound: 'Ops! Parece que não tem nada aqui...',
      otherError: 'Vish! Algo de errado não está certo...'
    }
  },
  head () {
    return {
      title: "Ops! | Nakadoro"
    }
  }
}
</script>

<style scoped>
h1 {
  font-size: 20px;
}
</style>
