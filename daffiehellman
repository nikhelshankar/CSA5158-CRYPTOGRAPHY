#include<stdio.h>
#include<math.h>
long long int power(long long int a, long long int b,
                                     long long int P)
{
    if (b == 1)
        return a;
    else
        return (((long long int)pow(a, b)) % P);
}
int main()
{
    long long int P, G, x, a, y, b, ka, kb;
    printf("Enter the value of P:");
    scanf("%d",&P);
    printf("The value of P : %lld\n", P);
    printf("Enter the value of G:");
	scanf("%d",&G); 
    printf("The value of G : %lld\n\n", G);
    printf("Enter the value of a:");
	scanf("%d",&a); 
    printf("The private key a for Alice : %lld\n", a);
    x = power(G, a, P); 
    printf("Enter the value of b:");
	scanf("%d",&b); 
    printf("The private key b for Bob : %lld\n\n", b);
    y = power(G, b, P);
    ka = power(y, a, P);
    kb = power(x, b, P);
    printf("Secret key for the Alice is : %lld\n", ka);
    printf("Secret Key for the Bob is : %lld\n", kb);
    return 0;
}
