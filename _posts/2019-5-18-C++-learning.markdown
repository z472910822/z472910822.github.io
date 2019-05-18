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
