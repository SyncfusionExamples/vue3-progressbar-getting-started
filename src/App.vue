<template>
  <ejs-progressbar id="percentage" :type='type' :showProgressValue='showProgressValue' :value='value' :animation="animation">
  </ejs-progressbar>
</template>

<script>
import { ProgressBarComponent } from "@syncfusion/ej2-vue-progressbar";

export default {
  name: "App",
  components: {
    "ejs-progressbar": ProgressBarComponent,
  },
  data() {
    return {
      type: 'Circular',
      showProgressValue: 'true',
      value: 100,
      animation: {
        enable: true,
        duration: 2000,
        delay: 0,
      },
    };
  },
};
</script>