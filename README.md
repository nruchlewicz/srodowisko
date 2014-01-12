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
 /* main ()
 {
   int n,i;
   for (n=1; n<31; n=n+1)
     { 
       i=n*2;
       if (n<16) printf ("\naktualna liczba to:%i  ",n );
       
	 else printf("\naktualna liczba to:%i ",i);
       }
 } */
#include <stdio.h>
#include <stdlib.h>

int main ()
 {
   int n,i;
   i=0;
   for (n=1; n<31; n=n+1)
     {
       if (n<15) {printf ("\naktualna liczba to:%i  ",n );}

       else {  n=n+1;
           printf("\naktualna liczba to:%i ",n);
           } }
   return 0;
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
#LAB3

1. program z zadeklarowana tablica 5 liczb calkowitych i wyslwietla jej zawartosc oraz zawartosc w odwrotnej kolejnosci.

```c
#include <stdio.h>
int main()
{
    int i;
    int tab[]={1,3,7,8,9};
    printf("Tablica w podanej kolejności: ");
    for (i=0; i<5; i++)
        {
        printf("%i ",tab[i]);
        }
    printf("\nTablica w odwrotnej kolejnosci: ");
    for (i=4; i>=0; i--)
        {
        printf("%i ",tab[i]);
        }
    return 0;
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
/*#include <stdio.h>
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
*/
int main()
{
    int i, n;
    n=1;
    int tab[5];
        for (i=0; i<5; i++) // uzupełnienie tablicy potegami liczby 2.
        {
            n=n*2;
            tab[i]=n;
        }
        for (i=0; i<5; i++)
        {
            printf("\n%i element tablicy to: %i",i,tab[i]);
        }

    return 0;
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
#ZAMIANA LICZB Z SYSTEMU "10" na "2", "8" i "16"

```c
//zamiana liczby z systemu "10" na "2", "8", "16"
#include <stdio.h>
 int main(){
 	
   int liczba,b,i,j,liczba1, liczba2;
 	b=0;
 	i=0;
 	j=0;
        printf("Podaj liczbe dziesietna   \n");
 	scanf("%d",&liczba);
        liczba1=liczba;
	liczba2=liczba;
 	printf("\n");
     int tablica[50];
     //zamiana na system "2"
while (liczba>0) {
 b=liczba%2;
  if (b==1) (tablica[j]=1);
  if (b==0) (tablica[j]=0);
 liczba=liczba/2;
 j++;
}
printf("System dwojkowy:");
for (i=j-1; i>=0; i=i-1){
  printf("%i",tablica[i]);
}
//zamiana na system "8"
 int tab[50];
 b=0;
 i=0;
 j=0;
 while (liczba1>0){
   b=liczba1%8;
    if (b==0) (tab[j]=0);
    else (tab[j]=b);
   liczba1=liczba1/8;
   j++;
 }
 printf("\nsystem osemkowy: ");
 for (i=j-1; i>=0; i=i-1){
   printf("%i",tab[i]);
 }
 //zamiana na system "16"
 char tab1[50];
 b=0;
 i=0;
 j=0;
 while (liczba2>0){
   b=liczba2%16;
   if (b==0) (tab1[j]='0');
   if ((b>0)&&(b<10)) (tab1[j]=b);
   if (b==10) (tab1[j]='A');
   if (b==11) (tab1[j]='B');
   if (b==12) (tab1[j]='C');
   if (b==13) (tab1[j]='D');
   if (b==14) (tab1[j]='E');
   if (b==15) (tab1[j]='F');
   liczba2=liczba2/16;
   j++;
 }
 char z;
 printf("\nsystem szesnastkowy");
for (i=j-1; i>=0; i=i-1){
   printf("%c",tab1[i]);
 }
 printf("\n");
return 0;	
}
```

ZAD dokonczyc w domu:

```c
#include <stdio.h>
#include <stdlib.h>
int main (int argc, char *argv[])
{
  FILE *fout;

  int a,i;
  float c,d;
  float tab[11];
  c=0.0;
if ((fout=fopen("dane.dat", "w")) == NULL) {
    printf("Nie mogę otworzyć pliku do zapisu'\n");
    return 2;
 }
      for (i=0; i<11; i++)
	{
	  fprintf(fout,"%1.2lf\t",(tab[i]=c));
	  d=c*c;
	  fprintf(fout,"%1.2lf\n",(tab[i]=d));
       c=c+0.1;
	}
  fclose(fout);
 
  return 0;
 }
```
Lab6
========
Program Wczytuje 2 tablice liczb rzeczywistych taj samej dlugosci i drukuje ich iloczyn skalarny.
```c
#include <stdio.h>
main()
{
  int n,i;
  double a,b;
  printf("Podaj liczbe elementow tablicy: ");
  scanf("%i",&n);
  double tab1[n];
  double tab2[n];
  printf("\nUzupelnij tablice: %i elementów",n);
  for (i=0; i<n; i++)
  {
    scanf("%lf",&tab1[i]);
  }
  printf("Uzupelnij druga %i tablice: ",n);
  for (i=0; i<n; i++)
  {
    scanf("%lf",&tab2[i]);
  }
  a=0;
  b=0;
 for (i=0; i<n; i++)
  {
    a=(tab1[i]*tab2[i]);
    b=b+a;
    }
printf("Iloczyn skalarny wynosi: %lf",b);
}

```

Wczytuje 2 tablice liczb rzeczywistych i drukuje wynik ich porownania leksykalnego.
```c
#include <stdio.h>
main()
{
  int n,i;
  char a;
  printf("Podaj liczbe elementow tablic: ");
  scanf("%i",&n);
  double tab1[n];
  double tab2[n];
  printf("Uzupełnij pierwsza tablice %i elementowa: ",n);
  for (i=0; i<n; i++){
    scanf("%lf",&tab1[i]);
  }
  printf("Uzupelnij druga tablice %i elementowa: ",n);
  for (i=0; i<n; i++){
    scanf("%lf",&tab2[i]);
  }
  i=0;
  while (tab1[i]==tab2[i] && (i<n))    {
    i=i+1;
  }
  if (i<n){
    if (tab1[i]>tab2[i]) printf("Wieksza leksykalnie jest tablica 1");
    if (tab1[i]<tab2[i]) printf("Leksykalnie wieksza jest tablica 2");}
    else printf("Tablice sa rowne");
}
```

Szyfr Cezara
=======
```c
//SZYFR CEZARA
#include <stdio.h>
main ()
{
  int a,i;
  printf("Podaj ile chcesz znakow zakodowac: ");
  scanf("%i",&a);
  char tablica[a];
  printf("Podaj to co chcesz zakodowac (duze litery!):");
  for(i=0; i<=a; i++){
    scanf("%c",&tablica[i]);
    // tablica[i]=getchar();
  }
  //szyfrowanie
  for (i=1; i<=a; i++){
    tablica[i]=65+(tablica[i]-62)%26;
    printf("%c",tablica[i]);
  }
  //deszyfrowanie
  printf("\n");
  for (i=1; i<=a; i++)
    {
      tablica[i]=65+(tablica[i]+62)%26;
      printf("%c",tablica[i]);
    }
}
```


Lab 6.
=======
1. Instrukcja switch
```c
#include <stdio.h>
main ()
{
  int n;
  printf("\nPodaj liczbe: ");
  scanf("%d",&n);
  switch (n)
    {
    case 0: printf("Zero\n");
    case 1:
    case 2: printf("Mala\n");
      break;
    case 3: 
    case 4: 
    case 5: printf("Srednia");
    case 6: printf("duza");
 
    }}
```

2. Program dziala do momentu nacisniecia 4, pyta uzytkownika o wybor, instrukcja switch.
```c
# include <stdio.h>
main ()
{
  int wybor;
  printf("1: wyswietl A\n2: wyswietl C\n3: wyswietl F\n4: koniec");
  printf("\nPodaj liczbe: ");
  scanf("%d",&wybor);
  while (wybor!=4){
  switch (wybor)
    {
    case 1: printf("A\n");
      break;
    case 2: printf("C\n");
      break;
    case 3: printf("F\n");
      break;
    case 4:  break;
    default: printf("podano zly znak");
    }
  printf("\nPodaj liczbe: ");
  scanf("%d",&wybor);
}
}
```
3. program,ktory wyswitla biezacy dzien tygodnia i pokazuje jaki dzien tygodnia bedzie za 100 dni.
```c
#include <stdio.h>
main()
{
  int a,b;
  printf("Jaki jest dzis dzien tygodnia?1-7 ");
  scanf("%d",&a);
  printf("dzis jest: ");
  switch (a)
    {
    case 1: printf("Poniedzialek\n");
      break;
    case 2: printf("wtorek\n");
      break;
    case 3: printf("sroda\n");
      break;
    case 4: printf("czwartek\n");
      break;
    case 5: printf("piatek\n");
      break;
    case 6: printf("sobota\n");
      break;
    case 7: printf("niedziela\n");
      break;
    default: printf("nie ma takiego dnia tygodnia!!");
    }
  b=(100%7)+a;
  printf("za 100 dni bedzie: ");
  switch (b)
    {
    case 8: printf("Poniedzialek");
      break;
    case 9: printf("wtorek");
      break;
    case 3: printf("sroda");
      break;
    case 4: printf("czwartek");
      break;
    case 5: printf("piatek");
      break;
    case 6: printf("sobota");
      break;
    case 7: printf("niedziela");
      break;
  
    }
}
```

4. Funkcja, ktora przyjmuje 1argument typu int n, a nastepnie wyswietla "dzien dobry" n razy
```c
#include <stdio.h>
int ile_razy (int n)
{
  scanf("%i",&n);
  return n;
}
main()
{
  int i,n;
  printf("Podaj liczbe n: ");
  n=ile_razy(n);
 for (i=0; i<n; i++)
    {
      printf("Dzien dobry\n");
    }
}
```

5.funkcja silnia
```c
#include <stdio.h>
int silnia (int n, int wynik, int i)
{
  wynik=1;
  printf("Podaj n: ");
  scanf("%i",&n);
  for (i=1; i<=n; i++)
    {
      wynik=wynik*i;
    }
 printf("%i\n",wynik);
}
main ()
{ 
  int n, i, wynik;
  silnia(n, wynik, i);
}
```
6.funkcja kalkulator
```c
#include <stdio.h>
float oblicz (float lewy, char op, float prawy, float wynik)
{
printf("Podaj operacje: ");
  scanf("%c",&op);
  printf("Podaj lewy: ");
  scanf("%f",&lewy);
  printf("Podaj prawy: ");
  scanf("%f",&prawy);
  switch (op)
    {
   case '+': wynik=lewy+prawy; return wynik;
   case '-': wynik=lewy-prawy; return wynik;
   case '*': wynik=lewy*prawy; return wynik;
   case '/': wynik=lewy/prawy; return wynik; 
   default : printf("blad"); break;
    }
}
main ()
{
  float lewy, prawy, wynik;
  char op;
  printf("%3.3f",oblicz(lewy, op, prawy, wynik));
}
```

7. tablica 100 losowych liczb, wyswietla najwiekszy element

```c
#include <stdio.h>
main()
{
  int tab[100];
  int i,e;
  for(i=0; i<100; i++)
    {
      e=rand();
         printf("%d\n",(tab[i]=e));
    }
 int max = tab[0];
 for (i=0; i<100; ++i){
    if(tab[i] > max)
      max =tab[i];
 }
  printf("Najwieksza wartosc to:%d ",max);
}
 ```

8.tablica 100 liczb losowych od 0 do 10 i wyswietla ich sume. 

```c
#include <stdio.h>
main()
{
  int tab[100];
  int i,e;
  for(i=0; i<100; i++)
    {
      e=(rand(10)%11);
         printf("%d\n",(tab[i]=e));
    }
  int suma=0;
  for (i=0; i<100; i++){
    suma=tab[i]+suma;
 }
  printf("suma wszyskich elementow tablicy to: %d",suma);
}
 ```        

#LAB7
zad1. Funcje 
```c
#include <stdio.h>
//funkcja wyswietla dzien dobry
void f1 ()
{
  printf("F1: dzien dobry\n");
}
//f. wyswietla dzien dobry, otrzymana w argumencie liczbę razy.
//f nie przekazuje żadnej wartosci.
void f2 (int a)
{
  int i;
  printf("F2: Podaj liczbe: ");
  scanf("%i",&a);
  for (i=0; i<a; i++)
    {
  printf("\ndzien dobry");
    }
}
//to co f2, a ponadto zwróci wartość (int) 0;
int f3 (int a)
{
  int i;
  printf("\nF3: Podaj liczbe: ");
  scanf("%i",&a);
  for (i=0; i<a; i++)
    {
  printf("\ndzien dobry");
    }
  return 0;
}
main()
{
  int a;
  f1();
  f2(a);
  f3(a);
}
```

Zad2. Dwie funkcje, pierwsza sprawdza czy otrzymany argument jest podzielny przez2, a druga czy jest podzielny przez 3. Zastosować te funcje w programie, który bedzie czytał z wejścia liczbę i stwierdzał czy jest ona podzielna przez 2, 3 i przez 6. Np. liczba 9 jest podzielna przez 3. Liczba 12 jest podzielna przez 2, 3 i 6.
```c
#include <stdio.h>

int dwa (int liczba)
{
  if (liczba%2==0) return 1;
  else return 0;
 }
int trzy (int liczba)
{
  if (liczba%3==0) return 1;
  else return 0;
 
}
main()
{
  int liczba;
  printf("Podaj liczbe calkowita: ");
  scanf("%i",&liczba);
  if (dwa(liczba)==1) printf("Liczba jest podzielna przez 2\n");
  if (trzy(liczba)==1) printf("Liczna jest podzielna przez 3\n");
  if (dwa(liczba)&&trzy(liczba)) printf("Liczba jest podzielna przez 6");
  else printf("");
} 
```
Zad3. a)Funkcja rekurencyjna liczaca silnie od liczby n=10.
```c
#include <stdio.h>
int silnia (int n)
{
  if (n==0) return 1; // ponieważ 0!=1.
  else return n*silnia(n-1); //funkcja wykonuje sama siebie, do czasu, aż n==0. Wtedy za n przyjmie wartość 1.
}
main()
{
  int n=10;
  printf("%i!=%i\n",n,silnia(n));
}
```
zad3. b)Funkcja rekurencyjna licząca silnię z n!. Gdzie n podaje użytkownik.
```c
#include <stdio.h>

int silnia (int n)
{
    if ((n==0) || (n==1)) return 1;
    else return n*silnia(n-1);
}
main()
{
    int n;
    printf("podaj liczbe n: ");
    scanf("%i",&n);
    printf("%i! = %i",n,silnia(n));
}
```

Zad4. Funkcja obliczająca NWD dwóch podanych w programie liczb. Za pomocą odejmowania. 
```c
#include <stdio.h>
int NWD (int a, int b)
{
  if (b==a) return a;
  else 
    if (b>a) return NWD(a,b-a); // NWD(a,b)=NWD(a, b-a)
  else 
    if (a>b) return NWD(a-b,b); // NWD(a,b)=NWD(a-b, b)
}
main()
{
  int a,b;
  printf("Podaj a: ");
  scanf("%i",&a);
  printf("Podaj b: ");
  scanf("%i",&b);
  printf("NWD liczb: %i, %i = %i\n",a,b,NWD(a,b));
}
```
Zad5. Funkcja obliczaj ca NWD dwóch podanych liczb za pomoca modulo. 
```c
#include <stdio.h>
int NWD (int a, int b)
{
  if (a*b==0) return a+b;
  else 
    if (b>a) return NWD(a,b%a);
  else 
    if (a>b) return NWD(a%b,b);
}
main()
{
  int a,b;
  printf("Podaj a: ");
  scanf("%i",&a);
  printf("Podaj b: ");
  scanf("%i",&b);
  printf("NWD liczb: %i, %i = %i\n",a,b,NWD(a,b));
}
```

Zad6. Funkcja obliczająca ciąg Fibonacciego z f(15).
```c
#include <stdio.h>
int f (int n)
{
  if (n==0) return 0; //f(0)=0;
  if (n==1) return 1; //f(1)=1;
  else return f(n-2)+f(n-1); //f(n+2)=f(n)+f(n+1);
}
main ()
{
  int n;
  n=15;
  printf("ciąg fibonacciego z 15 = %i",f(n));
}
```
Zad7. Funkcja obliczająca ciąg Fibonacciego z f(n), gdzie n podaje użytkownik. 
```c
#include <stdio.h>
int f (int n)
{
  if (n==0) return 0; //f(0)=0;
  if (n==1) return 1; //f(1)=1;
  else return f(n-2)+f(n-1); //f(n+2)=f(n)+f(n+1);
}
main ()
{
  int n;
  printf("Podaj liczbę: ");
  scanf("%i",&n);
  printf("ciąg fibonacciego z 15 = %i",f(n));
}
```

Zad8. Funkcja z dużą potęgą.
```c
#include <stdio.h>
double potega ( double x, int n)
{
  if (n==0) return 1.0;
  else if (n%2==0) return potega (x*x, n/2);
  else return x*potega(x*x,n/2);
}
main ()
{
  double x,n;
  x=2;
  n=10;
  printf("%3.3f",potega(x, n));  
}
/* wynik=1024. Ponieważ: potega(2.0, 10)=potega(4.0, 5)=4.0*potega(16.0, 2)=1024 */
```

Zad9. Napisać funkcję rekurencyjną obliczającą kwadrat liczby naturalnej(podanej przez uzytkownika) bez uzycia mnożenia w oparciu o własności:
0^2=0;
(n+1)^2=n^2+2n+1; 
```c
/*Napisać funkcję rekurencyjną obliczającą kwadrat liczby naturalnej bez uzycia mnożenia w oparciu o własności:
0^2=0;
(n+1)^2=n^2+2n+1; */
#include <stdio.h>

int kwadrat (int n)
{
  if (n==0) return 0;
  else return kwadrat(n-1)+(n-1)+(n-1)+1;
}
main ()
{
  int n;
  n=6;
  printf("%i do kwadratu= %i",n,kwadrat(n));
}

  printf("%i do kwadratu= %i",n,kwadrat(n));
}
```

#ZADANIA Dr. W. Bzyl - REKURENCJA
1. Napisać rekurencyjną implementację funkcji obliczającej n do potęgi k.

```c
#include <stdio.h>
#include <stdlib.h>
int potega (int n, int k)
{
    if (k==0) return 1;
    else return n*potega(n*n, k/2);
}
 main()
{
    int n,k;
    printf("Podaj liczbe: ");
    scanf("%d",&n);
    printf("\ndo potegi: ");
    scanf("%d",&k);
    printf("%d",potega(n, k));

}
```

2. Napisać funkcję rekurencyjną C(n,k) obliczającą współczynnik Newtona
n po k, czyli liczbę podzbiorów k-elementowych zbioru n-elementowego.

```c
#include <stdio.h>
#include <stdlib.h>
int newton(int n, int k)
{
    if ((k==0) || (n==k)) return 1;
    else return newton(n-1, k-1)+ newton(n-1, k);
}
int main()
{
    int n,k;
    printf("Podaj n ");
    scanf("%i",&n);
    printf("Podaj k: ");
    scanf("%i",&k);
    printf("Wspolczynnik Newtona %i po %i wynosi: %i",n,k,newton(n, k));
    return 0;
}
```
#LAB8

1. Program z funkcją, która rozkłada podaną liczbę n<=1 na czynniki pierwsze. Wersja rekurencyjna.

```c
#include <stdio.h>
#include <stdlib.h>
#define DUZO 1000
int k, cz[DUZO];
void czynn (int n, int dzielnik)
{
  if (n%dzielnik==0){
    cz[k]=dzielnik;
    k=k+1;
    czynn (n/dzielnik, dzielnik);
  }
  else 
    if (dzielnik<n) czynn(n, dzielnik+1);
}
main()
{
  int n,i;
  printf("Podaj liczbe naturalna wieksza niz 1: ");
  scanf("%i",&n);
  while (n<=1)
    {
      printf("Podaj liczbe naturalna wieksza niz 1: ");
      scanf("%i",&n);
    }
  k=0;
  czynn (n,2);
  printf("\nCzynniki piwersze liczby %i : \n",n);
  for (i=0; i<k; i=i+1)
    printf(" %i",cz[i]);
  printf("\n");
}
```

2. Program z funkcją, która rozkłada podaną liczbę n<=1 na czynniki pierwsze. Wersja iteracyjna.

```c
#include <stdio.h>
#define DUZO 1000
 int cz[DUZO];
 int k;
