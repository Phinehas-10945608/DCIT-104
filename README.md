#include<iostream> 
using namespace std; 
  // Name: Phinehas Borketey Borteye
  // Student ID : 10945608
  // Programming Language used : C++
bool isPrime(int n); 
  
int main() 
{	 
	int num, sum=0, count=0; 
		 
   	cout<<"Please enter the required number: "; 
   	cin>>num; 
   	 
	for(int j=0; count<num; j++) 
	{ 
		if(isPrime(j))  
		{ 
			sum += j; 
			count++;	 
		} 
	} 
	 
	cout<<"The average of first "<<num<<" prime numbers is "<<(float)sum/count; 
} 
  
bool isPrime(int n) 
{ 
	bool Phine = true; 
	 
	if (n<2)		Phine = false; 
	else if(n==2)	Phine = true; 
	else 
	{ 
		for(int i=2; i<=n/2; i++) 
		{ 
			if(n%i==0) 
			{ 
				Phine = false; 
				break; 
			} 
		} 
	}	 
	return Phine;	 
} 
