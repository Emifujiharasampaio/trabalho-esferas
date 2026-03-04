# trabalho-esferas
#include <iostream>
#include <stdio.h>
#include <math.h>

using namespace std;

int main()
{ //centro da esfera 1 e 2 e raio de cada
    float x1, y1, z1, r1;
    float x2, y2, z2, r2;
    float distancia , somaRaios2;
     printf (" digite x1, y1, z1, r1:");
     scanf ("%f %f %f %f" , &x1, &y1, &z1, &r1);
     
     printf (" digite x2, y2, z2, r2:");
     scanf (" %f %f %f %f", &x2, &y2, &z2, &r2);
     
     // distancia 
     distancia = (x2 - x1) * (x2-x1);
                  (y2-y1) * (y2-y1);
                  (z2-z1) * (z2-z1);
    // soma dos raios ao quadrado
    
    somaRaios2 = (r1 + r2) * (r1 + r2);
    
    if (distancia <= somaRaios2){
		  printf (" as esferas se colidem");
	} else { 
		printf (" as esferas nao se colidem");
	}
    return 0;       
}
