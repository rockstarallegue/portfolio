<template>
  <div class="child full rounded-2 bg-orange-1 nasalization inset-font container">
    <div class="child full column rounded-2">
      <div class="child full col row container">
        <div class="child full q-pa-none row">
              <div class="col-9 text-left text-title q-pa-sm">
                Committers Box
              </div>
              <q-separator vertical></q-separator>
              <!-- MORE DROPDOWN BUTTON -->
              <div class="col text-center q-pa-sm">
                  <q-btn-dropdown
                      dense flat style="color: #404258;" size="xs" icon="more_vert"
                      class="nasalization q-px-xs inset-font"
                  >
                      <q-list>
                      <q-item clickable >
                          <q-item-section>
                          <q-item-label>Die</q-item-label>
                          </q-item-section>
                      </q-item>

                      <q-item clickable>
                          <q-item-section>
                          <q-item-label>Live forever</q-item-label>
                          </q-item-section>
                      </q-item>
                      </q-list>
                  </q-btn-dropdown>
              </div>
          </div>
      </div>
      <q-separator color="blue-grey-3"/>
      <div class="child full col container">
      </div>
      <q-separator color="blue-grey-3"/>
      <div class="child full col-6 container">
      </div>
    </div>
  </div>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'CommittersBox',
  /* setup() {
    return {
      splitterModelA: ref(70), // start at 50%
      splitterModelB: ref(50),
      insideModel: ref(70),
    };
  }, */
});
</script>
