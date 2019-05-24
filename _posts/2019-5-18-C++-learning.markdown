---
layout:     post
title:      "C++学习 5-19 复习笔记"
date:       2019-05-18 20:15:00
author:     "Zlc"
header-img: "img/post-bg-miui6.jpg"
tags:
    - C++
    - ZLC
    - 复习笔记
---
```
#include<iostream>
using namespace std;
template<typename X>
X add(X x,X y)
{
	return x+y;
}
template<typename X>
X sub(X x,X y)
{
	return x-y;
}
int main(){
	int a=5;
	int b=2;
	cout<<add(a,b)<<endl;
	cout<<sub(a,b)<<endl;
	return 0;
}
```
```
	#include<iostream>
using namespace std;
template <typename T>
void insertionSort(T a[],int n)
{
	int i,j;
	for(i=1;i<n;i++)
	{
		int j=i;
		T temp=a[j];
		while(j>0&&temp<a[j-1])
		{
			a[j]=a[j-1];
			j--;
		}
		a[j]=temp;
	}
}
int main(){
	int a[10];
	for(int i=0;i<10;i++)
	{
		cin>>a[i];
	}
	insertionSort(a,10);
	for(int i=0;i<10;i++)
	{
		cout<<a[i]<<" ";
	}
	cout<<endl;
}
```
###transform函数的作用是：将某操作应用于指定范围的每个元素。transform函数有两个重载版本：<br>
transform(first,last,result,op);//first是容器的首迭代器，last为容器的末迭代器，result为存放结果的容器，op为要进行操作的一元函数对象或sturct、class。<br>
transform(first1,last1,first2,result,binary_op);//first1是第一个容器的首迭代 器，last1为第一个容器的末迭代器，first2为第二个容器的首迭代器，<br>result为存放结果的容器，binary_op为要进行操作的二元函数 对象或sturct、class。
