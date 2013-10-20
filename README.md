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
//suma kwadratow
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
