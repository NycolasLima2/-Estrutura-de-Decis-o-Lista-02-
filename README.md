# -Estrutura-de-Decis-o-Lista-02- 

#include <stdio.h>
#include <stdlib.h>
#include <math.h>
#include <locale.h>

void exercicio27();
void exercicio28();
void exercicio29();
void exercicio30();
void exercicio31();
void exercicio32();
void exercicio33();
void exercicio34();
void exercicio35();
void exercicio36();
void exercicio37();
void exercicio38();
void exercicio39();
void exercicio40();
void exercicio41();


int main()
{setlocale (LC_ALL, "");
  int opcao;
    do{
    printf("----------Menu----------\n");
    printf("exe 27: Calculo da Diferenca entre Dois Numeros Inteiros");
    printf("\nexe 28: Classificação de Número Positivo ou Negativo");
    printf("\nexe 29: Cálculo da Média e Verificação de Aprovação");
    printf("\nexe 30: Cálculo da Média e Verificação de Aprovação com Exame");
    printf("\nexe 31: Resolução de Equação de Segundo Grau");
    printf("\nexe 32: Ordenação de Três Números Inteiros");
    printf("\nexe 33: Valores Divisíveis por 2 e 3");
    printf("\nexe 34: Valores Divisíveis por 2 ou 3");
    printf("\nexe 35: Maior e Menor Valor");
    printf("\nexe 36: Par ou Ímpar");
    printf("\nexe 37: Verificação de Faixa de Valor");
    printf("\nexe 38: Verificação de Valor Menor ou Igual a 3");
    printf("\nexe 39:Múltiplo de 3 e 5");
    printf("\nexe 40: Soma e Verificação (> 100)");
    printf("\nexe 41: Multiplicação e Verificação (> 30)");



    printf("\n\nDigite a opcao desejada: ");
    scanf("%d",&opcao);

    switch(opcao){
    case 27:
        exercicio27();
    break;
    case 28:
        exercicio28();
    break;
    case 29:
        exercicio29();
    break;
    case 30:
        exercicio30();
    break;
    case 31:
        exercicio31();
    break;
    case 32:
        exercicio32();
    break;
    case 33:
        exercicio33();
    break;

    case 34:
        exercicio34();
    break;
    case 35:
        exercicio35();
    break;
case 36:
        exercicio36();
    break;
    case 37:
        exercicio37();
    break;
    case 38:
        exercicio38();
    break;
    case 39:
        exercicio39();
    break;
    case 40:
        exercicio40();
    break;
    case 41:
        exercicio41();
    break;

    default:
    printf("Opcao invalida! Tente novamente.\n");
        }
    }
        while (opcao != 0);
    return 0;
    }





