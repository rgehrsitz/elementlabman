<script setup lang="ts">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import HelloWorld from './components/HelloWorld.vue'
import FooterView from './components/FooterView.vue';
import HeaderView from './components/HeaderView.vue';
</script>

<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld msg="Hello Vue 3 + TypeScript + Vite" />-->
  <el-container>
    <el-header>
      <HeaderView />
    </el-header>
    <el-container>
      <el-aside width="56px">
        <div>
          Aside
          <el-button-group>
            <el-tooltip
              class="item"
              effect="light"
              content="Right Top prompts info"
              placement="right-start"
              show-after="1000"
            >
              <el-button type="primary" icon="el-icon-edit"></el-button>
            </el-tooltip>
            <el-button type="primary" icon="el-icon-share"></el-button>
            <el-button type="primary" icon="el-icon-delete"></el-button>
          </el-button-group>
        </div>
        <div>
          <el-button type="primary" icon="el-icon-edit"></el-button>
        </div>
      </el-aside>
      <el-container>
        <el-main>
          Main
          <HelloWorld msg="Hello Vue 3 + TypeScript + Vite" />
        </el-main>
      </el-container>
    </el-container>
    <el-footer>
      <FooterView></FooterView>
    </el-footer>
  </el-container>
</template>

<style>
.el-header,
.el-footer {
  background-color: #b3c0d1;
  color: var(--el-text-color-primary);
  display: flex;
  justify-content: space-between;
  flex-wrap: nowrap;
  font-size: 16px;
}

.el-aside {
  background-color: #d3dce6;
  color: var(--el-text-color-primary);
  text-align: center;
  line-height: 50px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.el-main {
  background-color: #e9eef3;
  color: var(--el-text-color-primary);
  text-align: center;
  line-height: 60px;
}

body {
  height: 100vh;
  margin: 0px;
}

body > .el-container {
  height: 100%;
}
.el-container.is-vertical {
  height: 100vh;
}

.el-button-group > .el-button {
  border-radius: 0px;
  margin-left: 0px;
  margin-right: 0px;
}
</style>
