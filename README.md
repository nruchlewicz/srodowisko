# ROZWIAZANIA

Zadanie 1

```c
int main()
{
 int i;
 int tabela[]={1,2,4,6,12};
   for (i=4; i>=0; i=i-1)
     printf("%i",tabela[i]);
 return 0;
}
```

Zadanie 2 program, ktory wypisuje liczby od 1 do 1000.
```c
  main ()
 {
   int n;
   for (n=1; n<1001; n=n+1)
     { 
        printf("%i ",n);
       }
 }
```

Program, ktory wypisuje na akranie czesc
```c
  main ()
 {
    printf ("\n CZESC\n\n");
 }
```

//Program, ktory wypisuje na ekranie liczby od 1do15 co 1 i od 16 d0 31 co 2
```c
  main ()
 {
   int n,i;
   for (n=1; n<31; n=n+1)
     { 
       i=n*2;
       if (n<16) printf ("\naktualna liczba to:%i  ",n );
       
	 else printf("\naktualna liczba to:%i ",i);
       }
 }
 ```
 
 //wczytanie liczby z klawiatury i wypisanie jej kwadratu i szecianu
 ```c
main()
 {
   int a;
   printf("Podaj liczbe pierwsza\n");
   scanf("%i",&a);
   printf("Podana liczba to:%i ",a);
   printf("\nKwadrat liczby:%i ",a^2);
   printf("\nszescian liczby:%i ",a^3);
 

 }
 ```
suma kwadratow
```c
main()
{ 
  int a,b,c,d,e,f;
  for (a=0; a<10; a=a+1){
    for (b=0; b<10; b=b+1){
      c=(a*a);
      d=(2*a*b);
e=b*b;
      f=c+d+e;
      printf("%i ",f);
    } printf("\n");
}}

```
program, ktory wczytuje liczbe naturalna n i drukuje wartosc sumy kwadratow
```c
main()
 {
   int a,i,s;
   do{
   printf("Podaj liczbe naturalna");
   scanf("%d",&a);
   }while (a<0);
   s=0;
   for (i=0; i<=a; i=i+1){
     s=s+i*i;
 }
   printf("suma kwadratów wynosi:%d ",s);
 }
```
dzialania rozne 
```c
main ()
{ 
  int n1, n2, n3;
  n1= 5+3*8/2-3;
  printf("5+3*8/2-3=%i",n1);
  n2=2%2+2*2-2/2;
  printf("\nwynik=%i",n2);
  n3=2*4*(5+9/2);
  printf("\n2*4*(5+9/2)=%i",n3);

}
```

Program, ktory wypisuje dane z tabeli w odwrotnej kolejnosci
```c
int main()
{
  int tabela[]={1,2,4,6,12};
  int a;
  for( a=4; a>=0; a=a-1)
    {
      printf("\n%i",tabela[a]);
   
    }
  return 0;
}
```
program wypisujacy potegi liczby 2 za pomoca petli while i for
```c
 main()
{
  int i;
  i=1;
  while (i<=2010){
    printf("\n%i",i);
    i=i*2;
  }
  for(i=1; i<=2010; i=i*2)
    {
      printf("\n%i",i);
    }
}
```
LAB3:
1. program z zadeklarowana tablica 5 liczb calkowitych i wyslwietla jej zawartosc oraz zawartosc w odwrotnej kolejnosci.
```c
#include <stdio.h>
main ()
{
  int tab[]={1,3,7,8,9};
  int i;
  for (i=0; i<5; i++)
    {
      printf("\n%i",tab[i]);
    }
  printf("\n");
for (i=4; i>=0; i--)
    {
      printf("\n%i",tab[i]);
    }
}
```
2. wczytuje do uzytkownika dane piecioelementowej tablicy i wypisuje jej zawartosc  oraz zawartosc w odwrtnej kolejnosci

