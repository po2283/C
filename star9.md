#include<stdio.h>

int main() {

	int N;
	scanf_s("%d", &N);

	int i, j;
	for (i = 0; i < N; i++) {
		for (j = 0; j < i; j++) {
			printf(" ");
		}
		for (j = 0; j < 2 * N - (1 + 2 * i); j++) {
			printf("*");
		}

		printf("\n");
	}

	for (i=N-1; i>0; i--) {
		for (j = i - 1; j > 0; j--) {
			printf(" ");
		}
		for (j = 2 * N - (2 * i - 1); j > 0; j--) {
			printf("*");
		}
		printf("\n");
	}
	return 0;

}
