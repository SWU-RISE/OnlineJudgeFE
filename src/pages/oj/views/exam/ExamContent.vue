<template>
<div>
<Form :model="formItem" :label-width="80">
        <FormItem label="课程名称">
            <Input v-model="formItem.input" placeholder="Enter something..."></Input>
        </FormItem>
		<FormItem label="出题人">
            <Input v-model="formItem.input" placeholder="Enter something..."></Input>
        </FormItem>
        <FormItem label="试卷类型">
            <RadioGroup v-model="formItem.radio">
                <Radio label="male">A卷</Radio>
                <Radio label="female">B卷</Radio>
            </RadioGroup>
        </FormItem>
		<FormItem label="出题时间">
            <Row>
                <Col span="11">
                    <DatePicker type="date" placeholder="Select date" v-model="formItem.date"></DatePicker>
                </Col>
                <Col span="2" style="text-align: center">-</Col>
                <Col span="11">
                    <TimePicker type="time" placeholder="Select time" v-model="formItem.time"></TimePicker>
                </Col>
            </Row>
        </FormItem>
    </Form>
</div>
</template>
<script>
  export default {
    name: 'BasicContent'
  }
</script>
<style lang="less" scoped>
.layout{
    border: 1px solid #d7dde4;
    background: #f5f7f9;
    position: relative;
    border-radius: 4px;
    overflow: hidden;
}
.layout-logo{
    width: 100px;
    height: 30px;
    background: #5b6270;
    border-radius: 3px;
    float: left;
    position: relative;
    top: 15px;
    left: 20px;
}
.layout-nav{
    width: 420px;
    margin: 0 auto;
    margin-right: 20px;
}
.layout-footer-center{
    text-align: center;
}
</style>
