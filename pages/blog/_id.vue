<template>
<div>
  <div>blog id</div>
  <div>{{ $route.params.id }}のエントリーです。</div>
</div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
})
// export default {
//         validate({ params }) {
//         return /^\d+$/.test(params.id)
//     }
// }
</script>
