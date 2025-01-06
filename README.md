# algo1
// Algorithme qui lit une phrase,qui se termine par un point
#include <stdio.h>

int main()
    char caractere;
    int longueur = 0, nb_mots = 0, nb_voyelles = 0;
    int dans_un_mot = 0; // Indicateur pour savoir si on est dans un mot
    char voyelles[] = "aeiouyAEIOUY";

    printf("Veuillez entrer une phrase qui se termine par un point :\n");

        while (1)
    // Lecture d'un caractère
        caractere = getchar();

    // Vérification de la fin de la phrase
        if (caractere == '.')
            longueur++;
            end-if

        if (dans_un_mot)
            nb_mots++;
            end-if

    // Vérification si le caractère est une voyelle
        for (int i = 0; voyelles[i] != '\0'; i++)
            if (caractere == voyelles[i]) {
                nb_voyelles++;
            end-if

    // Gestion des mots
        if (isspace(caractere))
            if (dans_un_mot) {
                nb_mots++;
                dans_un_mot = 0;
            }
        else {
            dans_un_mot = 1;
        }
        end-if

    // Affichage des résultats
    printf("Longueur de la phrase : %d caractères\n", longueur);
    printf("Nombre de mots dans la phrase : %d\n", nb_mots);
    printf("Nombre de voyelles dans la phrase : %d\n", nb_voyelles);

    return 0;

    end
