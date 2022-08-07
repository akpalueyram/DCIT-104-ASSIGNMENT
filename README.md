#include<iostream>
using namespace std;
void prime(int x);
int main()
{
int n = 0;
   cout<<"Any number:"<<endl;
   cin>>n;
   prime(n);
}
void prime (int x)
{
int sum = 0;
  for(int i = x;i>1;i-)
  {
  bool isPrime = true;
  for (int j=2;j<i;j++)
    if(i%j==0)
        {
        isPrime = false;
        j=i;
        }
   }
   if (isPrime == true)
       {
       cout<<"prime numbers:"<<i<<",";
       sum = sum + i;
       }
   }
   cout<<endl<<"sum of the given prime numbers:"<<sum;
 }
