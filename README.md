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

Exercise 3 
#include <stdio.h>
#include <math.h>

int main(void) {

  int a, grade;
  
  printf("Give me the grade: ");
  
  scanf("%d", &a);
  
  grade = a % 10;
  
  if (a <=60){
  
    printf("F");
    
  }
  
  else if(a <= 70 && a >= 61){
  
    if (grade <= 3 && grade >= 1)
    
        {printf("D-");}
   
      else if (grade <= 7 && grade >= 4)
      
        {printf("D");}
        
      else if ((grade >= 8 && grade <= 9) || grade == 0 )
      
        {printf("D+");}
        
      else
        {printf("FATAL ERROR");}
  }
  
  else if(a <= 80 && a >= 71){
  
    if(grade <= 3 && grade >= 1){
      printf("C-");
    }
    else if(grade <= 7 && grade >= 4){
      printf("C");
    }
    else if((grade >= 8 && grade <= 9) || grade==0){
      printf("C+");
    }
    else {printf("FATAL ERROR");
    }
  }
  else if(a <= 90 && a >= 81){
  
    if(grade <=3 && grade >=1){
      printf("B-");
    }
    else if(grade <=7 && grade >=4){
      printf("B");
    }
    else if((grade >= 8 && grade <= 9) || grade==0){
      printf("B+");
    }
    else {printf("FATAL ERROR");
    }
  }
  
  else if(a <= 100 && a >= 91){
  
    if(grade <=3 && grade >=1){
      printf("A-");
    }
    else if(grade <=7 && grade >=4){
      printf("A");
    }
    else if((grade >= 8 && grade <= 9) || grade==0){
      printf("A+");
    }
    else {printf("FATAL ERROR");
    }
  }    
  return 0;
}
