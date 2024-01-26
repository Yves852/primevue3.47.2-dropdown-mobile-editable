<script setup lang="ts">
// https://primevue.org/dropdown/#editable
const selectedCity = ref();
const cities = ref([
    { name: 'New York', code: 'NY' },
    { name: 'Rome', code: 'RM' },
    { name: 'London', code: 'LDN' },
    { name: 'Istanbul', code: 'IST' },
    { name: 'Paris', code: 'PRS' }
]);
</script>
<template>
  <div>
    <Dropdown
    v-model="selectedCity"
    editable
    :options="cities"
    optionLabel="name"
    placeholder="Select a City"
    class="w-full md:w-14rem" />
  </div>
</template>
