<template>
  <div class="page1">
    <h1>This is an vue1 page</h1>
    <div>
      <SelectDemo :selectLabel="selectLabel" :list="list" :name="name"/>
    </div>
  </div>
</template>

<script>
import SelectDemo from '@/components/SelectDemo.vue'
export default {
  name: 'Page1',
  data () {
    return {
      selectLabel: '自定义下拉label',
      name: 'selectName',
      list: [
        { id: 1, value: 1, name: 'one' },
        { id: 2, value: 2, name: 'two' }
      ]
    }
  },
  components: {
    SelectDemo
  }
}
</script>
