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

