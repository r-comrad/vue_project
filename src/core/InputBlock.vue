<script setup>
import { ref } from "vue";

defineProps(['name'])

const text = ref("");

const emit = defineEmits(['textUpdated'])

function returnText() {
  emit('textUpdated', text.value)
}

// emit('enlarge-text')

</script>


<template>
    <!-- <input v-model="value" :placeholder="name"> -->

    <input class="sss" v-model="text" :placeholder="name" @input="returnText">
    <br>
    <!-- <p>{{text}}</p> -->
    <!-- <label></label> -->

    <!-- <label for="username" class="form-label">{{ text }}</label> -->
    <!-- <input type="text" name="username" id="username" class="form-control" v-model="username"> -->
</template>

<style scoped>

.sss {
  display: block;
  margin: 0 auto 2rem;
}

</style>
