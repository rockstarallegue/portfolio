<template>
  <div class="child full rounded-2 container">
    <!--div class="q-px-xs nasalization text-grey-8">Context window</div-->
    <div class="child full bg-orange-1 blue-borders rounded-1 container">
    <div class="child full bg-static-noise rounded-1 container">
      <div class="child full blue-borders u-light-glass rounded-1 container">
        <div class="center nasalization q-px-md q-pb-lg text-orange-1">
          pathos.cloud
          <img
            alt="Quasar logo"
            src="~assets/saturn_mid.png"
            style="width: 69px; height: 69px"
          >
        </div>
      </div>
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
