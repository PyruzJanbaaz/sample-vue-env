<template>
  <div class="hello">
    <h2>{{ url }}</h2>
  </div>
</template>

<script>
export default {
  name: 'HelloEnv',
  data() {
    return {
      url: process.env.VUE_APP_ROOT_API
    }
  }
}
</script>