int czynniki ( int dzielnik, int n){
   while (dzielnik<=n)
    {
  if (n%dzielnik==0)
    {
      cz[k]=dzielnik;
      k=k+1;
     n=n/dzielnik;
    }
  else
    if (dzielnik<n) 
dzielnik=dzielnik+1;
     }
}
main()

{
  int i, n, dzielnik;
  printf("Podaj liczbe naturalna wieksza niz 1: ");
  scanf("%i",&n);
  while (n<=1)
    {
       printf("Podaj liczbe naturalna wieksza niz 1: ");
       scanf("%i",&n);
    }
  k=0;
  dzielnik=2;
  czynniki(dzielnik,n);
  printf("\nk=%iCzynniki piwersze liczby %i : \n",k,n);
  for (i=0; i<k; i=i+1)
    {
      printf("%i",cz[i]);
      printf("\n");
    }
}
```

Zad3.Program oblicza pierwiastek kwardatowy z x z dokładnością do eps.

```c
#include <stdio.h>
#include <stdlib.h>

double pierw2pom (double a, double x, double b, double eps)
{
  if (b-a<eps) return a;
  else 
    {
      double c;
      c=((a+b)/2);
      if (x<c*c) return pierw2pom(a,x,c,eps);
      else 
        return pierw2pom(c,x,b,eps);
    }
}
double pierw2 (double x, double eps)
{
  return pierw2pom(0,x,1+x, eps);
}
main()
{
  double x=2.0, eps=0.3;
  printf("%f",pierw2(x, eps));
}
```
Zad4. program drukuje wszystkie rzeczywiste wartości zdefiniowanej w nim funkcji
funkcja począwszy od rzeczywistej wartości dol_x do rzeczywistej 
wartości gora_x z rzeczywistym krokiem krok_x.

Wywołanie w kompilatorze gcc -o ... -lm + deklaracja biblioteki <math.h>

```c
#include<stdio.h>
#include<math.h>

