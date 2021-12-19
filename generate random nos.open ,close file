#include <stdio.h>
#include<stdlib.h>
#include<time.h>

int main(void) {
    int arr[100];
    int i;
  // creating a FILE variable
  FILE *fptr;

  // integer variable
  int num;

  // open the file in write mode
  fptr = fopen("integers", "w");

  if (fptr != NULL) {
    printf("File created successfully!\n");
  }
  else {
    printf("Failed to create the file.\n");
    // exit status for OS that an error occurred
    return -1;
  }
  for (i = 0; i<=9;i++){
    arr[i]=(rand()%20)+1;
printf("arr[%d]=%d\n",i,arr[i]);

  }





  fclose(fptr);

  // open file for reading
  fptr = fopen("integers", "r");

  // display numbers
  printf("\nNumbers:\n");
  while ( (num = getw(fptr)) != EOF ) {
    printf("%d\n", num);
  }

  printf("\nEnd of file.\n");

  // close connection
  fclose(fptr);

  return 0;
}
