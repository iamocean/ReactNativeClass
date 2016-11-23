# 「React Native 入门」之样式与布局

在开始真正编码之前，我们先来了解下在 **React Native** 里的样式语法、图片引用等基础知识

### 样式语法

**React Native** 的样式语法与 **WEB** 的 **CSS** 样式语法基本类似，但是两个单词之间连接采用驼峰式而不是 " - " 连字符，另外在 **React Native** 里样式不需要指定具体单位（默认就是 **dp**）。

样式语法如下：

```javascript
selector {
  property: value
}
```



**内联样式**

```javascript
<View style={{width: 300, height: 300, backgroundColor: 'red'}}>
	<Text style={{fontSize: 16, textAlign:'center'}}>Hello React Native</Text>
</View>
```

其中 `style={{width: 300, height: 300, backgroundColor: 'red'}}`  这种是内联样式写法，需要注意的是第一个 **{}** 是 **JS** 表达式，第二个 **{}** 是 **JS** 对象（放样式用的）。



**外联样式**

```javascript
<View style={styles.box}>
	<Text style={styles.txt}>Hello React Native</Text>
</View>

const styles = StyleSheet.create({
  box: {
  	width: 300,
  	height: 300,
  	backgroundColor: 'red'
  },
  txt: {
  	fontSize: 16,
  	textAlign: 'center'
  }
});
```

`const styles` 表示定义了常量 **styles**

`StyleSheet.create`  是 **React Native** 内置的写法，用于检测样式是否编写正确，如果编写不正确，则在运行 **APP** 时就会及时反馈具体的错误信息。







### 图片引用写法

**本地图片**

```javascript
<Image source={require('本地图片路径')} style={width: 100, height: 100}></Image>
```

**网络图片**

```javascript
<Image source={{uri: '网络图片地址'}} style={width: 100, height: 100}></Image>
```

本地图片引用可以不写 *width* 和 *height* 值，默认能读取得到本地图片的宽高，但是一般建议都写上，其中 `require` 只接受字符串，如果需要动态修改本地图片路径，那么需要把 `require('本地图片路径')` 当成一整个变量来处理。

网络图片引用必需填写 *width* 和 *height* 值，否则图片无法解析出来。


