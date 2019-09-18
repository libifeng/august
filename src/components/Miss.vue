<template>
    <div>
        <h2 v-if='seen'>可以</h2>
        <h2 v-else>不可以</h2>
        <h2>{{color}}</h2>
        <h2>{{taste}}</h2>
        <h2>{{pen}}</h2>
    </div>
</template>
<script>
export default {
  props: {
    color: {
      type: String,
      required: true,
      default: "red"
    },
    taste:{
        type:String,
        required:true,
        default:'辣味'
    },
    pen:{
        type:String,
        required:true,
        default:'铅笔'
    }
  },
  data: function() {
    return {
      seen: false
    };
  }
};
</script>
