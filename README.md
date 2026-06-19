# day-5-array-and-the-vectors
Day 5 of the c++ programming in the summer training camp 
//this is program of the me

//this is the program of the calculation of the min element 

#include<iostream>
#include<climits>
using namespace std;
int minelement(int arr[],int size){
    int minele=INT_MAX;
    for(int i=0;i<size;i++){
        minele=min(minele,arr[i]);
    }
    return minele;
}
int main(){
    int nums[]={11,45,76,764,154}
return 0;
}


//this is the program of the maxelement calculation in an array

#include<iostream>
#include<climits>
using namespace std;
int maxelement(int arr[],int size){
    int maxele=INT_MIN;
    for(int i=0;i<size;i++){
        maxele=max(maxele,arr[i]);
    }
    return maxele;
}
int main(){
    int nums[]={11,45,76,4,154};
    cout<<"the max number in this array is "<<maxelement(nums,sizeof(nums)/sizeof(nums[0]));
    return 0;
}
};
    cout<<"the min element in the array is  "<<minelement(nums,sizeof(nums)/sizeof(nums[0]));
    return 0;
}


//this is the program array sum calculation 

#include<iostream>
using namespace std;
int arraysum(int arr[],int size){
    int sum=0;
    for(int i=0;i<size;i++){
       sum=sum+arr[i];
    }
    return sum;
}
int main(){
    int nums[]={2,4,1};
    cout<<" Sum of the array is  "<<arraysum(nums,sizeof(nums)/sizeof(nums[0]));
    return 0;
}


//this is the program of the reverse array printing 

#include<iostream>
using namespace std;
void reversearray(int arr[],int size){
    int st=0,end=size-1;
    while(st<=end){
        int extra=arr[st];
        arr[st]=arr[end];
        arr[end]=extra;
        st++;end--;
    }
    for(int i=0;i<size;i++){
        cout<<arr[i]<<" ";
    }
}
int main(){
    int nums[]={21,32,45,5};
    reversearray(nums,4);
    return 0;
}


//this is the program of the second largest element in the array 

#include<iostream>
#include<climits>
using namespace std;
int maxelement(int arr[],int size){
    int maxele=INT_MIN;
    for(int i=0;i<size;i++){
        maxele=max(maxele,arr[i]);
    }
    int secondlar=INT_MIN;
    for(int i=0;i<size;i++){
        if(arr[i]<maxele){
            secondlar=max(secondlar,arr[i]);
        }
    }
    return secondlar;
}
int main(){
    int nums[]={11,45,4,154,445};
    cout<<"the max number in this array is "<<maxelement(nums,sizeof(nums)/sizeof(nums[0]));
    return 0;
}


//this is the program of the matrix sum 


#include <iostream>
#include <vector>
using namespace std;
int matrixsum(const vector<vector<int>>& matrix, int m, int n) {
    int sum = 0;
    for (int i = 0; i < m; i++) {
        for (int j = 0; j < n; j++) {
            sum = sum + matrix[i][j];
        }
    }
    return sum;
}

int main() {
    vector<vector<int>> mat = {{2, 3}, {3, 4}};
    int m = mat.size();
    int n = mat[0].size();
    cout << "the sum of the matrix is " << matrixsum(mat, m, n) << endl;
    return 0;
}