#define dol_x -0.9
#define gora_x 8
#define krok_x 0.1

double funkcja (double x)
{
  return (x*(3/27))-(2*x*(2/9))+(x/3)+2;
}

double  funkcja_b (double x) 
{
  return  log(x+1);
}
double funkcja_c (double x) 
{
  return x*sin(x) ;
}

int main () {
  double x;
  printf("\nTABLICOWANIE FUNKCJI:\n");
  printf("\n Argument |   Wartosc   ");
  printf("\n----------+-------------");
  for (x=dol_x; x<=gora_x; x=x+krok_x) //tablica warofści dla x*3/27 - 2*x*2/9 + x/3 + 2
    printf("\n %8.4lf | %10.4lf ", x, funkcja(x));
  printf("\n\n");
  
  printf("\nTABLICOWANIE FUNKCJI:\n");
  printf("\n Argument |   Wartosc   ");
  printf("\n----------+-------------");
  for (x=dol_x; x<=gora_x; x=x+krok_x)
    printf("\n %8.4lf | %10.4lf ", x, funkcja_b(x)); //tablica wartości dla log(x+1)
  printf("\n\n");
    
  printf("\nTABLICOWANIE FUNKCJI:\n");
  printf("\n Argument |   Wartosc   ");
  printf("\n----------+-------------");
  for (x=dol_x; x<=gora_x; x=x+krok_x)
    printf("\n %8.4lf | %10.4lf ", x, funkcja_c(x)); //tablica wartości dla f(x)=x*sin(x)
  printf("\n\n");

  return 0;
}
```

Zad.5 Program rysuje wykres (*)dla log(x+1),  9o) dla (x*(3/27))-(2*x*(2/9))+(x/3)+2; (@) dla x*sin(x);

```c
#include<stdio.h>
#include<math.h>

