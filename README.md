#include<iostream>
using namespace std;
void prime(int a);
int main()
{
int b = 0;
   cout<<"Any number:"<<endl;
   cin>>b;
   prime(b);
}
void prime (int a)
{
int sum = 0;
  for(int m = a;m>1;m-)
  {
  bool isPrime = true;
  for (int n=2;n<m;n++)
    if(m%n==0)
        {
        isPrime = false;
        n=m;
        }
   }
   if (isPrime == true)
       {
       cout<<"prime numbers:"<<m<<",";
       sum = sum + m;
       }
   }
   cout<<endl<<"sum of the given prime numbers:"<<sum;
 }
