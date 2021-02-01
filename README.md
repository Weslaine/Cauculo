# Cauculo
Projeto de Calculo de Horario
#include <stdio.h>
   
int mintotal(int hora, int minuto) {

int r = (hora*60) + minuto;

return r;}

int main (){
  

int h1, m1, h2, m2,r1,r2, total; //variaveis declaradas

scanf ("%d%d", &h1, &m1); //armazendando valores da hora inicial

r1 = mintotal(h1, m1);

scanf ("%d%d", &h2, &m2);

r2 = mintotal(h2, m2);

total = r2-r1;

if (total < 0){

total +=1440; //calculo

printf ("%d minutos de diferenca!\n\n", total);} //impressão do resultado

else printf ("%d minutos de diferenca!\n\n", total); //impressão do resultado

return 0;

}
