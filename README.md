#include <iostream>
using namespace std;
void add(int a, int b)
{
    int sum;
    sum = a + b;
    cout << sum << endl;
}
void difference(int a, int b)
{
    int diff;
    if (a > b)
    {
        diff = a - b;
    }
    else
    {
        diff = b - a;
    }
    cout << diff << endl;
}
void multiply(int a, int b)
{
    int pro;
    pro = a * b;
    cout << pro << endl;
}
void divide(int a, int b)
{
    float div;
   
    div = (float)a / float(b);
    cout << div << endl;
}
int main()
{
    int c, d;
    char operatoR;
    cout << "Enter two numbers " << endl;
    cin >> c;
    cin >> d;
    cout << "Enter operator" << endl;
    cin >> operatoR;
    switch (operatoR)
    {
    case '+':
        add(c,d);
        break;
    case '-':
        difference(c, d);
        break;
    case '*':
        multiply(c, d);
        break;
    case '/':
        divide(c, d);
        break;
    default:
        cout << "invalid operator" << endl;
        break;
    }
    return 0;
}
