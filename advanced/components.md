<!--
 * @Autor: liu_x25@ecidi.com
 * @Date: 2021-11-01 16:40:02
 * @LastEditors: liu_x25@ecidi.com
 * @LastEditTime: 2021-11-01 17:10:07
 * @Description: 
-->

> 组件说明
## 侧边栏
*用于加载左侧树组件容器*
```html
<x-bar></x-bar>
```
## 侧边栏子模块
*用于加载树组件子容器*

```html
<x-bar-item module="Scene"></<x-bar-item>
```
|  属性   | 必传 | 描述  |
|  ----   |  ---- | ----  |
| module  |true|模块名称，用于标识加载模块唯一命名 |
| icon  |false|模块图标(自定义模块时必传) |
| title  |false|模块标题(自定义模块时必传) |

*参数说明*

|  模块   | 描述  |
|  ----  | ----  |
| Scene  | 场景树，用于构建场景列表以及分类模块 |
| Layer  | 图层树，用于构建图层树以及分类模块 |
| Plot   | 标绘树，用于构建标绘树以及分类模块 |

## 工具栏
*用于加载底部工具栏容器*
```html
<x-tools></x-tools>
```
## 工具栏子模块
*用于加载底部工具栏子模块*
```html
<x-tools-item :module="Home"></x-tools-item>
```
|  属性   | 必传 | 描述  |
|  ----   |  ---- | ----  |
| module  |true|模块名称，用于标识加载模块唯一命名 |
| icon  |false|模块图标(自定义模块时必传) |
| title  |false|模块标题(自定义模块时必传) |

*参数说明*

|  模块   | 描述  |
|  ----  | ----  |
| Home  | 复位功能模块 |
| MeasureDistance  | 测距功能 |
| MeasureArea   | 面积测量 |
| MeasureHeight   | 高度测量 |
| MeasurePosition  | 位置测量 |
| CutFace   | 面剖切 |
| Flyroam   | 飞行漫游 |
| Lookaround  | 定点环视 |
| AnalysisPositionview   | 通视分析 |
| AnalysisChooseview   | 可视域分析 |
| AnalysisSkyline  | 天际线分析 |
| AnalysisSunlight   | 日照分析 |
| AnalysisHighlimit   | 限高分析 |
| AnalysisProfile  | 剖面分析 |
| Scene   | 场景保存 |
| Scenelist   | 场景列表 |
| Plot  | 动态标绘 |
| Transparency   | 透明度调节 |
| Splitescreen   | 分屏功能 |
| Fullscreen  | 全屏控制 |
| Help   | 帮助模块 |

## 多级工具栏
*用于加载二级工具栏*
```html
<x-tools-items :module="Home"></x-tools-items>
```
|  属性   | 必传 | 描述  |
|  ----   |  ---- | ----  |
| module  |true|模块名称，用于标识加载模块唯一命名 |


> 示例代码
```html
<x-world>
    <x-bar>
        <x-bar-item module="Scene" />
        <x-bar-item module="Layer" />
        <x-bar-item module="Plot" />
    </x-bar>
    <x-tools>
        <x-tools-item module="Home"> </x-tools-item>
        <x-tools-items module="Measure">
          <x-tools-item module="MeasureDistance"> </x-tools-item>
          <x-tools-item module="MeasureArea"> </x-tools-item>
        </x-tools-items>
    </x-tools>
</x-world>
```