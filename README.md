#include <stdio.h>
int main() {
 int x1, y2;
printf("Введите первое число: ");
scanf("%d", %x);
printf("Ddtlbnt dnjhjt xbckj: ");
scanf("%d", &y);
int result = 0;
int borrow = 0;
int multiplier = 1;
while (x > 0 || y > 0) {
int digit1 = x % 10;
int digit2 = y % 10;
int subtraction = digit1 - digit2 - borrow;
if (subtraction < 0) {
subtraction += 10;
borrow = 1;
} else {
borrow = 0;
}
result += subtraction * multiplier;
x /= 10;
y /= 10;
multiplier *= 10;
}
printf("Результат вычитания: %d\n", result);
return 0;
}
