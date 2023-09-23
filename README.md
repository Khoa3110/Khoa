#include <stdio.h>
#include <stdlib.h>

int main(int argc, char *argv[]) {
char Chuoi[100];
   int a;
  
   printf("\nNhap mot chuoi bat ky: ");
   gets(Chuoi);
   a = strlen(Chuoi);
  
   printf("\nDo dai cua chuoi la: %d", a);
   
   
   //bai 2
char s1[100];
char s2[100];
int b,c,d;

printf("\nNhap chuoi s1: ");
gets(s1);
b = strlen(s1);
printf("\nNhap chuoi s2: ");
gets(s2);
c = strlen(s2);
strcat(s1, s2);
d = b+c;
printf("\n%s", s1);
printf("\nChuoi co do dai la %d", d);

//bai 3
char str[100];
int j;
int DoDai;
printf("\nNhap chuoi str: ");
gets(str);
DoDai = strlen(str);
printf(
"Hien thi str = ");
int i;
for(i=0; i<DoDai; i++){
	printf("\n%c", str(i));
}





    return 0;
}
