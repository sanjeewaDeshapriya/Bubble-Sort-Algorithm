# Bubble-Sort-Algorithm

#include <stdio.h>

int arr[5]={2,4,1,5,3};
int swap=0;




int main() {
    
    
    
    
    sort(arr);
    disArr();

    return 0;
}

void sort(int arr[5]){
    do{
        swap=0;
        for(int i=0;i<=sizeof(arr[5])-1;i++){
            if (arr[i]>arr[i+1]){
                int temp;
                temp=arr[i];
                arr[i]=arr[i+1];
                arr[i+1]=temp;
                swap=1;
        }
    }
        
    }while(swap);
}

void disArr(){
    for(int j=0;j<=sizeof(arr[5]);j++){
        printf("\n  %d",arr[j]);
    }
}
