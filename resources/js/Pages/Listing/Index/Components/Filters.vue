<template>
  <div class="mb-8 mt-4 flex flex-wrap gap-2">
    <div class="flex flex-nowrap items-center">
      <input type="text" placeholder="Price from" class="input-filter-l" /> 
      <input type="text" placeholder="Price to" class="input-filter-r" /> 
    </div>
    <div class="flex flex-nowrap items-center">
      <select class="input-filter-l">
        <option :value="null">Beds</option>
        <option v-for="m in 5" :key="m" :value="m">{{ m }}</option>
        <option>6+</option>
      </select>
      <select class="input-filter-r">
        <option :value="null">Bath</option>
        <option v-for="m in 5" :key="m" :value="m">{{ m }}</option>
        <option>6+</option>
      </select>
    </div>
    <div class="flex flex-nowrap items-center">
      <input type="text" placeholder="Area from" class="input-filter-l" /> 
      <input type="text" placeholder="Area to" class="input-filter-r" /> 
    </div>
    <button type="submit">Filter</button>
    <button type="reset">Clear</button>
  </div>
</template>
