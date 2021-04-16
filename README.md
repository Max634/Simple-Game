#include <iostream>
#include <stdlib.h> // srand
using namespace std;

int main()
{
    int number = rand() % 100 + 1;
    int guess = 0;
    cout << number << endl;
    do {
        cout << "Guess the number from 1 to 100";
        cin >> guess;
        if (guess > number) { cout << "Too High.\n" << endl; }
        else if (guess < number) { cout << "Too low.\n" << endl; }
        else {
            cout << "That's right!" << endl;
            exit(0);
        }
    } while (number != guess);
    return 0;
} // main
