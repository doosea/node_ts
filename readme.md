# ts 学习笔记


## git 操作
- git init : 初始化仓库
- git remote add origin "https://github.com/doosea/xxx.git" : 为当前仓库建立远程连接
- git branch -a : 列出所有本地和远程的分支
- git branch --set-upstream-to=origin/master master : 建立本地分支和远程分支的关联
- git config credential.helper store : 保存用户名和密码,不用再次输入
- git add file : 添加文件到暂存区
- git commit -m "msg" : 提交msg
- git push origin master : push 到远程

- git pull --allow-unrelated-histories : 忽略版本不同造成的影响



## 1. 变量

1. 声明

        let age: number;
    - let 为ts 关键字
    - age 为变量名  
    - number 为变量类型

2. 赋值

        age = 18

3. 声明并赋值

        let age: number = 18;


4. 变量命名

    - 区分大小写
    - 推荐使用驼峰命名

5. 数据类型

    1. 原始数据类型(基本数据类型)
    2. 对象类型

        常用的基本数据类型:

        - `number` : 数字类型 (整数和浮点数, 正数负数) 
        - `string` : 字符串类型 (推荐使用单引号)
        - `boolean` : 布尔类型 (`true` / `false`)
        - `undefined` : 只有一个值,值为类型本身(`undefined`), 表示声明但未赋值
        - `null` : 只有一个值,值为类型本身(`null`),  表示声明且已经赋值,但是值为`null`


## 2. 运算符

1. 算数运算符: 
    - `+ - * / `
    - 加号 `+` 还可以用来字符串拼接, 加号两边只要有一边是string ,就是执行字符串拼接

2. 赋值运算符:
    - `=, +=, -=, /=, *=`  

3. 自增和自减运算法:
    - `++`: `+= 1` 的简化形式 
    - `--`: `-= 1` 的简化形式

4. 比较运算符:
    - `<, <=, >, >=, ===, !==`, 返回 `boolean` 类型

5. 逻辑运算符:
    - `&&`: 与 and
    - `||`: 或 or
    - `!`: 非

## 3. 条件语句

        if (判断条件) {
            满足条件时执行
        } else {
            不满足条件时执行
        }


## 4. 三元运算符
        结果 = 判断条件 ? 值1 : 值2
        let s1: string = 2 > 3 ?  "大于":"小于"

## 5. 循环语句
   
-   for 循环
     
        for (初始化语句; 判断条件; 计数器更新) {
            循环体
        }
    
        for (let i: number=0; i<=3; i++){
            console.log(i)
        }
    
- 断点调试
 
    
    