<template>
  <div class="custom-item">
    <DxTextArea
      :inputAttr="{
        wrap: 'off',
        rows: '1',
        style: 'white-space: nowrap;',
      }"
      :value="fieldData && fieldData.Name"
      :read-only="true"
      class="product-name"
    />
  </div>
</template>
<script>
import DxTextArea from "devextreme-vue/text-area";

export default {
  components: {
    DxTextArea,
  },
  props: {
    fieldData: {
      type: Object,
      default: () => {},
    },
  },
};
</script>