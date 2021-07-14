#include <stdio.h>
#include <string.h>
 
int main()
{
    int smallest, secondsmallest;
    int array[100], size, i;
    printf("number of elements to be entered:");
    scanf("%d", &size);
    printf("Enter the elements:");
    for (i = 0 ; i < size; i++)
        scanf("%d", &array[i]);
    if (array[0] < array[1]) {
        smallest = array[0];
        secondsmallest = array[1];
    }
    else {
      smallest = array[1];
      secondsmallest = array[0];
    }
    for (i = 2; i < size; i++) {
        if (array[i] < smallest) {
        secondsmallest = smallest;
        smallest = array[i];
        }
        else if (array[i] < secondsmallest) {
            secondsmallest = array[i];
        }
    }
    printf("Second smallest element is %d", secondsmallest);
}
