<!--
 * @Autor: liu_x25@ecidi.com
 * @Date: 2021-11-01 17:33:55
 * @LastEditors: liu_x25@ecidi.com
 * @LastEditTime: 2021-11-03 19:36:14
 * @Description: 实例说明
-->

### `tip`提示类使用


>`showAt()` 打开提示框

|  属性   | 必传 | 简述  |
|  ----   |  ---- | ----  |
| position  |true|屏幕坐标（x,y） |
| message  |false|提示文字 |

```javascript
tip.showAt(position,message);
```
>`setVisible()` 设置提示框显示隐藏
```javascript
tip.setVisible(visible:Boolean);
```