```c
#include <stdio.h>
main()
{
  int tab[5];
  int i;
printf("podaj 5 liczb do tabeli");
  for (i=0; i<5; i++)
    {   
scanf("%i",&tab[i]);
    }
  printf("Liczby w tabeli to: ");
  for (i=0; i<5; i++)
    {
      printf("%i ",tab[i]);
    }
  printf("\nLiczby w tabeli w odwrotnej kolejnosci to: ");
for (i=4; i>=0; i--)
    {
      printf("%i ",tab[i]);
    }
}
```
3. wczytuje od uzytkownika 5 elementow do tablicy i wyswitla ilosc parzystych liczb

```c
#include <stdio.h>
main()
{
  int tab[5];
  int i,a;
  a=0;
printf("podaj 5 liczb do tabeli");
  for (i=0; i<5; i++)
    {   
scanf("%i",&tab[i]);
    }
  for (i=0; i<5; i++)
    {
      if ((tab[i]%2)==0) a=a+1;
      else a=a;
    }
  printf("Liczba parzystych elementów tablcy to: %i", a);
  a=0;
}
```

4.zadeklarowane 2 5-elementowe tab, wczytuje do 1 tab, a nastepnie przekopiuje powiekszone dwukrotnie dane do drugiej tab.

```c
#include <stdio.h>
main()
{
  int tab[5];
  int tablica[5];
  int i,a;
  a=0;
    printf("podaj 5 liczb do tabeli");
     for (i=0; i<5; i++)
       {   
       scanf("%i",&tab[i]);
       }
 printf("Liczby powiekszone dwukrotnie to: ");
  for (i=0; i<5; i++)
    {
      a=tab[i]*2;
      printf("%i ",a);
    }
}
```

5. wczytuje dane do 5-elementowej tab, a nastepnie wyswietla najwiekszy element.

```c
#include <stdio.h>
main()
{
 int tab[5];
 int i,a;
 a=0;
    printf("podaj 5 liczb do tabeli\n");
     for (i=0; i<5; i++)
       {   
       scanf("%i",&tab[i]);
       }
     for (i=0; i<5; i++){
       if (tab[1]>tab[2] && tab[1]>tab[3] && tab[1]>tab[4] && tab[1]>tab[5]) a=tab[1];
	 else if(tab[2]>tab[3] && tab[2]>tab[4] && tab[2]>tab[5]) a=tab[2];
	 else if(tab[3]>tab[4] && tab[3]>tab[5]) a=tab[3];
	 else if(tab[4]>tab[5]) a=tab[4];
	 else a=tab[5];
     }
printf("%i ",a);
}
```

6. zadeklarowana tab 5-elementow i uzupelni kolejnymi potegami liczby2 i wyswietli;

```c
#include <stdio.h>
main()
{
  int tab[5];
  int i,a;
  a=2;
  for (i=0; i<5; i++)
    {
      tab[i]=a;
      a=a*2;
	}
  for (i=0; i<5; i++)
    {
      printf("%i ", tab[i]);
    }
}
```

7. wczytuje od uzytkownika dane do tab i wyswietla ich sume.

```c
#include <stdio.h>
main()
{
  int tab[5];
  int i,suma;
  suma=0;
  printf("uzupelnij tabele:\n");
  for (i=0; i<4; i++)
    { 
      scanf("%i ",&tab[i]);
    }
  for (i=0; i<4; i++)
    {
      suma=suma+tab[i];
    }
  printf("Suma elementow w tablicy to: %i",suma);
}
```

8. zadeklarowane 2 5-elementowe tab, wczytuje do 1 tab, a nastepnie przekopiuje dane do drugiej tab.

```c
#include <stdio.h>
main()
{
  int tab[5];
  int tablica[5];
  int i,a;
  a=0;
    printf("podaj 5 liczb do tabeli");
     for (i=0; i<5; i++)
       {   
       scanf("%i",&tab[i]);
       }
 printf("Liczby w tabeli to odwrotnie: ");
  for (i=4; i>=0; i--)
    {
      a=tab[i];
      printf("%i ",a);
    }
}
```

9. wczytuje od uzytkownika 5-elementowa tab i przestawia pierwszy i ostatni element i wyswietla

