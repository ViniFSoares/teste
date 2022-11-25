#include <stdio.h>
int main()
{
	int vetor[4];
	int valor;
	int div=1000;
	int x, i;
	
	printf("Digite um valor até 9999: ");
	scanf("%d", &valor);
	
	for (i=0 ; i<4 ; i++){
		
		vetor[i] = valor/ div;
		valor = valor - (vetor[i] * div);
		div = div/10;
		printf("Indice %d - %d\n", i, vetor[i]);
		
			   	
		}
	for (i=0, x=3; i<4 ; i++, x--){
		
		if (vetor[i] != vetor[x]){
		
		printf("\n\nNão é palindromo");
		break;
	}
	}
	if (i==4)
		printf ("\n\nÉ palindromo");
		
	return 0;
}
