<template>
  <section class="container">
    <el-row>
      <el-col>
        <el-card>
          <el-table :data="showReadBooks" class="table">
            <el-table-column span="600" prop="skill" label="スキル">
            </el-table-column>
            <el-table-column prop="explain" label="詳細">
            </el-table-column>
          </el-table>
        </el-card>
      </el-col>
    </el-row>
  </section>
</template>

<script>
export default {
  computed: {
    showReadBooks() {
      return [
        {
          id: '001',
          skill: 'インフラ系',
          explain: 'TCP/IP の知識一通り。L1~L7 までの理解。LBやスイッチなどの機器の構築と基本操作など。',
        },
        {
           id: '002',
           skill: 'Linux',
           explain: 'サーバの一通りの構築、操作。CentOS/Ubuntu の実務経験あり。',
        },
        {
          id: '003',
          skill: 'MySQL',
          explain: '基本的な構築、管理系の操作。サーバーの監視設定。',
        },
        {
          id: '004',
          skill: 'Zabbix',
          explain: '基本的な構築、管理系の操作、サーバーの監視設定の投入。',
        },
        {
          id: '005',
          skill: 'Apache/Nginx',
          explain: '基本的な構築、管理系の操作、サーバーの監視設定の投入。',
        },
        {
          id: '006',
          skill: 'Ansible',
          explain: '基本的な構築、管理系の操作、サーバーの監視設定の投入。数百台の管理経験あり。',
        },
        {
           id: '007',
           skill: 'Golang',
           explain: '独学でのプログラミング。',
        },
        {
           id: '007',
           skill: 'Git',
           explain: 'Github の使い方、 Git の操作。gitflow での管理。',
        },
        {
          id: '008',
          skill: 'Python',
          explain: '独学でのプログラミング。',
        },
        {
          id: '009',
          skill: 'Nuxt.js',
          explain: 'このページを作れる程度。',
        },
        {
          id: '010',
          skill: 'Container/Kubernetes',
          explain: 'このページを作れる程度。Kubernetes で構築されている。',
        },
      ]
    }
  }
}
</script>
