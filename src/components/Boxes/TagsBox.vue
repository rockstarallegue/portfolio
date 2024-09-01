<template>
  <div class="child full rounded-2 anti-cake-grad nasalization blue-borders inset-font container">
    <div class="child full q-pa-none rounded-2 blue-borders column">
      <div class="child full-width col row light-glass rounded-u-2">
        <div class="col text-center q-pa-xs">
          <q-btn flat size="0.8em" color="blue-grey-8" icon="label"
                 label="ALL TAGS" class="q-pa-none q-ma-none"/>
        </div>
        <q-separator vertical color="blue-grey-3"/>
        <div class="col-1 text-center q-py-xs">
          <q-btn flat size="0.8em" color="blue-grey-8" icon="more_vert" class="q-pa-none"/>
        </div>
        <q-separator vertical color="blue-grey-3"/>
        <div class="col-2 text-center q-pa-xs">
          <q-btn flat size="0.8em" color="blue-grey-8" icon="tune" class="q-pa-none"/>
        </div>
        <q-separator vertical color="blue-grey-3"/>
        <div class="col-2 text-center q-pa-xs">
          <q-btn flat size="0.8em" color="blue-grey-8" icon="add" class="q-pa-none"/>
        </div>
      </div>
      <q-separator horizontal color="blue-grey-3"/>
      <div class="child full-width col-9 light-glass q-pa-sm rounded-b-2 container">
        <div class="child full bg-blue-grey-1 blue-borders rounded-2"></div>
      </div>
    </div>
  </div>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'TagsBox',
  /* setup() {
    return {
      splitterModelA: ref(70), // start at 50%
      splitterModelB: ref(50),
      insideModel: ref(70),
    };
  }, */
});
</script>
