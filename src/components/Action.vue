<template>
    <div>
        <h2 v-for="(item,index) in items" :key="index">{{item}}</h2>
        <h2>{{drink}}</h2>
    </div>
</template>
<script>
export default {
  props: {
    drink: {
      type: String,
      required: true,
      default: "冰峰"
    }
  },
  data: function() {
    return {
      items: ["果汁", "饮料", "橙汁"]
    };
  }
};
</script>
