<template>
  <section class="bg-[#98C1D9] flex items-center justify-center flex-col h-210">
    <div class="text-white text-5xl font-bold cairo-font text-center mb-10">
      <h1>{{ title }}</h1>
    </div>
    <form
      @submit.prevent="handleSubmit"
      class="bg-[#6C9CB8] text-white w-125 h-auto p-15 text-xl text-white cairo-font space-y-5"
    >
      <div v-for="(filed, index) in fileds" :Key="index" class="flex flex-col mb-5">
        <label class="mb-2">{{ filed.label }}</label>
        <input
          :type="filed.type"
          :placeholder="filed.placeholder"
          v-model="filed.value"
          class="bg-[#ffffff] w-100 h-10 rounded-md"
        />
      </div>
      <div class="bg-[#EE6C4D] w-100 h-10 rounded-md text-center p-1">
        <button type="submit">{{ buttonText }}</button>
      </div>
    </form>
  </section>
</template>
<script>
import { title } from 'process'

export default {
  props: {
    title: String,
    fileds: Array,
    buttonText: String,
  },
  data() {
    return {
      FormData: {},
    }
  },
  methods: {
    handleSubmit() {
      this.$emit('submit', this.FormData)
    },
  },
}
</script>
