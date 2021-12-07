# s2
FACTORIAL:

#include <iostream>
using namespace std;

int main() {
	int name;
	cout << "Enter your full name:" <<endl;
	cin >> name;
	
	int y, z = 1;
	cout <<"Enter the number for factorial:" <<endl;
	cin >> y;
	while (cin.fail() || y <=0)
	{
	    cout <<"Invalid" <<endl;
	    cin.clear();
	    cin.ignore(1000, '\n');
	    cin >> y;
	}
	for (int x = 1; x<= y; x++)
	z = z * x;
	cout << "The factorial is:" <<z;
}	

///////////// multiplication

#include <iostream>
using namespace std;

int main() 
{
  int name;
	cout << "Enter your full name:" <<endl;
	cin >> name;
  int y, x = 0;
	cout << "Enter a number for the multiplication table: " <<endl;
	cin >> y;
	while (cin.fail())
	{
		cout << "Invalid command enter the number again: " << endl;
		cin.clear();
		cin.ignore(1000, '\n');
		cin >> y;
	}
	while (x <= 10)
	{
		cout << y << " x " << x << " = " << y * x << endl;
		x++;
	}

}

//////// exponent

#include <iostream>
using namespace std;

int main() 
{
  
    int exponent;
    float base, result = 1;

    cout << "Enter base and exponent:  ";
    cin >> base >> exponent;

    cout << base << "^" << exponent << " = ";

    while (exponent != 0) {
        result *= base;
        --exponent;
    }

    cout << result;
    
    return 0;
}
