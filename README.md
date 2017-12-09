# 初探编程
建立这个项目的初衷是学习 *Javascript* 和 *Python 3* 程序语言的，我是从[程序设计基础](http://www.xuetangx.com/courses/course-v1:TsinghuaX+30240233X_2015_T2+sp/info)这门课中 *C++* 的学习来开始的，下面是我参考[廖雪峰的教程](https://www.liaoxuefeng.com/)写的笔记以及在学习C++的过程中碰到的实际问题的解决，方便以后复习使用！   

*文本编辑器*：1. [Dev-C++](https://sourceforge.net/projects/orwelldevcpp/) 2. [VS Code](https://code.visualstudio.com/) 3. [Notepad ++](https://notepad-plus-plus.org/download/v7.5.3.html)

## Ⅰ. 知识点
### 1. *C++*   
	提示：
	
	注意运算符的优先级问题；
### 2. *Javascript*
### 3. *Python 3*   

	提示：
	
 	1. 坚持使用**4个空格**的缩进；
	2. Python程序**对大小写敏感**；  
	
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