void exercicio27(){
float r;
int v, e;
printf("\n\n\ninsira 2 valores diferentes\n");
scanf("%d", &v);
scanf("%d", &e);
if(v > e){
r = v - e;

} else{
r = e - v;
}
printf("%.1f\n\n\n", r);


}
void exercicio28(){
float r;
int v;
printf("\n\n\ninsira 1 valor\n");
scanf("%d", &v);
if(v > 0){
printf("o valor %d positivo\n\n\n", v);

} else{
printf("o valor %d negativo\n\n\n", v);
}






}
void exercicio29(){
int v1, v2, v3, v4;
float R;
printf("insira suas notas duas ultimas 4 avaliacoes da materia ########\n");
scanf("%d\n", &v1);
scanf("%d\n", &v2);
scanf("%d\n", &v3);
scanf("%d", &v4);
R = (v1 + v2 + v3 + v4) / 4;
    if(R > 7){
    printf("sua media em materia ### foi de %2.f, ou seja, aprovado\n\n", R);

    } else {
    printf("sua media em materia ### foi de %2.f, ou seja, reprovado\n\n", R);
    }

}
void exercicio30(){
int v1, v2, v3, v4;
float R;
printf("insira suas notas duas ultimas 4 avaliacoes da materia ########\n");
scanf("%d\n", &v1);
scanf("%d\n", &v2);
scanf("%d\n", &v3);
scanf("%d", &v4);
R = (v1 + v2 + v3 + v4) / 4;
if(R > 7){
    printf("sua media em materia ### foi de %2.f, ou seja, aprovado\n\n", R);

    } else if (R >5.1 && R < 6.5) {
    printf("sua media em materia ### foi de %2.f, ou seja, exame\n\n", R);
    } else {
    printf("sua media em materia ### foi de %2.f, ou seja, reprovado\n\n", R);
    }



}
void exercicio31(){
int v1, v2, v3;
float R, R1,R2;
printf("\n\ninsira os valores para descobrir o delta, 3 valores A, B e C\n\n\n ");
scanf("%d", &v1);
scanf("%d", &v2);
scanf("%d", &v3);
/// pow(base,exp)
//valor para teste: 1, -3, -4
R = pow(v2, 2) - 4 *(v1*v3);
if (R >= 0){
R1 = (-v2 + pow(R,0.5))/2*v1;
R2 = (-v2 - pow(R,0.5))/2*v1;
printf("\npositivo: %.2f\n",R1);
printf("\nnegativo: %.2f\n",R2);
} else printf("não ha nada o que fazer com esse valor ridiculamente baixo\n");

}
void exercicio32(){
int V1, V2, V3,w;
printf("insira 3 valores diferentes");
scanf("%d", &V1);
scanf("%d", &V2);
scanf("%d", &V3);
if (V1 <= V2)
        {
            if (V2 < V3)
            {
                printf("A sequencia é %d %d %d\n", V1, V2, V3);
            }
            else
            {
                if (V1 <= V3)
                {
                    printf("A sequencia é %d %d %d\n",V1, V3, V2);
                }
                else
                {
                    printf("A sequencia é %d %d %d\n", V3, V1, V2);
                }
            }
        }
        else
        {
            if (V2 <= V3)
            {
                if (V1 < V3)
                {
                    printf("A sequencia é %d %d %d\n",  V2, V1 ,V3);
                }
                else
                {
                    printf("A sequencia é %d %d %d\n",V2, V3, V1);
                }
            }
            else
            {
                printf("A sequencia é %d %d %d\n ",V3, V2, V1);
            }
        }
    }
