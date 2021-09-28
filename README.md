# Lecture-6---Exercises---sept-26
//slide 24 (Odd or Even)

	#include<iostream>
	using namespace std;

	int main() {
	    int n;

	    cout << "Enter an integer: ";
	    cin >> n;

	    if (n % 2 == 0)
		cout << n << "is even.";
	    else
		cout << n << "is odd.";

	    return 0;

	}
 //slide 25 (Number Checker)
 
	  #include <iostream>
	  using namespace std;

	  int main() {
		int num;
		cout << "Enter the number to checked: ";
		cin >> num;
		if (num >= 0)
			cout << num << "is a positive number.";
		else

			cout << num << "is a negative number.";

		return 0;

	}
  //slide 26 (Profit or Loss)

	  #include <iostream>
	  using namespace std;

	int main()
	{
	    float unitPrice, salesAmount, amount;
	    cout << "\nPlease Enter the Actual Product Cost = ";
	    cin >> unitPrice;
	    cout << "\nPlease Enter the Sale Price (or Selling Price) = ";
	    cin >> salesAmount;

	    if (salesAmount > unitPrice) {
		amount = salesAmount - unitPrice;
		cout << "\nProfit Amount = " << amount;
	    }
	    else if (unitPrice > salesAmount) {
		amount = unitPrice - salesAmount;
		cout << "\nLoss Amount = " << amount;
	    }
	    else
		cout << "\nNo Profit No Loss!";
	    cout << "\n";

	    return 0;

	}
  //slide 27 (Name the Shape)
  
		int shapeSides{};

	cout << "how many sides does your shape have?" << endl;
	cin >> shapeSides;

	if (shapeSides == 3) {
		cout << "This shape is a triangle" << endl;
	}else if (shapeSides == 4) {
		cout << "shape is a square" << endl;
	}
	else if (shapeSides == 5) {
		cout << "This shape is a pentagon" << endl;
	}
	else if (shapeSides == 6) {
		cout << "This shape is a hexagon" << endl;
	}
	else if (shapeSides == 7) {
		cout << "This shape is a heptagon or otherwise known as septagon" << endl;
	}
	else if (shapeSides == 8) {
		cout << "This shape is a octagon" << endl;
	}
	else if (shapeSides == 9) {
		cout << "This shape is a nonagon" << endl;
	}
	else if (shapeSides == 10) {
		cout << "This shape is a decagon" << endl;
	}
	else {
		cout << "This shape  cannot be identified with current limitations" << endl;
	}

