<template>
  <div class="footer">
    <!-- <mt-tabbar v-model="selected"
    :fixed="true">
      <mt-tab-item id="主页" @click.native="menuTab('/Home')">
        <img slot="icon" src="../assets/logo.png">
        页面1
      </mt-tab-item>
      <mt-tab-item id="资产公告"  @click.native="menuTab('/page1')">
        <img slot="icon" src="../assets/logo.png">
        页面2
      </mt-tab-item>
      <mt-tab-item id="路线图" @click.native="menuTab('/page2')">
        <img slot="icon" src="../assets/logo.png">
        页面3
      </mt-tab-item>
    </mt-tabbar> -->
  </div>
</template>

<script>
import { mapGetters } from "vuex";

export default {
  name: "NavigateTabBar",
  data: () => ({
    selected: 0
  }),
  methods: {
    menuTab(name) {
      this.$router.push(name);
    }
  }
};
</script>
