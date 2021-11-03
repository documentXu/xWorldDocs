<!--
 * @Autor: liu_x25@ecidi.com
 * @Date: 2021-11-01 17:33:55
 * @LastEditors: liu_x25@ecidi.com
 * @LastEditTime: 2021-11-03 19:35:26
 * @Description: 实例说明
-->

### `layer`图层操作方法


>`opens()` 打开多个图层
```javascript
layer.opens([service]);
```
>`open()` 打开单个图层
```javascript
layer.open(service);
```
>`closes()` 关闭多个图层
```javascript
layer.closes(service);
```

>`close()` 关闭单个图层
```javascript
layer.close(service);
```

>`getAllModel` 获取所有模型
```javascript
layer.getAllModel();
```

>`getAllVectorTilesMap` 获取所有矢量瓦片地图
```javascript
layer.getAllVectorTilesMap();
```

>`getAllMap` 获取所有栅格地图
```javascript
layer.getAllMap();
```