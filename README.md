#include <stdio.h>
#include <stdlib.h>

int main(int argc, char *argv[]) {
int dataList[100];
	char choose;
int x,y,i,j, sum=0;
int index = 0;
	
	
	do {
		printf("\n1. Them phan tu N vao mang");
		printf("\n2. Hien Thi");
		printf("\n3. Tinh Tong");
		printf("\n4. Sap Xep");
		printf("\n5. Thoat");
		printf("\nChon: ");
		fflush(stdin);fflush(stdout);
		scanf("%c", &choose);
		switch(choose){
			case'1':{
			printf("\nNhap phan tu N  them: ");
				scanf("%d", &x);
				dataList[index++] = x;
				break;
			}
			case '2':{
				printf("Danh Sach la: ");
				for(i=0; i<index;i++){
					printf("%d", dataList[i]);
				}
				printf("\n");
				break;
			}

		case '3':{
			printf("Tong cua cac phan tu N la: ");
			for(i=0; i<index; i++){			
				sum = sum + dataList[i];
			}
			printf("%d", sum);
				printf("\n");
			
			
			break;
		}
		case '4':{
		for(i=0;i<index-1;i++) {
					for(j=i+1;j<index;j++) {
						if(dataList[i] > dataList[j]) {
							x = dataList[i];
							dataList[i] = dataList[j];
							dataList[j] = x;
						}
					}
				}
				printf("\nKet qua sap xep: ");
				for(i=0;i<index;i++) {
					printf("%d ", dataList[i]);
				}
				printf("\n");
			break;
		}
		case '5':{
			printf("\nTHOAT!!!");
			
			break;
		} default:{
		printf("\NHAP SAI!!!");
		break;
		}
	
;}}while(choose !='5');


    return 0;}

