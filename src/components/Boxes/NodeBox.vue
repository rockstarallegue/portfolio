<template>
  <div class="child full rounded-u-l-2 nasalization container">
    <div class="child full q-pa-none rounded-2 column">
      <div class="child full-width col row container">
        <div class="child full row">
          <div class="child full text-center q-pa-none">
            <div class="child full text-center">
              <q-btn flat size="1em" round color="grey-8"
                     icon="route" label="PATH :: paths/ubsh464ry47ry48sure74" />
            </div>
          </div>
        </div>
      </div>
      <q-separator horizontal color="blue-grey-3"/>
      <div class="child full-width col-9  q-pa-sm container">
        <div class="child full bg-noise blue-borders rounded-1 container">
          <div class="child full u-light-glass rounded-1 q-pa-md container">
            <q-carousel
              v-model="slide"
              transition-prev="scale"
              transition-next="scale"
              swipeable
              animated
              control-color="orange-1"
              navigation
              arrows
              class="u-light-glass full text-orange-1 shadow-2 rounded-1"
            >
              <q-carousel-slide name="style" class="column no-wrap flex-center">
                <q-icon name="photo" size="156px" />
                <div class="q-mt-md text-center">
                  {{ lorem }}
                </div>
              </q-carousel-slide>
              <q-carousel-slide name="tv" class="column no-wrap flex-center">
                <q-icon name="music_note" size="156px" />
                <div class="q-mt-md text-center">
                  {{ lorem }}
                </div>
              </q-carousel-slide>
              <q-carousel-slide name="layers" class="column no-wrap flex-center">
                <q-icon name="play_circle" size="156px" />
                <div class="q-mt-md text-center">
                  {{ lorem }}
                </div>
              </q-carousel-slide>
              <q-carousel-slide name="read" class="column no-wrap flex-center">
                <q-icon name="menu_book" size="156px" />
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
import { ref, defineComponent } from 'vue';

export default defineComponent({
  name: 'NodeBox',
  setup() {
    return {
      slide: ref('style'),
      lorem: 'Insanus Contentus',
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
