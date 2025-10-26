#include<stdio.h>
int main()
{
    float sub1,sub2,sub3,sub4,sub5,attendence_percentage,total,percentage;
    int remarks;
    char grade;
   printf("Enter sub1,sub2,sub3,sub4,sub5 marks\n");
   scanf("%f %f %f %f %f",&sub1,&sub2,&sub3,&sub4,&sub5);
   printf("Enter the attendence percentage\n");
   scanf("%f",&attendence_percentage);
   total = (sub1+sub2+sub3+sub4+sub5);
   percentage = total/5;
    printf("total percentage = %f\n",percentage);
    if(attendence_percentage < 75){
        printf("grade = F\n remarks = Fail\n");
    }
    else{
        if(percentage>= 45&&percentage<=45 && attendence_percentage){
            percentage += 5;
            if(percentage > 100)
            percentage = 100;
        }
        if (percentage >= 90){
            printf("grade = A+\nremarks = excellent\n");
        }
        else{
            if (percentage >80){
                printf("grade = A\nremarks = very good\n");
            }
            else{
                if (percentage > 70){
                    printf("grade = B\n remarks = good\n");
                }
                else{
                    if(percentage >60){
                        printf("grade = C\n remarks = average\n");
                    }
                    else{
                        if (percentage > 50){
                            printf("grade = D\n remarks =pass ");
                        }
                        else{
                            printf("grade = F\n remarks = fail");
                        }
                    }
                }
            }
        }
    }
    return 0;
}
