# 「React Native 入门」之样式与布局

在开始真正编码之前，我们先来了解下在 **React Native** 里的样式写法、图片引用等基础知识

### 样式写法

**RN** 里的样式基本与 **WEB** 的 **CSS** 语法类似，两个单词之间采用驼峰写法而不是" - "连字符。另外在 RN 里样式不需要指定具体单位（默认就是 **dp**）,

语法同样都是

```
selector {
  property: value
}
```



**内联样式**

```
<View style={{width: 300, height: 300, backgroundColor: 'red'}}>
	<Text style={{fontSize: 16, textAlign:'center'}}>Hello React Native</Text>
</View>
```

其中类似 `style={{width: 300, height: 300, backgroundColor: 'red'}}`  这种内联的样式写法，需要注意的下，第一个 **{}** 是 **JS** 表达式，第二个 **{}** 是 **JS** 对象。

**外链样式**

```
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

`StyleSheet.create`  是 **RN** 内置的写法，用于检测样式是否编写正确，如果不正确则在运行 **APP** 时就会即时报出具体的错误信息



### 图片引用写法

**本地图片**

```
<Image source={require('本地图片路径')} style={width: 100, height: 100}></Image>
```

**网络图片**

```
<Image source={{uri: '网络图片地址'}} style={width: 100, height: 100}></Image>
```

图片引用需要填写 *width* 和 *height* 值，否则图片无法解析。



