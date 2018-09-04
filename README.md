# RegExp
常用正则表达式

#### 判断用户输入的是不是合法的用户名（长度6-20个字符，只能包括字母、数字、下划线）
------
```
function isValidUsername(str){
  var reg = /^\w{6,20}$/g;
  return reg.test(str);
}
```

#### 判断用户输入的是不是手机号
------
```
function isPhoneNum(str){
  var reg = /^1[3578]\d{9}$/g;
  return reg.test(str)
}
```

#### 判断用户输入的是不是邮箱
------
```
function isEmail(str){
  var reg = /^\w+@\w+\.\w+/g
  return reg.test(str)
}
```

#### 去除字符串两边的空白字符
------
```
function trim(str) {
  var reg = /^\s+|\s+$/g;
  return str.replace(reg,'')
}
```

#### 得到字符串里所有的颜色
------
```
var subj = "color: #121212; background-color: #AA00ef; width: 12px; bad-colors: f#fddee "
var colorReg = /#([0-9a-fA-F]{6}|[0-9a-fA-F]{3})(?=;)/g
console.log( subj.match(colorReg) )
```
