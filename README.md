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

#include <stdio.h> 
  
int main(void) { 

    int i;
    
    printf("Enter a number: ");
    
    scanf("%d", &i);
    
    if (i >= 0 && i <=60){ 
    
       printf("F"); 
       
    }
    
    else if (i >= 61 && i <=70){ 
    
       printf("D"); 
       
    }
    
    else if (i >= 71 && i <=80){ 
    
       printf("C");    
       
    }
    
    else if (i >= 81 && i <=90){ 
    
       printf("C");    
       
    }
    
    else if (i >= 91 && i <=100){ 
    
       printf("A");    
       
    }
    
    return 0;
    
} 
