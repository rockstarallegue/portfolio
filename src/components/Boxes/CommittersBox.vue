<template>
  <div class="child full nasalization container">
    <div class="child full q-pa-none column">
      <div class="child full-width col row">
        <div class="col text-center q-pa-xs">
          <q-btn flat size="0.8em" color="grey-8" icon="draw"
                 label="COMMITTERS" class="q-pa-none q-ma-none" />
        </div>
        <q-separator vertical color="grey-6"/>
        <div class="col-1 text-center q-py-xs">
          <q-btn flat size="0.8em" color="grey-8" icon="more_vert" class="q-pa-none"/>
        </div>
        <q-separator vertical color="grey-6"/>
        <div class="col-2 text-center q-pa-xs">
          <q-btn flat size="0.8em" color="grey-8" icon="tune" class="q-pa-none"/>
        </div>
        <q-separator vertical color="grey-6"/>
        <div class="col-2 text-center q-pa-xs">
          <q-btn flat size="0.8em" color="grey-8" icon="add" class="q-pa-none"/>
        </div>
      </div>
      <q-separator horizontal color="grey-6"/>
      <div class="child full-width col-9 q-pa-sm container">
        <div class="child full bg-noise rounded-1 container">
          <div class="child full u-light-glass blue-borders rounded-1 q-pa-md container">
            <q-carousel
              v-model="slide"
              transition-prev="scale"
              transition-next="scale"
              swipeable
              animated
              control-color="orange-1"
              navigation
              arrows
              class="transparent text-orange-1 shadow-1 rounded-borders"
            >
              <q-carousel-slide name="style" class="column no-wrap flex-center">
                <q-icon name="nature_people" size="56px" />
                <div class="q-mt-md text-center">
                  {{ lorem }}
                </div>
              </q-carousel-slide>
              <q-carousel-slide name="tv" class="column no-wrap flex-center">
                <q-icon name="snowboarding" size="56px" />
                <div class="q-mt-md text-center">
                  {{ lorem }}
                </div>
              </q-carousel-slide>
              <q-carousel-slide name="layers" class="column no-wrap flex-center">
                <q-icon name="hot_tub" size="56px" />
                <div class="q-mt-md text-center">
                  {{ lorem }}
                </div>
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
  name: 'CommittersBox',
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
