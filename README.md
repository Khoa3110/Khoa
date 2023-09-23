#include <stdio.h>
#include <stdlib.h>

int main(int argc, char *argv[]) {
    int n, i,j;
    printf("Hay nhap so phan tu: ");
    scanf("%d", &n);
char choose;
    int arr[n];

    for(i = 1; i <= n; i++) {
        printf("Hay nhap phan tu N[%d]: ", i);
        scanf("%d", &arr[i]);
    }


				do {
		printf("\n1. Ban co muon hoan doi vi tri thanh giam gian ");
		printf("\n2. Ban khong muon hoan doi vi tri ");
		printf("\n Vui long chon: ");
		fflush(stdin);fflush(stdout);
		scanf("%c", &choose);
		
		switch(choose) {
			case '1': { int tg;
 
    for( i = 0; i < n - 1; i++){
        for( j = i + 1; j < n; j++){
            if(arr[i] < arr[j]){
                
                tg = arr[i];
                arr[i] = arr[j];
                arr[j] = tg;        
            }
        }
    }
printf("\nKet qua sap xep: ");
				for(i=0;i<n;i++) {
					printf("%d ", arr[i]);
				}
				printf("\n");
				
				break;
			}
			case'2':{printf("Cac phan tu trong mang la: ");
    for(i = 1; i <= n; i++) {
        printf("%d ", arr[i]);
    }
				
				
				break;
			}}}
			while(choose != '2', choose != '1');
    return 0;
}
    
    printf("Cac phan tu trong mang la: ");
    for(i = 1; i <= n; i++) {
        printf("%d ", arr[i]);
    }
    
  int tg;
 
    for( i = 0; i < n - 1; i++){
        for( j = i + 1; j < n; j++){
            if(arr[i] < arr[j]){
                // Hoan vi 2 so a[i] va a[j]
                tg = arr[i];
                arr[i] = arr[j];
                arr[j] = tg;        
            }
        }
    }
printf("\nKet qua sap xep: ");
				for(i=0;i<n;i++) {
					printf("%d ", arr[i]);
				}
				printf("\n");
    return 0;
}

