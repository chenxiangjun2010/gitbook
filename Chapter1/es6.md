# 第2节：常用的es6

- `Math.min(...array)` 数组中最小值 类似于lodash的`_.min()`,其实可以通过`array.sort(function(a,b)=>return b-a),`对数组排序后在取第一位.
- `Math.max(...array)`数组中最大值，具体跟`Math.min(...array)`相反。
- `Array.from(new Set(array));` 数组的去重，不适合数组是对象数组。

