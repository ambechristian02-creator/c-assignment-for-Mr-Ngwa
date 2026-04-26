# c-assignment-for-Mr-Ngwa
#include <iostream>
using namespace std;

// Function to draw the diamond
void drawDiamond(int size) {
    // Upper half (including middle line)
    for (int i = 1; i <= size; i++) {
        // Print spaces
        for (int j = 1; j <= size - i; j++) {
            cout << " ";
        }

        // Print stars
        for (int k = 1; k <= (2 * i - 1); k++) {
            cout << "*";
        }

        cout << endl;
    }

    // Lower half
    for (int i = size - 1; i >= 1; i--) {
        // Print spaces
        for (int j = 1; j <= size - i; j++) {
            cout << " ";
        }

        // Print stars
        for (int k = 1; k <= (2 * i - 1); k++) {
            cout << "*";
        }

        cout << endl;
    }
}

int main() {
    int size;

    cout << "Enter the size of the diamond: ";
    cin >> size;

    drawDiamond(size);

    return 0;
}