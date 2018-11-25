<template>
  <el-menu mode="horizontal" :router="true">
    <el-menu-item index="1" :route="{ path: '/' }">
      Dove'S NeSt
    </el-menu-item>

    <el-menu-item index="2" :route="{ path: '/sns/' }">
      SNS
    </el-menu-item>

    <el-menu-item index="3" :route="{ path: '/artifacts/' }">
      Artifacts
    </el-menu-item>
  </el-menu>
</template>