#define szer 90
#define wys 40
#define dol_x -0.9
#define gora_x 8
#define dol_y -2.5
#define gora_y 2.5

double  funkcja_b (double x) {
  return  log(x+1);
}

double funkcja (double x)
{
  return (x*(3/27))-(2*x*(2/9))+(x/3)+2;
}

double funkcja_c (double x) 
{
  return x*sin(x) ;
}

char  rysunek[szer][wys];


void  rysuj(int x, int y, char znak) {
  if (0<=x && x<szer && 0<=y && y<wys)
    rysunek[x][y] = znak;
}

int  interpoluj (double x, double a, double b, int n) {
  return  floor((x-a)*n/(b-a));
}

int  f_b (int x) {
  return
    interpoluj(
           funkcja_b( ((double)gora_x - (double)dol_x)/szer*x + dol_x),
                 dol_y,  gora_y,  wys
               );
}

int main () {
  int  x,y, poziom, pion;

  printf("\nWYKRES FUNKCJI :\n\n ");

  for (x=0; x<szer; x=x+1)
    for (y=0; y<wys; y=y+1)
      rysuj(x, y, ' ');

  pion = interpoluj(0, dol_x, gora_x, szer);   //rysuje oś pionową |
  for(y=0; y<wys; y=y+1)
    rysuj(pion, y, '|'); 

  poziom = interpoluj(0, dol_y, gora_y, wys);  //rysuje oś poziomą --
  for(x=0; x<szer; x=x+1)
    rysuj(x, poziom, '-'); 

  rysuj(pion, poziom, '+');  //rysuje + na środku układu współrzednych 

  for (x=0; x<szer; x=x+1)    //wykres dla funkcji_b(x)
    rysuj(x, f_b(x), '*');

 for (x=0; x<szer; x=x+1)     //wykres na funkcji(x).
    rysuj(x, funkcja(x), 'o');

 for (x=0; x<szer; x=x+1)    //wykres dla funckji_c(x).
    rysuj(x, funkcja_c(x), '@');

  for (y=wys-1; y>=0; y=y-1) {
    for (x=0; x<szer; x=x+1)
      printf("%c", rysunek[x][y]);
    printf("\n ");
  }

  printf("\n\n");

  return 0;
}
```
//Program rysuje wykres dla x*sin(x);

```c
#include<stdio.h>
#include<math.h>

