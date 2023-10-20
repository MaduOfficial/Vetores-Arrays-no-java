# Vetores-Arrays-no-java

Anotações de Vetores Arrays no java
                                                                      Vetores-Arrays-no-java

Arrays
.Estrutura de dados mais simples existente na maioria das linguagens de rogramação.
.Lista ordenada de dados.

Problema
.Armazenar a temperatura média diária por 1 ano

Solução?

double tempDia001 = 31.3;
double tempDia002 = 32;
double tempDia003 = 33.7;
double tempDia004 = 34;
double tempDia005 = 33.1;

Usar um vetor/array é muito parecido com uma planilha do Exel, mas suponha que nós estamos utilizando apenas uma coluna do Exel, por exemplo apenas a coluna
A, na primeira linha a gente coloca a primeira temperatura na segunda linha a temperatura do sedundo dia na teceira linha a temperatura do terceiro dia e
assim vai até a gente ter as 365 temperaturas, então a solução que quando a gente precisar armazenar uma lista de dados é utilizar os arrays, eles funcionam
como uma lista armazenada de dados, quando a gente cria no Java a gente vai especificar o que nós precisamos de 365 posições, então é como se o Java tivesse
criando ele vai na memória e vai reservar 365 lugares, uma curiosidade sobre os arrays isso é para ser c#, JavaScript, C, C++ e para o Java, toda vez que
nós formos trabalhar com Arrays com Vetores as posições de um Array elas são indicadas por índices que nós chamamos de index que é o índice o primeiro
índice ele sempre começa do 0 e então o primeiro posiçãO é no índice ) a segunda posição é no índice 1 então o que para a gente começa no 1 em certas
linguagens de programação como no Java começa do 0.
Como a gente iria organizar essas informações em um Array no Java, a gente iria usar a variável double porque essas informações são do tipo Double, e a
gente abre e fecha couchetes [] que é para indicar que esse tipo de dado é um Array, no Java os Arrays você recisa indicar o número de posições,

Tem gente que esceve o programa assim

double temp[];

Mas na boa prática java é assim

double[] temperaturas = new double[365];

Essa seria uma maneira da gente criar e inicializar um Array.

double[] temperaturas = new double[365];
		temperaturas[0] = 31.3;
		temperaturas[1] = 32;
		temperaturas[2] = 33.7;
		temperaturas[3] = 34;
		temperaturas[4] = 33.1;

você digita uma variável e logo em seguida colchetes [] para indicar que isso é um vetor/array e a posição e aí você pode colocar um valor lá dentro.

package com.madu.arrays;

public class Arrays {

	public static void main(String[] args) {
		
		double tempDia001 = 31.3;
		double tempDia002 = 32;
		double tempDia003 = 33.7;
		double tempDia004 = 34;
		double tempDia005 = 33.1;
		
		double[] temperaturas = new double[365];
		temperaturas[0] = 31.3;
		temperaturas[1] = 32;
		temperaturas[2] = 33.7;
		temperaturas[3] = 34;
		temperaturas[4] = 33.1;
		
		System.out.println("O valor da temperatura do dia 3 é: " + temperaturas[2]);
		
		System.out.println("O tamanho do array: " + temperaturas.length);
		
		System.out.println("Valores do array: ");
		
	    for (int i=0; i<temperaturas.length; i++) {
	    	System.out.println("O valor da temperatura do dia " + (i+1) + "é: " + temperaturas[i]);
		}

	}

}

Console:

O valor da temperatura do dia 3 ?: 33.7
O tamanho do array: 365
Valores do array: 
O valor da temperatura do dia 1?: 31.3
O valor da temperatura do dia 2?: 32.0
O valor da temperatura do dia 3?: 33.7
O valor da temperatura do dia 4?: 34.0
O valor da temperatura do dia 5?: 33.1
O valor da temperatura do dia 6?: 0.0
O valor da temperatura do dia 7?: 0.0
O valor da temperatura do dia 8?: 0.0
O valor da temperatura do dia 9?: 0.0
O valor da temperatura do dia 10?: 0.0
O valor da temperatura do dia 11?: 0.0
O valor da temperatura do dia 12?: 0.0
O valor da temperatura do dia 13?: 0.0
O valor da temperatura do dia 14?: 0.0
O valor da temperatura do dia 15?: 0.0
O valor da temperatura do dia 16?: 0.0
O valor da temperatura do dia 17?: 0.0

Não coloquei todos os 365 dias para não ficar muito longo

Quandoa gente cria um Array seja ele um Double, int, byte, short, float ou qualquer número do Java o valor inicial é 0, então o valor inicial de um
Double sempre vai ser 0 é por isso que ele tá imprimindo tudo 0 

package com.madu.arrays;

public class Arrays {

	public static void main(String[] args) {
		
		double tempDia001 = 31.3;
		double tempDia002 = 32;
		double tempDia003 = 33.7;
		double tempDia004 = 34;
		double tempDia005 = 33.1;
		
		double[] temperaturas = new double[365];
		temperaturas[0] = 31.3;
		temperaturas[1] = 32;
		temperaturas[2] = 33.7;
		temperaturas[3] = 34;
		temperaturas[4] = 33.1;
		
		System.out.println("O valor da temperatura do dia 3 é: " + temperaturas[2]);
		
		System.out.println("O tamanho do array: " + temperaturas.length);
		
		System.out.println("Valores do array: ");
		
	    for (int i=0; i<temperaturas.length; i++) {
	    	System.out.println("O valor da temperatura do dia " + (i+1) + "é: " + temperaturas[i]);
		}

	    for (double temp : temperaturas) {
	    	System.out.println(temp);
	    }
	}

}
