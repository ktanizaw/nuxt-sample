<template>
<div>
  <div>ブログページ</div>
  <div>
  <label for="title"><input name="title" type="text"></label>
  </div>
  <div>
    <label for="test">
  <input type="checkbox"><option value="1"></option>

  </label>
  </div>
  <Button/>
  <div class="home">
    <MyCom>
      <template #name>
      谷澤健太
      </template>
    </MyCom>
    <MyCom>
      <template #address>
      蒲田
      </template>
    </MyCom>
    <MyCom v-slot:default="slotProps">
      {{ slotProps.userNm.jpName }}
    </MyCom>
    <MyCom #default="user">
      <div class="item">
        {{ user.userNm }}
      </div>
    </MyCom>
  </div>
</div>
</template>

<script lang="ts">
import MyCom from '../../components/myCom.vue'
import Vue from 'vue'

export default Vue.extend({
  components: {
    MyCom
  }
})
</script>
