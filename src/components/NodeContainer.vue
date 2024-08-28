<template>
  <div class="child full anti-surface rounded-2 container">
   <div class="full row rounded-2 blue-borders light-glass">
    <div class="child full col-6 q-py-sm q-pl-sm q-pr-sm container">
      <div class="child full rounded-2 blue-borders bg-orange-1">
      </div>
    </div>
    <div class="child full col q-py-sm q-pl-xs q-pr-sm container">
      <div class="child full column rounded-2">
        <div class="child full col-4 container">
          <div class="child full blue-borders bg-orange-1 rounded-2 container">
            <CommittersBox></CommittersBox>
          </div>
        </div>
        <div class="child full col"></div>
        <!-- q-separator color="blue-grey-5"/-->
        <div class="child full col-7 container">
          <div class="child full blue-borders bg-orange-1 rounded-2 container">
          </div>
        </div>
      </div>
    </div>
   </div>
  </div>
</template>

<script>
import { defineComponent } from 'vue';
import CommittersBox from 'src/components/Boxes/CommittersBox.vue';

export default defineComponent({
  components: { CommittersBox },
  name: 'NodeContainer',
  /* setup() {
    return {
      splitterModelA: ref(70), // start at 50%
      splitterModelB: ref(50),
      insideModel: ref(70),
    };
  }, */
});
</script>
