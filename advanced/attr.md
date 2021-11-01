<!--
 * @Autor: liu_x25@ecidi.com
 * @Date: 2021-11-01 16:23:22
 * @LastEditors: liu_x25@ecidi.com
 * @LastEditTime: 2021-11-01 17:28:57
 * @Description: 
-->

## 组件属性

|  属性  | 默认值  | 描述  |
|  ----  | ----   |----  |
| showTerrain  | false  | 是否显示地形 |
| showLegend   | false  | 是否显示图例 |
| showAttr   | false  | 是否显示属性 |
| showNavigation   | false  | 是否显示指北针 |
| showTips   | false  | 是否显示比例尺 |


## 实例方法

该方法会返回xWorld核心操作类实例
```javascript
 init(xApi) {
    console.log("初始化成功",xApi);
 }
```



## 示例代码
```html
<template>
    <x-world 
        :showTerrain="true"
        :showLegend="true"
        :showAttr="true"
        :showTips="true"
        @init="init"
    ></x-world>
</template>
<script>
    import xWorld from "@/components/xWorld";
    export default{
        components:{
            xWorld
        },
        method:{
            init(xApi) {
                console.log("初始化成功",xApi);
            }
        }
    }
</script>
```