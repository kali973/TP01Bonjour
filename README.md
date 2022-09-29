Gilles COUTARD

Créer un fichier "bonjour.c" contenant les lignes suivantes :

int main() {
printf("Vive le C ! \n");
}

Compilez le fichier dans le Terminal en tapant : gcc -Wall -o bonjour bonjour.c.

Attention : N'oubliez pas le \n : il permet de vider le buffer et de passer à la ligne (sinon ça risque de ne rien afficher).

Suivant la version du compilateur vous obtiendrez une erreur de compilation ou des warnings car le code correct est:

#include <stdio.h>

int main() {
printf("Vive le C ! \n");
return 0;
}

Pourquoi faut-il rajouter ces 2 lignes ? 

Parce que main commence par int 