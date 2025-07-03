#include <stdio.h>
#include <stdlib.h>

int main() {
int n;
printf("ingrese la cantidad de libros: ");
scanf("%i" ,&n);

char titulo[n][20];
char autor[n][20];
char genero[n][20];
int ISBN[n];
float precio[n];
int stock[n];
float ganancia[n];
int i;

for(i = 0; i < n; i++) {
printf("ingrese el titulo: ");
scanf(" %[^\n]" , titulo[i]);

printf("ingrese el autor: ");
scanf(" %[^\n]", autor[i]);

printf("ingrese el genero: ");
scanf(" %[^\n]", genero[i]);
       
printf("ingrese el ISBN: ");
scanf("%d", &ISBN[i]);

printf("ingrese el precio: ");
scanf("%f", &precio[i]);
if(precio < 0) {
printf("precio invalido");
}
printf("ingrese el stock: ");
scanf("%d" , &stock[i]);

printf("ingrese la ganancia: ");
scanf("%f" , &ganancia[i]);

}
system("CLS");

printf("TITULO \t\t AUTOR\t\tGENERO\t ISBN\t PRECIO\t  STOCK\t   GANANCIA\n");
for(i = 0; i < n; i++) {
printf("%s \t", titulo[i]);
printf("%s \t", autor[i]);
printf("%s \t", genero[i]);
printf("%d \t", ISBN[i]);
printf("%.2f \t", precio[i]);
printf("%d \t", stock[i]);
printf("%.2f \n", ganancia[i]);
}
return 0;
}
# .c32540377-Daniel-Guerrero-
