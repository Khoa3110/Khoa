#include <iostream>

/* run this program using the console pauser or add your own getch, system("pause") or input loop */
//ax+b=0
int main(int argc, char** argv) {
	int a,b;
	printf("\n Nhap gia tri cua A = ");
	scanf("\n%d", &a);
	printf("\n Nhap gia tri cua B = ");
	scanf("\n%d", &b);
	if(a==0, b==0){
		printf("Phuong trinh co vo so nghiem");
	} else {
		printf("Phuong trinh khong co nghiem");
	}	
	return 0;
}
