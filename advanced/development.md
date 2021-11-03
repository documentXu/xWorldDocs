<!--
 * @Autor: liu_x25@ecidi.com
 * @Date: 2021-11-01 17:20:34
 * @LastEditors: liu_x25@ecidi.com
 * @LastEditTime: 2021-11-02 14:34:42
 * @Description: 组件
-->

>根据项目要求需要重写系统原始组件功能时，可在不影响框架代码情况下通过插槽重写该组件或根据项目要求需要新开发功能组件。具体写法如下

*当`module`模块标识名不存在时务必传递`icon`和`title`参数*

###### 主框架代码

```template
<x-tools-item
    module="AnalysisExplosion"
    icon="iconfx fx-analysis-explosion"
    title="分层爆炸"
    >
    <self-components />
</x-tools-item>
```

###### 子组件代码

```vue
<template>
    <div>子组件内容</div>
</template>
<script>
export default{
    mounted(){
        console.log('组件引用成功')
    },
    destoryed(){
        console.log('组件销毁成功')
        this.clear();
    },
    clear(){
        this.$parent.exit();//退出组件
    }
}
</script>
```

