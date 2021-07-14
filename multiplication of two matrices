#include <stdio.h>


void element(int m[15][15],int row, int column){
    for(int i=0;i < row;i++)
    for(int j=0;j < column;j++){
        printf("enter the element for %d row,%d column:",i+1,j+1);
        scanf("%d",&m[i][j]);
    }
}

void multiplication(int a[15][15],int b[15][15],int result[15][15],int r1,int c1,int r2,int c2){
    for (int i = 0; i < r1; ++i) 
    for (int j = 0; j < c2; ++j) 
    result[i][j] = 0;
    
    for (int i = 0; i < r1; ++i)
    for (int j = 0; j < c2; ++j)
    for (int k = 0; k < c1; ++k) {
    result[i][j] += a[i][k] * b[k][j];
    }
}

void display(int result[15][15], int row, int column) {

   printf("\nOutput Matrix:\n");
   for (int i = 0; i < row; ++i) {
      for (int j = 0; j < column; ++j) {
         printf("%d  ", result[i][j]);
         if (j == column - 1)
            printf("\n");
      }
   }
}
    

int main(){
    int a[15][15], b[15][15], result[15][15], r1,c1,r2,c2;
    printf("please enter the number of rows and columns for first array:");
    scanf("%d%d",&r1, &c1);
    printf("please enter the number of rows and columns for second array:");
    scanf("%d%d",&r2, &c2);
    
    while(c1 != r2){
    printf("error, the matrices cannot be multiplied,try again\n");
    printf("please enter the number of rows and columns for first array:");
    scanf("%d%d",&r1, &c1);
    printf("please enter the number of rows and columns for second array:");
    scanf("%d%d",&r2, &c2);
    }
    
     element(a ,r1 ,c1);
     printf("\n");
     element(b, r2, c2);
     
     multiplication(a,b,result,r1,c1,r2,c2);
     
     display(result,r1,c2);
     
}
