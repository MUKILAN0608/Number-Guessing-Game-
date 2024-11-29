#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;

int main() {
    srand(time(0));  
    int n = rand() % 100 + 1;  
    int i;  
    int c = 10;  
    int prev_diff = 101;  

    cout << "GUESS A NUMBER BETWEEN 1 TO 100!" << endl;

    for (int k = 1; k <= c; k++) {
        cout << "CHANCE " << k << " of " << c << " remaining." << endl;
        cout << "Enter your guess: ";
        cin >> i;

        if (i == n) {
            cout << "CONGRATULATIONS! YOU GUESSED THE NUMBER CORRECTLY!" << endl;
            cout << "GAME OVER" << endl;
            break;
        }
        
        if (k == c) {
            cout << "GAME OVER! You've run out of chances." << endl;
            cout << "The correct number was " << n << "." << endl;
            break;
        }

        if (i > n) {
            cout << "The number is too HIGH. Try again." << endl;
        } else {
            cout << "The number is too LOW. Try again." << endl;
        }

        int current_diff = abs(n - i);  
        if (current_diff < prev_diff) {
            cout << "You're getting WARMER!" << endl;
        } else if (current_diff > prev_diff) {
            cout << "You're getting COLDER!" << endl;
        }
        prev_diff = current_diff;  
    }

    return 0;
}
