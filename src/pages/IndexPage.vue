<template>
  <q-page class="flex flex-center q-pa-none bg-noise container">
      <div class="full child q-pa-sm container u-thin-glass">
        <SplitterBoard></SplitterBoard>
      </div>

  </q-page>
</template>

<script>
import { defineComponent } from 'vue';
import SplitterBoard from 'src/components/SplitterBoard.vue';

export default defineComponent({
  components: { SplitterBoard },
  name: 'IndexPage',
});
</script>
