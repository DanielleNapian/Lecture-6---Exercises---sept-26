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
  
	  #include <stdio.h>
	  #include <math.h>

	double const PI = 3.14159265358979323846f;

	int main()
	{
		int choice = 0;
		printf("Select your shape:\n");
		printf("1. Triangle\n");
		printf("2. Rectangle\n");
		printf("3. Square\n");
		printf("4. Ellipse\n");
		printf("5. Circle\n");
		printf("6. Exit\n");
		do
		{
			printf("Choice: ");
			scanf("%d", &choice);

			if (choice == 1)
			{
				double a, b, c;
				printf("Enter length of three sides: ");
				scanf(% lf % lf % lf, &a, &b, &c);
				Triangle triang(a, b, c);
				printf("The area of triangle is %0.3lf\n", triang.getArea());
			}
			else if (choice == 2)
			{
				double l, w;
				printf("Enter length and width: ");
				scanf("%lf %lf" & l, &w);
				Rectangle rect(l, w);
				printf("The area of rectangle is %0.3lf\n", rect.getArea());
			}
			else if (choice == 3)
			{
				double s;
				printf("Enter sidelength: ");
				scanf("%lf", &s);
				Rectangle square(s);
				printf("The area of square is %0.3lf\n", square.getArea());
			}
			else if (choice == 4)
			{
				double a, b;
				printf("Enter the length of major and minor axis: ");
				scanf("%lf %lf", &a, &b);
				Ellipse ellip(a, b);
				printf("The area of ellipse is %0.3lf\n", ellip.getArea());
			}
			else if (choice == 5)
			{
				double r;
				printf("Enter the radius: ");
				scanf("%lf", &r);
				Ellipse circle(r);
				printf("The area of circle is %0.3lf\n", circle.getArea());
			}

		} while (choice != 6);
		return 0;

	}