void exercicio33(){
    int v1, v2, v3, v4, a, b, c, d;

    printf("\n-----Valores Divisíveis por 2 e 3-----Exercicio 33\n");

    printf("Insira quatro valores numéricos inteiros: ");
    scanf("%d %d %d %d", &v1, &v2, &v3, &v4);

    a = v1;
    b = v2;
    c = v3;
    d = v4;

  if(v1 % 2 == 0 && v1 % 3 == 0) {
        printf("%d \n", v1);
    }

    if(v2 % 2 == 0 && v2 % 3 == 0) {
        printf("%d \n", v2);
    }

    if(v3 % 2 == 0 && v3 % 3 == 0) {
        printf("%d \n", v3);
    }

    if(v4 % 2 == 0 && v4 % 3 == 0) {
        printf("%d \n", v4);
    }
}
void exercicio34(){
    int v1, v2, v3, v4, a, b, c, d;
    
    printf("Insira um valor numérico inteiro: ");
    scanf("%d %d %d %d", &v1, &v2, &v3, &v4);

if (v1 % 2 == 0 || v1 % 3 == 0) {
        printf("%d\n", v1);
    }

    if (v2 % 2 == 0 || v2 % 3 == 0) {
        printf("%d\n", v2);
    }

    if (v3 % 2 == 0 || v3 % 3 == 0) {
        printf("%d\n", v3);
    }

    if (v4 % 2 == 0 || v4 % 3 == 0) {
        printf("%d\n", v4);
    }

    return 0;
}
void exercicio35(){
double V1, V2, V3, V4, V5;
    int Maor, Meor;

    printf("digite 5 valores\n");


    scanf("%lf", &V1);
    scanf("%lf", &V2);
    scanf("%lf", &V3);
    scanf("%lf", &V4);
    scanf("%lf", &V5);


    Maor = (int)V1;
    if (V2 > Maor) {
        Maor = (int)V2;
        if (V3 > Maor) {
            Maor = (int)V3;
            if (V4 > Maor) {
                Maor = (int)V4;
                if (V5 > Maor) {
                    Maor = (int)V5;
                }
            }
        } else {
            if (V4 > Maor) {
                Maor = (int)V4;
                if (V5 > Maor) {
                    Maor = (int)V5;
                }
            } else {
                if (V5 > Maor) {
                    Maor = (int)V5;
                }
            }
        }
    } else {
        if (V3 > Maor) {
            Maor = (int)V3;
            if (V4 > Maor) {
                Maor = (int)V4;
                if (V5 > Maor) {
                    Maor = (int)V5;
                }
            } else {
                if (V5 > Maor) {
                    Maor = (int)V5;
                }
            }
        } else {
            if (V4 > Maor) {
                Maor = (int)V4;
                if (V5 > Maor) {
                    Maor = (int)V5;
                }
            } else {
                if (V5 > Maor) {
                    Maor = (int)V5;
                }
            }
        }
    }
    printf("------%d Numero Maior------\n", Maor);


    Meor = (int)V1;
    if (V2 < Meor) {
        Meor = (int)V2;
        if (V3 < Meor) {
            Meor = (int)V3;
            if (V4 < Meor) {
                Meor = (int)V4;
                if (V5 < Meor) {
                    Meor = (int)V5;
                }
            }
        } else {
            if (V4 < Meor) {
                Meor = (int)V4;
                if (V5 < Meor) {
                    Meor = (int)V5;
                }
            } else {
                if (V5 < Meor) {
                    Meor = (int)V5;
                }
            }
        }
    } else {
        if (V3 < Meor) {
            Meor = (int)V3;
            if (V4 < Meor) {
                Meor = (int)V4;
                if (V5 < Meor) {
                    Meor = (int)V5;
                }
            } else {
                if (V5 < Meor) {
                    Meor = (int)V5;
                }
            }
        } else {
            if (V4 < Meor) {
                Meor = (int)V4;
                if (V5 < Meor) {
                    Meor = (int)V5;
                }
            } else {
                if (V5 < Meor) {
                    Meor = (int)V5;
                }
            }
        }
    }
    printf("------%d Numero Menor------\n", Meor);
}
void exercicio36(){
int numero;

    printf("Digite um número inteiro: ");
    scanf("%d", &numero);
    if (numero % 2 == 0) {
        printf("Resultado: Par\n");
    }
    else {
        printf("Resultado: Ímpar\n");
    }



}
void exercicio37(){
int valor;

    printf("Insira um valor inteiro entre 1 e 9: ");
    scanf("%d", &valor);
    if (valor >= 1 && valor <= 9) {
        printf("Resultado: Valor esta na faixa permitida\n");
    }
    else {
        printf("Resultado: Valor nao esta na faixa permitida\n");
    }

}
void exercicio38(){
int V;

printf("insira um valor\n");
scanf("%d", &V);
if( V <= 3) printf("este numero é menor que 3 ou 3");
else printf("este numero é menor que 3");

}
void exercicio39(){
    int numero;
    
    printf("Digite um número inteiro: ");
    scanf("%d", &numero);
    if (numero % 3 == 0 && numero % 5 == 0) {
        printf("Resultado: %d\n", numero);
    } else printf("ops: esse numero não é divisivel nos meu criterios");


}
void exercicio40(){
    float valor1, valor2, valor3, soma;

    printf("Digite o primeiro valor: ");
    scanf("%f", &valor1);
    scanf("%f", &valor2);
    scanf("%f", &valor3);
    soma = valor1 + valor2 + valor3;
    if (soma > 100) {
        printf("Resultado da soma: %.2f\n", soma);
    }





}
void exercicio41(){
    int numero, resultado;
    printf("Digite um número inteiro: ");
    scanf("%d", &numero);
    resultado = numero * 2;

    if (resultado > 30) {

        printf("Resultado: %d\n", resultado);
    }



}












