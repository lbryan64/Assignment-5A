// Assignment 5A.cpp :

#include <iostream>
using namespace std;

int main()
{
    int years, start, stat;
    cout << "Enter the number of years: ";
    cin >> years;
    cout << "Enter the starting year: ";
    cin >> start;
    int moveableYear = 0;
    moveableYear = start;
    int arr1[year];
    for (int i = 0; i < years; i++) {
        cout << "Enter stat for year " << moveableYear << ": ";
        cin >> stat;
        arr1[i] = stat;
        moveableYear++;
    }
    int best = arr1[0];
    int i = 0;
    int counter = 0;
    for (i = 0; i < years; i++) {
        if (best < arr1[i]) {
            best = arr1[i];
            counter++;
        }
    }
    cout << "Best stat was " << best << " in year " << (start + (1 * counter)) << endl;
    int counter2 = 0;
    int worst = arr1[0];
    for (i = 0; i < years; i++) {
        if (worst > arr1[i]) {
            worst = arr1[i];
            counter2++;
        }
    }
    cout << "\nWorst stat was " << worst << " in year " << (start + (1 * counter2));
}


