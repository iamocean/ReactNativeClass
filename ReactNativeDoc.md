# React Native 之 style 属性

常用的 **Style** 属性，重新整理分成以下几类

- [布局类](#布局类)
- [形状类](#形状类)
- [美化类](#美化类)



### 布局类

| 布局类属性(默认取值number)                        | View | Text | Image |
| ---------------------------------------- | ---- | ---- | ----- |
| flex                                     | √    | √    | √     |
| flexDirection(row\|column)               | √    | √    | √     |
| flexWrap(wrap\|nowrap)                   | √    | √    | √     |
| alignItems(flex-start\|flex-end\|center\|stretch) | √    | √    | √     |
| alignSelf(auto\|flex-start\|flex-end\|center\|stretch) | √    | √    | √     |
| justifyContent(flex-start\|flex-end\|center\|space-between\|space-arowd) | √    | √    | √     |
| position(relative\|absolute)             | √    | √    | √     |
| top                                      | √    | √    | √     |
| bottom                                   | √    | √    | √     |
| left                                     | √    | √    | √     |
| right                                    | √    | √    | √     |



### 形状类

| 形状类(默认取值number)   | View | Text | Image |
| ----------------- | ---- | ---- | ----- |
| width             | √    | √    | √     |
| height            | √    | √    | √     |
| padding           | √    | √    | √     |
| paddingTop        | √    | √    | √     |
| paddingBottom     | √    | √    | √     |
| paddingLeft       | √    | √    | √     |
| paddingRight      | √    | √    | √     |
| paddingHorizontal |      |      |       |
| paddingVertical   |      |      |       |
| margin            | √    | √    | √     |
| marginTop         | √    | √    | √     |
| marginBottom      | √    | √    | √     |
| marginLeft        | √    | √    | √     |
| marginRight       | √    | √    | √     |
| marginHorizontal  |      |      |       |
| marginVertical    |      |      |       |



### 美化类

| 美化类(默认取值number)                          | View | Text | Image |
| ---------------------------------------- | ---- | ---- | ----- |
| borderStyle(solid\|dotted\|dashed)       | √    | √    |       |
| borderColor(color)                       | √    | √    | √     |
| borderTopColor(color)                    | √    | √    |       |
| borderBottomColor(color)                 | √    | √    |       |
| borderLeftColor(color)                   | √    | √    |       |
| borderRightColor(color)                  | √    | √    |       |
| borderWidth                              | √    | √    | √     |
| borderTopWidth                           | √    | √    | √     |
| borderBottomWidth                        | √    | √    | √     |
| borderLeftWidth                          | √    | √    | √     |
| borderRightWidth                         | √    | √    | √     |
| borderRadius                             | √    | √    | √     |
| borderTopLeftRadius                      | √    | √    | √     |
| borderTopRightRadius                     | √    | √    | √     |
| borderBottomLeftRadius                   | √    | √    | √     |
| borderBottomRightRadius                  | √    | √    | √     |
| backgroundColor(color)                   | √    | √    | √     |
| opacity                                  | √    | √    | √     |
| overflow(visible\|hidden)                | √    | √    | √     |
| backfaceVisibility(visible\|hidden)      | √    | √    | √     |
| color(color)                             |      | √    |       |
| fontFamily(string)                       |      | √    |       |
| fontSize                                 |      | √    |       |
| fontStyle(normal\|italic)                |      | √    |       |
| fontWeight(normal\|bold\|100-900)        |      | √    |       |
| lineHeight                               |      | √    |       |
| textAlign(auto\|left\|right\|center\|justify) |      | √    |       |
| textDecorationLine(none\|underline\|line-through\|underline line-through) |      | √    |       |
| textShadowColor(color)                   |      | √    |       |
| textShadowOffset({width:number,height:number}) |      | √    |       |
| textShadowRadius                         |      | √    |       |