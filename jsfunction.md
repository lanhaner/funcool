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

# 返回数组中的最大值
```
let arrayMax = arr => Math.max(...arr)
let arr = [1,2,3,5]
console.log(arrayMax(arr)) //5
```

# 返回数组中的最小值
```
let arrayMin = arr => Math.min(...arr)
let arr = [1,2,3,5]
console.log(arrayMin(arr)) //1
```

# 将数组块划分为指定大小的较小数组
```
let chunk = (arr, size) => Array.from({
	length: Math.ceil(arr.length / size)
}, (v, i) => arr.slice(i * size, i * size + size))
let arr = [1, 2, 3, 5]
console.log(chunk(arr,2)) //0: Array [ 1, 2 ],1: Array [ 3, 5 ]
```

# 从数组中移除 false 值
```
let compact = arr => arr.filter(Boolean)
let arr = [false,null,0,"",undefined,NaN,1]
console.log(compact(arr)) //[ 1 ]
```

# 计算数组中值的出现次数
```
let countOccurrences = (arr, value) => arr.reduce((a, v) => v === value ? a + 1 : a + 0, 0)
let arr = [1,2,1,2,3,3,3,3]
console.log(countOccurrences(arr,3))//4
```

# 深拼合数组
```
let deepFlatten= arr => [].concat(...arr.map(v => Array.isArray(v) ? deepFlatten(v) : v))
let arr = [1, 2, [1, 2, [1, 2, [2, 3]]]]
console.log(deepFlatten(arr)) // [ 1, 2, 1, 2, 1, 2, 2, 3 ]
```

# 返回两个数组之间的差异
```
let difference = (a, b) => {
	const s = new Set(b)
	return a.filter(x => !s.has(x))
};
let arr = [1,2,3]
let arr2 = [2,3,4]
console.log(difference(arr,arr2))//[1]
console.log(difference(arr2,arr))//[4]
```

# 返回数组的所有不同值
```
let distinctValuesOfArray = arr => [...new Set(arr)]
let arr = [1, 2, 3, 1, 2]
console.log(distinctValuesOfArray(arr)) // [ 1, 2, 3 ]
```
# 返回数组中的每个第n个元素
```
let everyNth = (arr, nth) => arr.filter((e, i) => i % nth === 0)
```

# 筛选出数组中的非唯一值
```
let filterNonUnique = arr => arr.filter(i => arr.indexOf(i) !== arr.lastIndexOf(i))
```

# 拼合数组
```
let flatten = arr => arr.reduce((a, v) => a.concat(v), [])
```