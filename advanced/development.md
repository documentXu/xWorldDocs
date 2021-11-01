<!--
 * @Autor: liu_x25@ecidi.com
 * @Date: 2021-11-01 17:20:34
 * @LastEditors: liu_x25@ecidi.com
 * @LastEditTime: 2021-11-01 17:24:32
 * @Description: 组件
-->

## 原始组件开发
*根据项目要求需要重写系统原始组件功能时，可在不影响框架代码情况下通过插槽重写该组件，具体写法如下*
```html
<x-tools-item module="MeasureDistance">
    <self-components />
</x-tools-item>
```

## 新增组件开发
*根据项目要求需要新开发功能组件时，可参照如下写法*
```html
<x-tools-item
    module="AnalysisExplosion"
    icon="iconfx fx-analysis-explosion"
    title="分层爆炸"
    >
    <layer-explosion />
</x-tools-item>
```

