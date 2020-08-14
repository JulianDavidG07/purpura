<template>
  <div>
    <button class="button" @click="isOpen = !isOpen">Add {{ $data }}</button>
    <div class="modal" v-if="isOpen" @close="isOpen = false">
      Jajaja
    </div>
  </div>
</template>

<script scoped>
export default {
  name: "MenuBurger",
  data() {
    return {
      isOpen: true,
    };
  },
  methods: {
    toggle() {
      this.isOpen = !this.isOpen;
    },
  },
};
</script>

<style scoped>
.button {
  position: absolute;
  z-index: 40;
}
.modal {
  position: absolute;
  z-index: 45;
}
</style>
