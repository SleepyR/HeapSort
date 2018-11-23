#include <iostream>
using namespace std;

void heapify(int arr[],int n,int i)
{
  int left=2*i+1;
  int right=2*i+2;
  if(left<n && arr[left]>arr[right])
  {
    if(arr[left]>arr[i])
    {
      swap(arr[left],arr[i]);
      heapify(arr,n,left);
    }
  }
  else if(right<n) 
  {
    if(arr[right]>arr[i])
    {
      swap(arr[right],arr[i]);
      heapify(arr,n,right);
    }
  }
}

void heapsort(int arr[],int n)
{ 
  for(int i=n/2-1;i>=0;i--)
  {
    heapify(arr,n,i);
  }
  for(int i=n-1;i>=0;i--)
  {
    swap(arr[0],arr[i]);
    heapify(arr,i,0);
  }
}

void printArray(int a[],int n)
{
  for(int i=0;i<n;i++)
     cout<<a[i]<<" ";
} 
int main() 
{
  int arr[]={227,438,943,444,740,852,666,45,771,994,401,680,594};
  int n=sizeof(arr)/sizeof(arr[0]);
  heapsort(arr,n);
  cout<<"Printing the array"<<endl;
  printArray(arr,n);
}
