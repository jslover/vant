<template>
  <div class="van-badge-group van-hairline--top-bottom">
    <slot />
  </div>
</template>

<script>
import { create } from '../utils';

export default create({
  name: 'van-badge-group',

  props: {
    activeKey: {
      type: [Number, String],
      default: 0
    }
  },

  data() {
    return {
      badges: []
    };
  }
});
</script>
