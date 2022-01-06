# Armstrong-number
To find if a number is Armstrong or not

#include <iostream>
#include<math.h>
using namespace std;

int main()
{
	int n,sum;
	cin>>n;
	sum=0;
	int original =n;
	
	while(n>0){
		
		int lastdigit= n%10;
		sum+=pow(lastdigit,3);
		n= n/10;
		}
		
	if(sum==original){
		cout<<"Its Armstrong!"<<endl;
		}
	else{
		cout<<"not Armstrong!"<<endl;
		}

	return 0;
}
