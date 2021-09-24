# Pattern-code
Write a program that gets an integer, n, from the user and then prints n repetitions of the pattern: some A’s, some B’s, then a C. Each new repetition has one more A and one less B than the pattern before it. The first pattern has 1 A and n B’s. Example: if the number from the user is n=4, then the program prints: ABBBBCAABBBCAAABBCAAAABC
#include<stdio.h>

int main() {
    int n;
    printf("Enter n: ");
    scanf("%d", &n);
    
    int numA = 1;
    int numB = n;

    for(int i=0; i<n; i++){
       for(int j=0; j<numA; j++)
          printf("A");
       for(int k=0; k<numB; k++)
          printf("B");
       printf("C");

    numA++;
    numB--;

    } 
    printf("\n");
    return 0;
}
