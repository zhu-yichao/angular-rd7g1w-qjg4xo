<template>
  <a-image-preview-group :src-list="renderData" infinite>
    <a-space>
      <a-image :src="renderData[0]" width="200" />
    </a-space>
  </a-image-preview-group>
  <br />
  <a-image-preview-group>
    <a-space>
      <a-image
        src="https://p1-arco.byteimg.com/tos-cn-i-uwbnlip3yd/cd7a1aaea8e1c5e3d26fe2591e561798.png~tplv-uwbnlip3yd-webp.webp"
        width="200"
      />
    </a-space>
  </a-image-preview-group>
  <br />

  <a-image-preview-group :src-list="renderData1" infinite>
    <a-space>
      <a-image :src="renderData1[0]" width="200" />
    </a-space>
  </a-image-preview-group>
</template>
<script>
import { ref } from 'vue';

export default {
  setup() {
    const renderData = ref([]);
    const renderData1 = ref([]);
    setTimeout(() => {
      renderData.value = [
        'https://p1-arco.byteimg.com/tos-cn-i-uwbnlip3yd/cd7a1aaea8e1c5e3d26fe2591e561798.png~tplv-uwbnlip3yd-webp.webp',
        'https://p1-arco.byteimg.com/tos-cn-i-uwbnlip3yd/cd7a1aaea8e1c5e3d26fe2591e561798.png~tplv-uwbnlip3yd-webp.webp',
        'https://p1-arco.byteimg.com/tos-cn-i-uwbnlip3yd/24e0dd27418d2291b65db1b21aa62254.png~tplv-uwbnlip3yd-webp.webp',
        'https://p1-arco.byteimg.com/tos-cn-i-uwbnlip3yd/0265a04fddbd77a19602a15d9d55d797.png~tplv-uwbnlip3yd-webp.webp',
      ];
      renderData1.value = [
        'https://p1-arco.byteimg.com/tos-cn-i-uwbnlip3yd/0265a04fddbd77a19602a15d9d55d797.png~tplv-uwbnlip3yd-webp.webp',
      ];
    }, 0);
    return {
      renderData,
      renderData1,
    };
  },
};
</script>
