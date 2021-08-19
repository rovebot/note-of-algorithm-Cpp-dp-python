# C++

## 1.数组

### 1.1 内置数组

`int arr[5] = {};`

特点：

- 数组大小固定，速度较快
- 数组初始化不能直接使用拷贝和`=`赋值，数组的传递只能以遍历的形式拷
- `==`不能正确地比较两个内置字符串

### 1.2 array

`array<int, 5> arr = {};`

array是C++11中引入的一个数组，是一种固定的**容器类型**，定义时需指定元素类型和个数

特点：

- 数组大小固定，速度较快，但和内置数组一样不能增加和删除数组中的元素
- 可以使用拷贝和赋值操作
- 可以使用**迭代器**
- 使用内置数组时，数组衰减为指针的风险更大，而array不会
- 比内置数组更可靠、轻量

操作：

`array<int, 6> arr = {1, 2, 3, 1, 2, 3};  `
