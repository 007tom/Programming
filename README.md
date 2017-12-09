# 初探编程
建立这个项目的初衷是学习 *Javascript* 和 *Python 3* 程序语言的，我是从[程序设计基础](http://www.xuetangx.com/courses/course-v1:TsinghuaX+30240233X_2015_T2+sp/info)这门课中 *C++* 的学习来开始的，下面是我参考[廖雪峰的教程](https://www.liaoxuefeng.com/)写的笔记以及在学习C++的过程中碰到的实际问题的解决，方便以后复习使用！   

*文本编辑器*：1. [Dev-C++](https://sourceforge.net/projects/orwelldevcpp/) 2. [VS Code](https://code.visualstudio.com/) 3. [Notepad ++](https://notepad-plus-plus.org/download/v7.5.3.html)

需要注意的是， *C++* 笔记的整理过程注重计算思维，而 *Python 3* 和 *Javascript* 注重的是语法方面。
## Ⅰ. 知识点
	
	注意：
	
	1. 严格区分大小写；
	2. ; 表示语句的结束；
	3. 缩进：Tab 4个空格键；

### 1. *C++*   
	提示：
	
	注意运算符的优先级问题；   
	
#### 1.1 程序结构的基本含义：
   
   ```
#include <iostream>  // 包含库函数
using namespace std; // 命名空间
/* 主函数 */
int main() {
	return 0;
}
   ```
   
### 2. *Javascript*   

#### 2.1 数据类型：

(1) 数字：

+ 不区分整数和浮点数；

+ *NaN* 表示 *Not a Number*，当无法计算结果时用 *NaN* 表示；

+ *Infinity* 表示无限大，当数值超过 *Javascript* 的数字所能表示的最大值时，就表示为 *Infinity*；
```
0 / 0; // NaN
2 / 0; // Infinity
```
(2) 字符串：

(3) 布尔值：true false；

	* 运算符问题：
	
	1. && 与运算 || 或运算 ! 非运算；

	2. 比较运算符： > >= < <= == ===
	
		* == 会自动转换数据类型再比较， 应始终坚持 === 比较；
		
		* NaN 与所有值都不相等，包括它自己：
		
			NaN === NaN; // false
		
		 唯一能判断 NaN 的方法是通过 isNaN() 函数：
		
			isNaN(NaN); // true
			
		* 浮点数的相等比较：
		
			1/3 === (1 - 2/3); // false
			
		 要比较两个浮点数是否相等，只能计算它们之差的绝对值，看是否小于某个阈值。
		 
		 	Math.abs(1/3 - (1 - 2/3)) < 0.0000001; // true
			
(4) null 和 undefined：

	* null、0 和 ' '：
	
	null 表示一个“空”的值，与 Python 中的 None 类似， 0 是一个数字， ' ' 表示一个长度为0的字符串；
	
	* undefined 表示 “未定义”；
	
	* 大多数情况下，我们都应该用 null。undefined 仅仅在判断函数参数是否传递的情况下有用。
	
（5）数组：

+ 有序集合，可以包含任意数据类型；

+ 创建数组的方法：   


		1. [a, b];
		
		2. new Array(a, b);
		
	出于代码可读性的考虑，强烈建议直接使用第一种方法；
	
+ 访问：索引法

		arr[0]; // 访问第 1 个元素
		arr[2]; // 返回 undefined
		
（6）对象：

+ 无序集合， 采用键-值对方式 （键，表示字符串类型，又称 “对象的属性”；值，可以是任意数据类型）

		var person = {
			name: 'Bob',
			age: 20
		};

+ 获取元素：

		person.name; // 'Bob'
		
（7）变量：

+ 任意数据类型

+ 变量名：

	1. 大小写英文、数字、$、_ 的组合，且不能以数字开头；
	
	2. 不能是 *Javascript* 的关键字；
	
	3. 以 *var语句* 声明；
	
	4. 不建议用中文做变量名；

+ 变量赋值： =

	1. 可以是任意数据类型；
	
	2. 同一变量可以反复赋值，且值可以是不同类型数据；

	3. 只能用 *var* 声明一次；


### 3. *Python 3*   

  
	
## Ⅱ. 案例
### 1/33. 买菜问题：    
	
	(1) 描述：   
	
	张阿姨来到菜市场买菜
	7.9元每公斤的西红柿她买了0.8公斤
	9.5元每公斤的鸡蛋她买了1.5公斤
	8.7元每公斤的黄瓜她买了0.6公斤   
	
	(2) 问题：   
	
	张阿姨一共花了多少钱?
#### *C++* 版：
   ```
#include <iostream>
using namespace std;

int main()
{
	cout << 7.9 * 0.8 + 9.5 * 1.5 + 8.7 * 0.6 << endl;
	return 0;
}
   ```         
	
   
#### *Python 3*:   

  ```
print(7.9 * 0.8 + 9.5 * 1.5 + 8.7 * 0.6)
  ```   
  
#### *Javascript*: 

  ```
  console.log(7.9 * 0.8 + 9.5 * 1.5 + 8.7 * 0.6)
  ``` 
 
### 2/33. 