```c
#include <stdio.h>
main()
{
  int tab[5];
  int i,tmp;
  tmp=0;
  printf("uzupelnij tablice:\n ");
  for (i=0; i<5; i++)
    {
      scanf("%i",&tab[i]);
    }
  tmp=tab[0];
  tab[0]=tab[4];
  tab[4]=tmp;
  for (i=0; i<5; i++)
    {
      printf("%i ",tab[i]);
    }
}
```

10. 2 tablice, jedna 5-elem, druga 10elem. Pobiera dane od użytkownika do pierwszej przekopiuje dwa razy dane z pierwszej do drugiej i wyswietli.

```c
#include <stdio.h>
main()
{
  int tab[5];
  int tabe[10];
  int i,j;
  printf("uzupelnij tablice: \n");
  for (i=0; i<5; i++)
    {
      scanf("%i ",&tab[i]);
    }
  i=0;
  for (j=0; j<10; j++)
    {
      if (tab[i]>tabe[j]){ tabe[j]=tab[i];
       printf("%i ",tabe[j]);
       i++;}
      
      else i=0; printf("%i ",tabe[j]); 
    }}
```

Zadanie 12/13. Program wczyta od uzytkownika dane 5-elementowej tab liczb całkowitych, a następnie wypize jej najmniejszy / największy element. 

```c
#include "stdio.h"
main()
{
int i, n, wynik;
int a[5];

for (i=0; i<5; i++)
{
printf("Podaj %i element ", i);
scanf("%d", &a[i]);
}
wynik=a[1];
for (i=0; i<5; i++) {
 if (wynik>a[i])
 {
wynik=a[i];
 }
}
printf("Najmniejszy element w tablicy to %d\n", wynik);
wynik = a[1];
for (i=0; i<5; i++){
 if (wynik<a[i])
 {
 wynik = a[i];
 }
}
printf("Najwiekszy element w tablicy to %d\n", wynik);

}
```
#Lab4

Program, sprawdzajajacy czy dana liczba jest pierwsza.
```c
# include <stdio.h>
main()
{
  int a,i,b;
  printf("Podaj liczbe: ");
  scanf ("%i",&a);
  b=0;
  for (i=1; i<=a; i++){
    if (a%i==0) 
      b=b+1;
  }
    if (b==2) printf("podana liczba jest pierwsza");
    else printf("Podana  liczba nie jest liczba pierwsza");
  
} 
```
program, ktory wypisuje wszystkie dzielniki dla podanej liczby
```c
#include <stdio.h>
main ()
{
  int a,i;
  printf("Podaj liczbe: ");
  scanf("%i",&a);
  for (i=1; i<=a; i++){

    if (a%i==0) printf("\nDzielnik:%i",i);
    else printf(" ");
      }
}
```
Program, ktory dla liczby , podanej z klawiatury oblicza najmniejsza liczbe n taka, ze 1+2+3+...+n>=m.
```c
#include <stdio.h>
main()
{
  int m,i,suma;
  printf("podaj liczbe M: ");
  scanf("%i",&m);]
//za pomoca petli for.
  suma=0;
  for (i=0; suma<=m; i++) {
    suma=suma+i;
    if (suma>=m) printf("%i\n",i);
    else printf("");
  }
//za pomoca petli while.
  suma=0;
  i=0;
  while (suma<=m)
	{
	 suma=suma+i;
	 if (suma>=m) printf("%i",i);
	 else i++;
		}
}
```

#ZAMIANA  LICZB Z SYSTEMU "10" na "2"

```c
#include <stdio.h>
 int main(){
 	
    int liczba,b,i,j;
 	b=0;
 	i=0;
 	j=0;
        printf("Podaj liczbe dziesietna   \n");
 	scanf("%d",&liczba);
 	printf("\n");
     int tablica[50];
 
while (liczba>0) {
 b=liczba%2;
 if (b==1) (tablica[j]=1);
   if (b==0) (tablica[j]=0);
 liczba=liczba/2;
 j++;
}
printf("system dwojkowy: ");
for (i=j-1; i>=0; i=i-1){
printf("%i",tablica[i]);
}
return 0;
}
```
