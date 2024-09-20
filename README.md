//Simple-calculator-
//To do basic arithmetic operations 
#include <iostream>
using namespace std;

int main() {

  char op;
  int a,b;
  start:
  cout<<"enter two numbers"<<endl;
   cin>>a>>b;
  // choose the operator
  cout << "Enter an operator (+, -, *, /): ";
  cin >> op;

  switch (op) {
  case '+':
    cout << "Result = "<< (a + b) <<endl;
    break;
  case '-':
    cout << "Result = " << (a - b)<<endl;
    break;
  case '*':
    cout << "Result = " << (a * b)<<endl;
    break;
  case '/':
    cout << "Result = " << (a / b)<<endl;
    break;
  default:
    cout << "Invalid Operator"<<endl;
  }
  goto start;
  return 0; 
}