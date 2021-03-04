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

Exercise 4

#include<stdio.h>

#include<math.h>

int main(void){

  float money1;
  
  int leftquarters, leftdimes, leftnickels, quarters, dimes, nickels;

  printf("Introduce an amount of money: ");
  
  scanf("%f", &money1);

  int indmoney = money1 * 100;
  
  quarters = indmoney / 25;
  
  leftquarters = indmoney % 25;
  
  dimes = leftquarters / 10;
  
  leftdimes = leftquarters % 10;
  
  nickels = leftdimes / 5;
  
  leftnickels = leftdimes % 5;
  
  printf("In %f$ there are %d quarters, %d dimes, %d nickels and %d pennies", money1, quarters, dimes, nickels, leftnickels);

  return 0;
}

Exercise 5

#include<stdio.h>

#include<math.h>

int main(void){

  int year, year1;
  
  printf("Introduce a year to know if it is a leap year: ");
  
  scanf("%d", &year);

  if ( ((year % 4) == 0 && (year % 100) != 0)|| (year % 400) == 0){
  
    printf("The year is a leap year");
    }
    
  else if ((year % 400) != 0 && (year % 100) == 0){
  
    printf("The year is not a leap year");
    }
    
  else{
  
    printf("The year %d is not a leap year", year);
    }
    
  return 0;
  
}

Exercise 6 

#include<stdio.h>

#include<math.h>

int main(void){

  float salary, nhours, hours, total, subtotal;

  printf("Introduce your salary per hour:");

  scanf("%f",&salary);

  printf("Introduce the hours you've worked this week:");

  scanf("%f",&hours);

  float mult = 1.5;

  
	if (hours <= 40) {

		total = hours * salary;

	}
	else {

		nhours = hours - 40;

		total = 40 * salary;

		total += nhours * (salary + (salary/2));

	}

  printf("Your weekly pay is: $%f\n", total);

  return 0;
}
