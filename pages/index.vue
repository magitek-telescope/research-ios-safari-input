<template>
  <section class="w-screen h-screen m-0 p-0 overflow-hidden">
    <div class="fixed pin-l pin-t w-screen h-screen opacity-75 bg-black">

    </div>
    <div class="absolute pin-l pin-b w-screen h-32 flex items-center justify-center bg-white z-10 px-8">
      <div class="w-full">
        <input type="text" class="w-full border border-b rounded h-8"><br>
        <div class="text-right mt-4">
          <button type="button" @click="handleClickButton" class="p-2 rounded bg-blue text-white">Submit</button>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  },
  methods: {
    handleClickButton() {
      alert(1)
    }
  }
}
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
  @apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
</style>
