# RegExp
常用正则表达式
### 判断用户输入的是不是合法的用户名（长度6-20个字符，只能包括字母、数字、下划线）
```
function isValidUsername(str){
  var reg = /^\w{6,20}$/g;
  return reg.test(str);
}
```

### 判断用户输入的是不是手机号
```
function isPhoneNum(str){
  var reg = /^1[3578]\d{9}$/g;
  return reg.test(str)
}
```

### 判断用户输入的是不是邮箱
```
function isEmail(str){
  var reg = /^\w+@\w+\.\w+/g
  return reg.test(str)
}
```
