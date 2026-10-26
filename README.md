# my-first-website
My first website built with HTML, CSS and JavaScript.
#include <iostream>
using namespace std;
void InitialiserTableau(double tableau[9])
{
    for (int i = 0; i < 9; i++) {
        tableau[i] = 0;
    }
}
void RemplirTableau(double tableau[9]) {
    for(int i=0 ; i<9 ; i++ ) {
        cout<<"dommer une valeur "<< endl ;
        cin >> tableau[i] ;

    }
}
void AfficheTableau(double tableau[9]) {
    for (int i = 0; i < 9; i++)
    {
        cout<< tableau[i] <<" " ;
    }
    cout<< endl ;
}
void  SommeTableau(double tableau[9]) {
    int i,somme ;
    somme =0 ;
    for (i=0 ; i<9 ; i++ ) {
        somme = somme + tableau[i] ;
    }
    cout << somme << endl ;
}
void Cumul(double tableau[9]) {
    double sm ;
    sm=0 ;

    for ( int i=0 ; i<9 ; i++) {
        sm =sm +tableau[i] ;
        tableau[i] = sm ;
    }

}


int main() {
    double tableau[9];

    InitialiserTableau(tableau);

    cout << "Remplissage du tableau :" << endl;
    RemplirTableau(tableau);

    cout << "Tableau initial :" << endl;
    AfficheTableau(tableau);

    cout << "Calcul de la somme :" << endl;
    SommeTableau(tableau);

    cout << "Calcul du cumul :" << endl;
    Cumul(tableau);

    cout << "Tableau apres cumul :" << endl;
    AfficheTableau(tableau);

    return 0;
}
