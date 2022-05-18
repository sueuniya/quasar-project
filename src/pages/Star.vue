<template>
  <q-page class="star">
    <div class="">
      <q-btn-toggle
        v-model="model"
        class="my-custom-toggle q-mt-md"
        no-caps
        rounded
        bordered
        unelevated
        toggle-color="primary"
        color="white"
        text-color="primary"
        :options="[
          {label: 'Option 1', value: 'one'},
          {label: 'Option 2', value: 'two'},
          {label: 'Option 3', value: 'three'},
          {label: 'Option 4', value: 'four'}
        ]"
      />
    </div>
  </q-page>
</template>

<script>
import { ref } from 'vue'

export default {
  setup () {
    return {
      model: ref('one')
    }
  }
}
</script>

<style lang="scss" >
   .my-custom-toggle {
     border: 1px solid orange;
  }
</style>