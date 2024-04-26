<!--PERTAMA-->
<!-- <script setup>
import { reactive, ref } from 'vue'

const counter = reactive({ count: 0 })
const msg = ref('Hello World')
</script>

<template>
  <h1>{{ msg }}</h1>
  <br />
  <p>count is : {{ counter.count }}</p>
</template> -->

<!--KEDUA-->
<!-- <script setup>
import { ref } from 'vue'

const titleClass = ref('title')
const dynamicId = ref('title')
</script>

<template>
  <h1 v-bind:class="titleClass">Make me red</h1>
  <!- add dynamic class binding here -->
<!-- <h1 v-bind:id="dynamicId">Make me blue</h1>
  <!- add dynamic class binding here -->
<!-- </template> -->
<!-- 
<style>
.title {
  color: red;
}

#title {
  color: blue;
}
</style> -->

<!--KETIGA-->
<!-- <script setup>
import { ref } from 'vue'
const count = ref(0)

function increment() {
  count.value += 5
}
</script>

<template>
  <button @click="increment">count {{ count }}</button>
</template> -->

<!--KEEMPAT-->
<!-- <script setup>
import { ref } from 'vue'

const text = ref('')
</script>

<template>
  <input v-model="text" placeholder="Type Here" />
  <p>{{ text }}</p>
</template> -->

<!--KELIMA-->
<script setup>
import { ref } from 'vue'

const awesome = ref(true)
function toggle() {
  awesome.value = !awesome.value
}
</script>

<template>
  <button @click="toggle">toggle</button>
  <h1 v-if="awesome">Vue is awesome</h1>
  <h1 v-else>Oh no</h1>
</template>
