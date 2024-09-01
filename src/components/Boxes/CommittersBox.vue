<template>
  <div class="child full rounded-2 anti-surface nasalization blue-borders inset-font container">
    <div class="child full q-pa-none rounded-2 blue-borders column">
      <div class="child full-width col row light-glass rounded-u-2">
        <div class="col text-center q-pa-xs">
          <q-btn flat size="0.8em" color="blue-grey-8" icon="draw"
                 label="COMMITTERS" class="q-pa-none q-ma-none" />
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
      <div class="child full-width col-8 light-glass q-pa-sm rounded-b-2 container">
        <div class="child full bg-blue-grey-1 blue-borders rounded-2"></div>
      </div>
    </div>

    <!-- div class="child full q-pa-none rounded-2 row items-start q-gutter-none">
      <q-card flat bordered class="my-card" :class="$q.dark.isActive ? 'bg-grey-9' : 'bg-grey-2'">
        <q-card-section>
          <div class="row items-center no-wrap">
            <div class="col">
              <div class="text-h6">Our Planet</div>
              <div class="text-subtitle2">by John Doe</div>
            </div>

            <div class="col-auto">
              <q-btn color="grey-7" round flat icon="more_vert">
                <q-menu cover auto-close>
                  <q-list>
                    <q-item clickable>
                      <q-item-section>Remove Card</q-item-section>
                    </q-item>
                    <q-item clickable>
                      <q-item-section>Send Feedback</q-item-section>
                    </q-item>
                    <q-item clickable>
                      <q-item-section>Share</q-item-section>
                    </q-item>
                  </q-list>
                </q-menu>
              </q-btn>
            </div>
          </div>
        </q-card-section>

        <q-card-section>
          {{ lorem }}
        </q-card-section>

        <q-separator />

        <q-card-actions>
          <q-btn flat>Action 1</q-btn>
          <q-btn flat>Action 2</q-btn>
        </q-card-actions>
      </q-card>
    </div-->

    <!-- div class="child full column rounded-2">
      <div class="child full col row container">
        <div class="child full q-pa-none row">
              <div class="col-8 text-left text-title q-pa-sm">
                Committers Box
              </div>
              <q-separator vertical></q-separator-->
              <!-- MORE DROPDOWN BUTTON -->
              <!--div class="col-3 text-center q-pa-sm">
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
      <div class="child full col-5 container">
      </div>
      <q-separator color="blue-grey-3"/>
      <div class="child full col-6 container">
      </div>
    </div-->
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
