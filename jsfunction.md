# 匹配正整数
```
let isPositiveNum = val => {
	return /^[1-9]\d*$/.test(val)
}
console.log(isPositiveNum(9)) //true
console.log(isPositiveNum(2.2)) //false

```

# 匹配负整数
```
 let isNegativeNum = val => {
 	return /^-[1-9]\d*$/.test(val)
 }
 console.log(isNegativeNum(-9)) //true
 console.log(isNegativeNum(2.2)) //false
```

# 匹配整数
```
let isInteger = val => {
	return /^(-|\+)?\d+$/.test(val)
}
console.log(isInteger(-9)) //true
console.log(isInteger(2.2)) //false
```

# 匹配非负浮点数
```
let isNotNegativeFloatNum = val => {
	return /^\d+(\.\d+)?$/.test(val)
}
console.log(isNotNegativeFloatNum(-9)) //false
console.log(isNotNegativeFloatNum(2.2)) //true
```

# 匹配由26个英文字母组成的字符串
```
let isAZaz = val => {
	return /^[A-Za-z]+$/.test(val)
}
console.log(isAZaz('122a')) //false
console.log(isAZaz('abc')) //true
```

# 匹配由26个英文字母的大写组成的字符串
```
let isAZ = val => {
	return /^[A-Z]+$/.test(val)
}
console.log(isAZ('Acs')) //false
console.log(isAZ('ABC')) //true
```

# 匹配由26个英文字母的小写组成的字符串
```
let isaz = val => {
	return /^[a-z]+$/.test(val)
}
console.log(isaz('Acs')) //false
console.log(isaz('abc')) //true
```

# 匹配电子邮件地址
```
let isEmailAddress = val => {
	return /^[\w-]+(\.[\w-]+)*@[\w-]+(\.[\w-]+)+$/.test(val) || /w+([-+.]w+)*@w+([-.]w+)*.w+([-.]w+)*/.test(val)
}
console.log(isEmailAddress('Acs')) //false
console.log(isEmailAddress('133@qq.com')) //true
```