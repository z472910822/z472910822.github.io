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
#include<iostream>
	
using namespace std;

template<typename X></br>
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
