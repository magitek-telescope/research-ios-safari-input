<template>
  <section class="w-full h-full m-0 p-0 overflow-hidden" style="box-sizing: content-box;" :class="{
    'pb-64': active
  }">
    <div class="fixed pin-l pin-t w-screen h-screen opacity-75 bg-black">

    </div>
    <div class="w-full h-full flex items-end">
      <div class="w-full h-48 flex items-center justify-center bg-white z-10 px-8" style="transform: translate(0px)">
        <div class="w-full">
          <input type="text" @focus="active = true" @blur="active = false" class="w-full border border-b rounded text-xl h-16"><br>
          <div class="text-right mt-4">
            <button type="button" @click="handleClickButton" class="p-2 rounded bg-blue text-white">Submit</button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  data() {
    return {
      active: false
    }
  },
  methods: {
    handleClickButton() {
      alert(1)
    }
  }
}
</script>

<style>
.pb-64 {
  padding-bottom: 16rem;
}
</style>
