---
layout:     post                   
title:      一维二维数组             
subtitle:   Javase
date:       2020-07-08             
author:     丠                 
header-img: img/bg101.png    
catalog: true                       
tags:                             
    - Javase
    - 数组
---



#  数组对象创建

所谓数组，是有序的元素序列

若将有限个类型相同的变量的集合命名，那么这个名称为数组名。

声明数组后，需要为数组分配空间，也就是定义多大的数组。

### 一维数组

`int [] ages = {12,18,9,33,45,60}; `//声明并初始化了一个整型数组，它有6个元素

`char [] symbol = new char[10] `//声明并分配了一个长度为10的char型数组

#### 一维数组的遍历数组、集合
```

public class JudgePrime {
    public static void main(String[] args){
        int [] ages = {12, 18, 9, 33, 45, 60};
        int i = 1;
        for(int age:ages){
            System.out.println("数组中第"+i+"个元素是"+age);
            i++;
        }
    }
}
```
age：元素变量，ages：遍历对象

### 二维数组

创建方法1
数据类型 [][] 数组名 = new 数据类型[行的个数][列的个数];

创建方法2
数据类型 [][] 数组名;
数组名 = new 数据类型[行的个数][列的个数];

创建方法3
数据类型 [][] 数组名 = {
{第一行值1,第一行值2,...}
{第二行值1,第二行值2,...}
...
}

### 二维数组实例
```
public class ArrayTest
{
    public static void main(String[] args) 
    {
        String[][] name = {
                                {"ZhaoYi", "QianEr", "SunSan"},
                                {"LiSi", "ZhouWu", "WuLiu"}
                           };
        for (int i = 0; i < 2; i++)
                 {
                           for (int j = 0; j < 3; j++) {
                                                             System.out.println(name[i][j]);
                                                       }
                 }
    }
}
```


### 注意

无论是一维数组抑或是二维数组，他们的元素下标范围是***0~数组长度-1***
