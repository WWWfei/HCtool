<template>
  <div class="main">
    <Header class="header">tools</Header>
    <div class="main-body">
      <div class="sidebar">
        <Sidebar></Sidebar>
      </div>
      <Building class="content"></Building>
    </div>
    <!-- <test></test> -->
  </div>
</template>

<script>
// https://juejin.im/post/5e8e8d5a6fb9a03c6d3d9f42#heading-11
// https://uniapp.dcloud.net.cn/README
import Vue from 'vue';
import Component from 'vue-class-component';

import Header from '../layouts/Header';
// import Test from '../test/TestDrag';
import Sidebar from '../layouts/Sidebar';
import Building from '../layouts/Buildiing';

@Component({
  components: {
    Header,
    // Test,
    Sidebar,
    Building,
  },
})
export default class Home extends Vue {
//  点击预览
//  r.onclick = function() {
//     var n = t.value;
//     if (n != "") {
//       var r = window.open("", "", "");
//       r.opener = null,
//       r.document.write(n),
//       r.document.close()
//     } else alert("请将需要运行的HTML填写到输入框后再运行！", "alert", "运行提示")
//   }

}
</script>

<style scoped lang="less">
.main {
  // border: solid 1px red;
  .main-body {
    display: flex;
    justify-content: flex-start;
    height: calc(100vh - 30px);
    margin-top: 65px;

    .sidebar {
      width: 30vw;
      background-color: whitesmoke;
    }
    .content {
      flex: 1;
      background-color: white;
    }
  }
}
</style>
