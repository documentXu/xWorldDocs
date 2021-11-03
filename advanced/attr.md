<!--
 * @Autor: liu_x25@ecidi.com
 * @Date: 2021-11-01 16:23:22
 * @LastEditors: liu_x25@ecidi.com
 * @LastEditTime: 2021-11-02 11:36:43
 * @Description: 
-->

## 组件属性

|  属性  | 默认值  | 描述  |
|  ----  | ----   |----  |
| showTips   | false  | 是否显示比例尺 |
| terrainServer   | https://www.supermapol.com/realspace/services/3D-stk_terrain/rest/realspace/datas/info/data/path  | 地形服务地址(设置为false则不加载地形) |

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
        :terrainServer="false"
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