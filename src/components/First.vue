<template>
    <div>
        <div>{{name}}</div>
        <div>{{age}}</div>
        <div>{{hobby}}</div>
        <div>{{sport}}</div>
        <div>{{fruit}}</div>
        <div>{{sports}}</div>
       <h3 v-for="(item,index) in items" :key='index'>
            {{item}}
        </h3>
    </div>
</template>
<script>
export default {
  props: {
    name: {
      type: String,
      required: true,
      default: "libifeng"
    },
    age: {
      type: Number,
      required: true,
      default: 29
    },
    hobby: {
      type: String,
      required: true,
      default: "睡觉"
    },
    sport: {
      type: String,
      required: true,
      default: "跑步"
    },
    fruit: {
      type: String,
      required: true,
      default: "香蕉"
    },
    sports:{
        type:String,
        required:true,
        default:'打篮球'
    }
  },
  data: function() {
    return {
      items: ["春", "夏", "秋", "冬"]
    };
  }
};
</script>
