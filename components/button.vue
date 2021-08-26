<template>
<button
@click="sendAlert()"
>
ボタン
</button>
</template>
<script>

export default ({
  setup() {
    const sendAlert = () => {
      alert('Hello! Nuxt.js!!')
    }

    return {
      sendAlert
    }
  },
})
</script>


<style>
</style>
