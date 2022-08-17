<template>
  <div class="custom-item">
    <DxTextBox
      :value="fieldData && fieldData.Name"
      :read-only="true"
      class="product-name"
    />
  </div>
</template>
<script>
import DxTextBox from "devextreme-vue/text-box";

export default {
  components: {
    DxTextBox,
  },
  props: {
    fieldData: {
      type: Object,
      default: () => {},
    },
  },
};
</script>