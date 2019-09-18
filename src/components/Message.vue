<template>
    <div>
        <h2 v-for="(item,index) in items" :key="index">{{item}}</h2>
        <div>{{sport}}</div>
        <div>{{arms}}</div>
        <div>{{computer}}</div>
        <div>{{book}}</div>
        <div>{{number}}</div>
    </div>
    
</template>
<script>
export default {
    props:{
     sport:{
         type:String,
         required:true,
         default:'打排球'
     },
     arms:{
         type:String,
         required:true,
         default:'水雷'
     },
     computer:{
         type:String,
         required:true,
         default:'Macbook Air'
     },
     book:{
         type:String,
         required:true,
         default:'语文'
     },
     number:{
         type:Number,
         required:true,
         default:19
     }

     
    },
    data:function(){
        return{
            items:[
                '水',
                '空气',
                '食物'
            ]
        }
    }
}
</script>
