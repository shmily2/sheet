<template>
  <div>{{seeData.item}}</div>
   <div v-for="(list,value,index)from seeData.item" :key="index">
      <p>{{list}}</p>
  </div>
</template>
<script  lang="ts">
import { reactive, defineComponent } from "vue";
const seeData = reactive({
  item: ["111", "2222", "333"],
  listData: [
    {
      itemData: [
        {
          name: "工单号",
          context: "GD20220214000000"
        },
        {
          name: "项目名称:",
          context: "项目1"
        },
        {
          name: "紧急类型：",
          context: "一般"
        },
        {
          name: "报修企业：",
          context: "企业1"
        },
        {
          name: "报修人：",
          context: "张三"
        },
        {
          name: "联系电话：",
          context: "13000000000"
        },
        {
          name: "工单状态：",
          context: "待接单"
        },
        {
          name: "解决方式：",
          context: ""
        },
        {
          type: "button",
          name: "操作：",
          button: [
            {
              name: "转单",
              click: val => {
                console.log(val);
              }
            },
            {
              name: "查看详情",
              click: val => {
                console.log(val);
              }
            }
          ]
        }
      ]
    },
    {
      itemData: [
        {
          name: "工单号",
          context: "GD20220214000000"
        },
        {
          name: "项目名称:",
          context: "项目1"
        },
        {
          name: "紧急类型：",
          context: "一般"
        },
        {
          name: "报修企业：",
          context: "企业1"
        },
        {
          name: "报修人：",
          context: "张三"
        },
        {
          name: "联系电话：",
          context: "13000000000"
        },
        {
          name: "工单状态：",
          context: "待接单"
        },
        {
          name: "解决方式：",
          context: ""
        },
        {
          type: "button",
          name: "操作：",
          button: [
            {
              name: "转单",
              click: val => {
                console.log(val);
              }
            },
            {
              name: "查看详情",
              click: val => {
                console.log(val);
              }
            }
          ]
        }
      ]
    },
    {
      itemData: [
        {
          name: "工单号",
          context: "GD20220214000000"
        },
        {
          name: "项目名称:",
          context: "项目1"
        },
        {
          name: "紧急类型：",
          context: "一般"
        },
        {
          name: "报修企业：",
          context: "企业1"
        },
        {
          name: "报修人：",
          context: "张三"
        },
        {
          name: "联系电话：",
          context: "13000000000"
        },
        {
          name: "工单状态：",
          context: "待接单"
        },
        {
          name: "解决方式：",
          context: ""
        },
        {
          type: "button",
          name: "操作：",
          button: [
            {
              name: "转单",
              click: val => {
                console.log(val);
              }
            },
            {
              name: "查看详情",
              click: val => {
                console.log(val);
              }
            }
          ]
        }
      ]
    }
  ]
});
export default defineComponent({
  setup() {
    return {
      seeData
    };
  }
});
</script>
<style lang="">
</style>


