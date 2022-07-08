# rh-css

## 使用

```less
// 放在最后一行
@import 'https://cdn.jsdelivr.net/npm/rh-css@0.0.2/lib/style.less';
```

## 基础

| 方法名                                                   | 描述                   |
| :------------------------------------------------------- | :--------------------- |
| `.PaddingMarginClear`                                    | margin, padding 归零   |
| `.WidthHeight(@width: 100%; @height: 0; @lineHeight: 0)` |
| `.PaddingMargin(@padding: 0; @margin: 0)`                |
| `#text.overflow;`                                        | 单行文本超出显示省略号 |

## 标签相关

| 方法名                 | 描述                   |
| :--------------------- | :--------------------- |
| `#textarea().noResize` | 取消textarea右下角箭头 |

## 对齐

- 默认居中
- `@row`: 水平反向
- `@col`: 垂直方向
  
| 方法名                                            | 描述              |
| :------------------------------------------------ | :---------------- |
| `#Align.flex(@row: center; @col: center;);`       | `flex`对齐        |
| `#Align.inlineFlex(@row: center; @col: center;);` | `inline-flex`对齐 |
| `#Align.position;`                                | 水平垂直对齐      |
| `#Align.position(row);`                           | 水平对齐          |
| `#Align.position(col);`                           | 垂直对齐          |

## css 箭头

- css border 边框箭头
- `#arrow.[top|right|bottom|left]([@width: 5px; @height: 5px; @borderWidth])`
- `@borderWidth`: 箭头线条粗细

```less
.arrow{
  // #arrow.top();
  // #arrow.right();
  // #arrow.bottom();
  #arrow.left();
}
```
