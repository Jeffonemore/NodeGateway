<!--
 * @Author: yaohongbin
 * @Date: 2021-11-04 18:49:48
 * @LastEditors: yaohongbin
 * @LastEditTime: 2022-02-21 16:31:55
 * @FilePath: \node-gateway-grant\src\components\RoleInput\index.vue
* @Description: 角色名称搜索组件
-->

<template>
  <search-input v-bind="$attrs" :request-options="searchOptions" :response-callback="responseCallback" v-on="$listeners">
    <slot />
  </search-input>
</template>

<script>
import SearchInput from '@/components/SearchInput'

export default {
  name: 'RoleInput',
  components: {
    SearchInput
  },
  computed: {
    searchOptions() {
      return {
        url: '/platform/list/role',
        method: 'post',
        data: {
          role_name: this.$attrs.value,
          page_no: 0,
          page_size: 0
        }
      }
    }
  },
  methods: {
    responseCallback({ data }) {
      return data.roles.map(item => ({
        value: item.role_name,
        name: item.role_name
      }))
    }
  }
}
</script>

<style>

</style>
