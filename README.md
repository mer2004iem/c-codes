# c-codes
#include<stdio.h>
struct calculator {
    int num1;
    char operator;
    int num2;
};
int main() {
    int result;
    struct calculator calc;
    scanf("%d",&calc.num1);
    scanf("%s",&calc.operator);
    scanf("%d",&calc.num2);
    switch(calc.operator) {
    case'+':
        result=calc.num1+calc.num2;
        break;
    case'-':
        result=calc.num1-calc.num2;
        break;
    case'*':
        result=calc.num1*calc.num2;
        break;
    case'/':
        result=calc.num1/calc.num2;
        break;
    }
    printf("%d",result);
}
