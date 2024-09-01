<template>
  <div class="child full bg-blue-grey-8 rounded-2 container">
    <div class="child full bg-cloudy rounded-2 blue-borders container">
      <div class="center blue-borders nasalization text-orange-1">
        pathos.cloud
        <img
          alt="Quasar logo"
          src="~assets/saturn_mid.png"
          style="width: 69px; height: 69px"
        >
      </div>
    </div>
  </div>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'ContextContainer',
  /* setup() {
    return {
      splitterModelA: ref(70), // start at 50%
      splitterModelB: ref(50),
      insideModel: ref(70),
    };
  }, */
});
</script>
