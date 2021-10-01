/****************************************************************************
 Zadanie 73 - Napisz program, ktory wypisze tabele znakow
    odpowiadaacych kolejnym kodom ASCII. Uwzgednij kody
    od 0 do 255. Ponizsze znaki kontrolne powinny byc przedstawione symbolicznie.
    kod skrot kod skrot
    0   nul     12   np
    7   bel     13   cr
    8   bs      26   eof
    9   ht      27   esc
    10  nl      127  del
    11  vt
****************************************************************************/

#include <stdio.h>

void wypisz() {

	int i;
	
	printf("kod\tASCII\r\n");
	for (i = 0; i <= 255; i++) {

		if (i != 0 && i != 7 && i != 8 && i != 9 && i != 10 && i != 11 && i != 12 && i != 13 && i != 26 && i != 27 && i != 127) {
			printf("%d\t%c\r\n", i, i);
		}
		if (i == 0) printf("%d\tnul\r\n", i);
		if (i == 7) printf("%d\tbel\r\n", i);
		if (i == 8) printf("%d\tbs\r\n", i);
		if (i == 9) printf("%d\tht\r\n", i);
		if (i == 10) printf("%d\tnl\r\n", i);
		if (i == 11) printf("%d\tvt\r\n", i);
		if (i == 12) printf("%d\tnp\r\n", i);
		if (i == 13) printf("%d\tcr\r\n", i);
		if (i == 26) printf("%d\teof\r\n", i);
		if (i == 27) printf("%d\tesc\r\n", i);
		if (i == 127) printf("%d\tdel\r\n", i);

	}

}

int main()
{
	printf("Program wypisuje tabele znakow odpowiadajacych kolejnym kodom ASCII.\nUwzglednione sa kody od 0 do 255.");


	wypisz();


	printf("\n\nKoniec programu.\n");
}