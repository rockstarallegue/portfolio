<template>
  <div class="child full nasalization container">
    <div class="child full q-pa-none column">
      <div class="child full-width col row">
        <div class="col text-center q-pa-xs">
          <q-btn flat size="0.8em" color="grey-8" icon="label"
                 label="LABELS" class="q-pa-none q-ma-none" />
        </div>
        <q-separator vertical color="blue-grey-3"/>
        <div class="col-1 text-center q-py-xs">
          <q-btn flat size="0.8em" color="grey-8" icon="more_vert" class="q-pa-none"/>
        </div>
        <q-separator vertical color="blue-grey-3"/>
        <div class="col-2 text-center q-pa-xs">
          <q-btn flat size="0.8em" color="grey-8" icon="tune" class="q-pa-none"/>
        </div>
        <q-separator vertical color="blue-grey-3"/>
        <div class="col-2 text-center q-pa-xs">
          <q-btn flat size="0.8em" color="grey-8" icon="add" class="q-pa-none"/>
        </div>
      </div>
      <q-separator horizontal color="blue-grey-3"/>
      <div class="child full-width col-9 q-pa-sm container">
        <div class="child full bg-noise blue-borders rounded-1 container">
          <div class="child full u-light-glass rounded-1 q-pa-md container">
            <q-carousel
              v-model="slide"
              vertical
              transition-prev="slide-down"
              transition-next="slide-up"
              swipeable
              animated
              control-color="orange-1"
              navigation
              arrows
              class="transparent text-orange-1 shadow-1 rounded-borders"
            >
              <q-carousel-slide name="style" class="column no-wrap flex-center">
                <q-icon name="pin" size="56px" />
              </q-carousel-slide>
              <q-carousel-slide name="layers" class="column no-wrap flex-center">
                <q-icon name="label" size="56px" />
              </q-carousel-slide>
            </q-carousel>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { defineComponent, ref } from 'vue';

export default defineComponent({
  name: 'TagsBox',
  setup() {
    return {
      slide: ref('style'),
      lorem: 'Arcanum Ens',
    };
  },
  /* setup() {
    return {
      splitterModelA: ref(70), // start at 50%
      splitterModelB: ref(50),
      insideModel: ref(70),
    };
  }, */
});
</script>
