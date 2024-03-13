# Naredba-goto
OSNOVNO O NAREDBI GOTO

Naredba goto omogućuje skokove unutar tijeka izvođenja.
- u jeziku su skokovi ograniceni na one unutar bloka, 
- čini kod izuzetno teškim za razumijeti i pratiti tijek izvođenja,
- uporaba goto opcenito se ne preporućuje i nije u skladu s  paradigmom strukturnog programiranja.

PREDNOSTI:
- Jednostavna implementacija, posebno u situacijama gdje su drugi mehanizmi složeni ili neadekvatni.
- Fleksibilnost u kontroli toka programa, omogućavajući specifične radnje koje se ne bi mogle postići drugim kontrolnim strukturama.

NEDOSTATCI:
- Poteškoće u održavanju koda - GOTO naredba može dovesti do nepreglednog koda, teškoća u razumijevanju i izmjenama.
- Teškoća u praćenju toka izvršavanja: Skakanje između različitih dijelova koda može otežati praćenje toka izvršavanja, što može dovesti do grešaka u logici programa.

PRIMJER 1:Napišite program u programskom jeziku C koji koristi goto naredbu za izvršavanje petlje. Program treba ispisati poruku "iteracija: X" gdje je X redni broj iteracije. Petlja treba izvršavati sve dok redni broj iteracije ne pređe 10.

#include <stdio.h>

int main(void) {
int i = 1;

petlja:
printf("iteracija: %d\n", i);
i++;
if (i <= 10)
goto petlja;

return 0;
}



