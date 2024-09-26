<template>
  <div class="child full column nasalization container">
    <div class="child full col q-px-sm q-pt-xs container center">
      <q-btn-group flat push
        class="child rounded-b-l-1 full-width bg-orange-1 text-grey-8 q-pa-none">
        <q-btn push class="blue-borders q-pb-xs full-width"
          size="xs" icon="label" label="LABELS"/>
        <q-btn push class="blue-borders q-px-xs q-pb-sm" icon="add" size="xs" />
        <q-btn push class="blue-borders q-px-xs q-pb-sm" icon="tune" size="xs" />
        <q-btn push class="blue-borders q-px-xs q-pb-sm" icon="more_vert" size="xs" />
      </q-btn-group>
    </div>
    <div class="child full col-9 q-pa-none">
      <div class="child full container">
        <div class="child full container">
          <q-carousel
            dense
            v-model="slide"
            transition-prev="scale"
            transition-next="scale"
            swipeable
            animated
            control-color="grey-8"
            navigation
            vertical
            arrows
            class="full q-pa-xl transparent"
          >
          <q-carousel-slide name="style"
              class="column no-wrap q-pa-none bg-orange-1 rounded-66 blue-borders flex-center">
              <div class="column full thick-glass
                no-wrap rounded-66 q-pa-none flex-center text-grey-8">
                <q-icon name="nature_people" size="36px" />
                <div class="q-mt-md text-center">
                  {{ lorem }}
                </div>
              </div>
            </q-carousel-slide>
            <q-carousel-slide name="tv"
              class="column no-wrap q-pa-none bg-orange-1 rounded-66 blue-borders flex-center">
              <div class="column full thick-glass
                no-wrap rounded-66 q-pa-none flex-center text-grey-8">
                <q-icon name="nature_people" size="36px" />
                <div class="q-mt-md text-center">
                  {{ lorem }}
                </div>
              </div>
            </q-carousel-slide>
            <q-carousel-slide name="telephone"
              class="column no-wrap q-pa-none bg-orange-1 rounded-66 blue-borders flex-center">
              <div class="column full thick-glass
                no-wrap rounded-66 q-pa-none flex-center text-grey-8">
                <q-icon name="nature_people" size="36px" />
                <div class="q-mt-md text-center">
                  {{ lorem }}
                </div>
              </div>
            </q-carousel-slide>
          </q-carousel>
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
