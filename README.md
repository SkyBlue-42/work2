#include <bits/stdc++.h>
using namespace std;
void rotateleft(int arr[],int n,int d){
    reverse(arr,arr+d);
    reverse(arr+d,arr+n);
    reverse(arr,arr+n);
}
int main(){
    int i,n=5;
    int arr[5]={1,2,3,4,5};
    int d=2;
    rotateleft(arr,n,d);
    for(i=0;i<n;i++){
        cout<<arr[i];
    }
    return 0;
}
