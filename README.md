# Exercises-chapter-6
Exercise 1 
#include <stdio.h>

#include <math.h>


int main(void) {

  float x1, y1, x2, y2, d, sumx, sumy, r;
  
  printf("Enter x1: ");
  
  scanf("%f", &x1);
  
  printf("Enter y1: ");
  
  scanf("%f", &y1);
  
  printf("Enter X2: ");
  
  scanf("%f", &x2);
  
  printf("Enter y2: ");
  
  scanf("%f", &y2);
  
  sumx = (x2 - x1);
  
  sumy = (y2 - y1);
  
  d = pow(sumx, 2) + pow(sumy, 2);
  
  r = sqrt(d);
  
  printf("The distance between 2 points is %f", r);
  
  return 0;
  
}

Exercise 2

