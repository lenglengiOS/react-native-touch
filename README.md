# react-native-touch

react-native-touch is a plugin that prevents repeated clicks.

由于目前fb官方封装的很多组件不能满足开发需求，比如Touchable系列的点击组件都没有考虑到重复点击的问题，假如用户在点击按钮push新页面的时候快速点击几次，就会同时push多次，[react-native-touch-once](https://www.npmjs.com/package/react-native-touch-once) 针对解决了这个问题，同时支持Android、iOS.

install

```yarn add react-native-touch-once```  或者 ```npm install react-native-touch-once --save```

Usage

```

import Touch from 'react-native-touch-once';


<Touch
      style={{width:SCREEN_WIDTH, backgroundColor:'#f4f4f4'}}
      activeOpacity={1}
      onPress={()=>this.goDatil(item)}>
      <View style={styles.item}>
           {/* doSomething */}
      </View>
</Touch>
```
用法和官方的Touchable系列组件用法相同，这里只是针对重复点击做了封装。
