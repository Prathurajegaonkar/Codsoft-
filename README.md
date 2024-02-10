# Codsoft-
2nd task :- Create simple calculator by using C++ programming language.

#include<iostream>
using namespace std;

// Function prototype
float add(float a, float b);
float subtract(float a, float b);
float multiply(float a, float b );
float divide(float a , float b);

int main() {
    float number1, number2;
    char op;

    cout << "Enter the first number: ";
    cin >> number1;
    cout << "Enter the second number: ";
    cin >>number2;

    cout << "Enter The operation (+, -, *, /): ";
    cin >> op;

    switch(op) {
        case '+':
            cout << "Result :- " << add(number1, number2);
            break;
        case '-':
            cout << "Result :- " << subtract(number1, number2);
            break;
        case '*':
            cout << "Result :- " << multiply(number1, number2);
            break;
        case '/':
            if (number2 == 0) {
                cout << "Cannot divide by zbro !";
            } else {
                cout << "Result :- " << divide(number1, number2);
            }
            break;
        default:
            cout << "Invalid operation !";
    }

    return 0;
}

// Function definitions
float add(float a, float b) { 
    return a + b;
}

float subtract(float a, float b) {
    return a - b;
}

float multiply(float a, float b) {
    return a * b;
}

float divide(float a, float b) {
    return a / b; 
}
