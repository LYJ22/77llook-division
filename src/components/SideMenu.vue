<script setup>
const props = defineProps(['name'])
const emit = defineEmits(['menuSelect'])

function buttonClick() {
  emit('menuSelect', props.name)
}
</script>

<template>
  <button @click="buttonClick" class="basic-theme alfa-slab-one-regular side-menu-button">
    {{ props.name }}
  </button>
</template>