#define szer 50
#define wys 30
#define dol_x -5
#define gora_x 5
#define dol_y -5
#define gora_y 5.0

double funkcja_c (double x) 
{
  return x*sin(x) ;
}

char  rysunek[szer][wys];

void  rysuj(int x, int y, char znak) {
  if (0<=x && x<szer && 0<=y && y<wys)
    rysunek[x][y] = znak;
}


int  interpoluj (double x, double a, double b, int n) {
  return  floor((x-a)*n/(b-a));
}

int  f_c (int x) {
  return
    interpoluj(
           funkcja_c( ((double)gora_x - (double)dol_x)/szer*x + dol_x),
                 dol_y,  gora_y,  wys
               );
}

int main () {
  int  x,y, poziom, pion;
  printf("\nWYKRES FUNKCJI :\n\n ");
  for (x=0; x<szer; x=x+1)
    for (y=0; y<wys; y=y+1)
      rysuj(x, y, ' ');
  //rysuje oś pionową |
  pion = interpoluj(0, dol_x, gora_x, szer);
  for(y=0; y<wys; y=y+1)
    rysuj(pion, y, '|');
  //rysuje oś poziomą -
  poziom = interpoluj(0, dol_y, gora_y, wys);
  for(x=0; x<szer; x=x+1)
    rysuj(x, poziom, '-');
  //rysuje + na środku układu wspołrzędnych 
  rysuj(pion, poziom, '+');
 
 for (x=0; x<szer; x=x+1) 
    rysuj(x, f_c(x), '@');

    for (y=wys-1; y>=0; y=y-1) {
    for (x=0; x<szer; x=x+1)
      printf("%c", rysunek[x][y]);
    printf("\n ");
  }
 
  printf("\n\n");

  return 0;
}
```

#Zad z funkcjami.

```c
#include <stdio.h>
#include <stdlib.h>
#define pi 3.14
int prosto (int a, int b)
{
    return a*b;
}
int delto (int c, int d)
{
    return (c*d)/2;
}
double stozek (int h, int r)
{
    return ((pi*r*r)*h)/3;
}
int main()
{
    int a,b,c,d,h,r;
    printf("\nPodaj bok a: ");
    scanf("%i",&a);
    printf("\nPodaj bok b: ");
    scanf("%i",&b);
    printf("\nPole prostokata o bokach %i, %i wynosi: %i",a,b,prosto(a,b));
    printf("\nPodaj przekatna deltoidu: ");
    scanf("%i",&c);
    printf("\nPodaj druga przekatna deltoidu: ");
    scanf("%i",&d);
    printf("\nPole deltoidu o przekatnych %i, %i wynosi: %i",c,d,delto(a,b));
    printf("\nPodaj promien podstawy stozka: ");
    scanf("%i",&r);
    printf("\nPodaj wysokosc stozka: ");
    scanf("%i",&h);
    printf("\nPole powiezchni stozka wynosi %3.2f",stozek(h,r));
    return 0;
}
```

f. sprawdza, czy podana liczba z zakresu od 0 do 1000 jest parzysa. 
```c
#include <stdio.h>
#include <stdlib.h>
void spr (int i)
{
       if (i%2==0) printf("Liczba %i jest parzysta",i);
       else printf("\nliczba %i nie jest parzysta",i) ;
}
main()
{
    int i;
    printf("Podaj i: ");
    scanf("%i", &i);
    while ((i<0)||(i>1000))
    {
    printf("Podaj i: ");
    scanf("%i",&i);
    }
    spr(i);
}
```

Program, który zawiera funkcję, która odpowiada czy podana liczba z zakresu od 1 do 10000 jest pierwsza.
```c
#include <stdio.h>
#include <stdlib.h>
double w;
int pierwsza (int p)
{
    int i;
 for(i=2; i<p; i++)
     {
          w=(p%i);
          if( w==0) {
              printf("%d  nie jest liczba pierwsza.\n", p);
              break;}
          else {
              printf("%d jest liczba pierwsza.\n", p);
              break;
          }
     }
}
main()
{
    int p;
    printf("Podaj liczbe: ");
    scanf("%i",&p);
    while ((p<0)||(p>1000))
    {
    printf("Podaj liczbe: ");
    scanf("%i",&p);
    }
    pierwsza(p);
}
```

Program, który zawiera funkcję, która oblicza wartość sumy liczb od 11 do 50 – użyć pętli for; użyć pętli while.
```c
#include <stdio.h>
#include <stdlib.h>
int suma (int suma)
{
    int i;
    suma=0;
    for (i=11; i<=50; i++)
     suma=i+suma;
     return suma;
}
int suma2 (int suma)
{
    int i=11;
    suma=0;
    while (i<=50)
    {
        suma=suma+i;
        i++;
    }
    return suma;
}
main()
{
   printf("Suma liczb od 11 do 50 wynosi: %i",suma(suma));
   printf("\nSuma liczb od 11 do 50 wynosi: %i",suma2(suma));
}
```

Program, który zawiera funkcję obliczającą silnię od 0 do 10. 
```c
#include <stdio.h>
#include <stdlib.h>
int silnia (int n)
{
    if ((n==0)||(n==1)) return 1;
    else return n*silnia(n-1);
}
main()
{
    int n;
    for (n=0; n<=10; n++)
    printf("%i!= %i\n",n,silnia(n));
}
```

#Lab9
1. Wskaźniki, przeanalizawać. 
```c

