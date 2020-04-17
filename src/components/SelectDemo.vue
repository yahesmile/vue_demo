<template>
    <div>
        <label v-text="selectLabel"></label>
        <select :name="name">
            <option value="">--请选择--</option>
            <option v-for="item in list" :value="item.value" :key="item.id">{{item.name}}</option>
        </select>
    </div>
</template>

<script>
export default {
  name: 'SelectDemo',
  props: {
    selectLabel: String,
    name: String,
    list: Array
  }
}
</script>
