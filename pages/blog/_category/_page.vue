<template>
    <div>
        <div>{{ $route.params.category }}カテゴリーの</div>
        <div>{{ $route.params.page }}ページ目です。</div>
    </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>
