<template>
<Panel>
	<p>基本信息</p>
	<BasicContent></BasicContent>
	<Divider />
	<p>创建试卷</p>
	<ExamContent></ExamContent>
</Panel>
</template>
<script>
  import BasicContent from './BasicContent'
  	 import ExamContent from './ExamContent'

  export default {
    name: 'exam',
    components: {
      BasicContent,
      ExamContent
    }
  }
</script>
<style lang="less" scoped>
</style>