<!--
 * @Author: yaohongbin
 * @Date: 2021-10-28 09:29:22
 * @LastEditors: yaohongbin
 * @LastEditTime: 2022-02-21 16:31:59
 * @FilePath: \node-gateway-grant\src\components\FormItemLayout\index.vue
 * @Description: 表单布局组件
-->

<template>
  <el-col v-bind="defaultAttrs" v-on="$listeners">
    <slot />
  </el-col>
</template>

<script>
import _ from 'lodash'

export default {
  name: 'FormItemLayout',
  computed: {
    defaultAttrs() {
      const defaultAttribute = {
        sm: 12,
        md: 8,
        lg: 6
      }
      return _.assign(defaultAttribute, this.$attrs)
    }
  }

}
</script>

<style>

</style>
