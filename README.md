# aula-p-1103
#include <stdlib.h>
#include <stdio.h>


int main()
{
    int escolha;
    float num1, num2, media, diferenca, produto, divisao;

    printf("\n\t   Escolha entre as opcoes 1 a 4: \n\t\n");
    printf("\n\t1- Media entre os numeros digitados:");
    printf("\n\t2- Diferenca entre o maior e o menor:");
    printf("\n\t3- Produto entre os numeros digitados: ");
    printf("\n\t4- Divisao do primeiro pelo segundo: \n\n\t");
    printf("\t\t\t Opcao: ");
    scanf("%d", &escolha);

    printf("\n\t1. Digite o 1o numero: ");
    scanf("%f", &num1);

    printf("\n\t2. Digite o 2o numero: ");
    scanf("%f", &num2);

    switch(escolha)
    {
        case 1:
            media=(num1+num2)/2;
             printf("\n\t==> Media = %.1f \n\t", media);
             break;

        case 2:
            if (num1>num2)
            {
                diferenca = num1-num2;
            }
                else
                {
                    diferenca = num2-num1;
                }
             printf("\n\t==> Diferenca = %.1f ", diferenca);
            break;

        case 3:
            produto = num1*num2;
             printf("\n\t==> Produto = %.1f ", produto);
             break;

        case 4:
            if (num2 == 0)
            {
                printf("\n\t==> Erro!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! ");
            }
                else
                {
                    divisao = num1/num2;
                    printf("\n\t==> Divisao = %.1f ", divisao);
                }

             break;

    }

}