#include <stdio.h>
main ()
{
  int t[3];
  int i,j;
  int *adt;
  for (i=0, j=0; i<3; i++) t[i]=j++ +i;
  for (i=0; i<3; i++) printf("%d",t[i]);
  printf("\n");
  for (i=0; i<3; i++) printf ("%d",*(t+i));
  printf("\n");
  for (adt=t; adt<t+3; adt++) printf("%d",*adt);
  printf("\n");
  for (adt=t+2; adt>=t; adt--)
  printf("%d",*adt);
  printf("\n");
	 }
```

2. 
```c
#include <stdio.h>
main()
{
  int t[4]={10,20,30,40};
  int *ad[4]; //deklaracja wskaźnika do wartości. 
  int i;
  for (i=0; i<4; i++) ad[i]=t+i; /*przypisanie do tablicy ad[4] wartości z tablicy t[4]={10,20,30,40} */
  for (i=0; i<4; i++) printf("%d ",*ad[i]); /*wypisanie tablicy ad[i]*/
  printf("\n");
  printf("%d %d \n",*(ad[1]+1), *ad[1]+1); /*wypisanie wartośći, która znajduje się pod:  *(ad[1]*1), czyli ad[2] -> 30, oraz wypisanie wartości z *ad[1]+1-> 20+1= 21; 
}
```

