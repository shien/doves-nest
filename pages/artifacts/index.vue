<template>
  <section class="container artifacts">
    <el-card>
      <div slot="header" class="clearfix">
        <span>作ったもの</span>
      </div>
      <el-table :data="showArtifacts" style="width: 100%" class="table">
        <el-table-column prop="title" label="タイトル" width="200">
        </el-table-column>
        <el-table-column prop="explain" label="説明">
        </el-table-column>
        <el-table-column prop="link" label="リンク" width="100">
        </el-table-column>
      </el-table>
    </el-card>
  </section>
</template>

<script>
export default {
  computed: {
    showArtifacts() {
      return [
        {
          id: '001',
          title: 'タイピングゲーム',
          explain: 'javascript の canvas で作ったタイピングゲーム',
          link: '/typinggame',
        },
        {
          id: '002',
          title: 'お絵かき用 bot',
          explain: 'イラストのお題をランダムで出してくれるslack bot',
          link: 'なし',
        },
      ]
    }
  }
}
</script>

<style>
.artifacts .el-table__row {
  cursor: pointer;
}
</style>
