<template>
  <div>
    <el-container>
      <el-header>导入</el-header>
      <el-main>
        <div class="content">
          <div class="alert">
            <el-alert title="警告提示的文案" show-icon :closable="false" style="backgroundColor: #409EFF;color:#fff">
            </el-alert>
          </div>

          <!-- 第一阶段： 准备导入 -->
          <div class="page-import-ready" v-show="fileImport.status === status.ready">

          </div>
        </div>
      </el-main>
    </el-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      fileImport:{
        status
      }
    };
  },

  components: {},

  computed: {},

  methods: {}
}

</script>
<style  lang="less">
.el-container {
  .el-header {
    color: red;
  }
  .content {
    .el-alert {
      width: 880px;
      margin: 0 auto;
      margin-bottom: 24px;
      .el-alert__icon {
        font-size: 16px;
        width: 16px;
        color: #fff;
        display: table-cell;
      }
      .el-alert__content {
        display: table-cell;
        line-height: 0px;
        padding: 0 16px 0 8px;
      }
    }
  }
}
</style>