<template>
  <q-page class="flex flex-center bg-blue-grey-8 q-pa-sm container">
      <div class="full child q-pa-none container rounded-2 shadow-2">
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
