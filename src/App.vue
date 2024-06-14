<script setup>
const checked = true;
</script>

<template>
  <div class="p-6 flex gap-4 flex-wrap">
    <a-button type="primary" class="my-button">Primary Button</a-button>
    <a-checkbox class="my-checkbox" v-model:checked="checked"></a-checkbox>
    <a-select
      class="my-select"
      ref="select"
      v-model:value="value1"
      style="width: 120px"
      @focus="focus"
      @change="handleChange"
    >
      <a-select-option value="jack">Jack</a-select-option>
      <a-select-option value="lucy">Lucy</a-select-option>
      <a-select-option value="disabled" disabled>Disabled</a-select-option>
      <a-select-option value="Yiminghe">yiminghe</a-select-option>
    </a-select>
  </div>
</template>
