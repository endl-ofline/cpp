# hello-world

// program that takes in five ages, works out the average and outputs it along with how many are above/below said average.

#include <iostream>
using namespace std;

int main()
{
	int ages[5];
	int placeholder = 0;

	for (int placeholder = 0; placeholder < 5; placeholder++)
	{
		cout << "Enter an age: ";
		cin >> ages[placeholder];
	}

	int mean = 0;
	int result = 0;

	mean = ages[0] + ages[1] + ages[2] + ages[3] + ages[4];
	mean = mean / 5;
	cout << endl << "The average is: " << mean << "." << endl;

	int above_average = 0;
	int below_average = 0;
	for (int placeholder = 0; placeholder < 5; placeholder++)
	{
		if (ages[placeholder] > mean)
		{
			above_average++;
		}
		else if (ages[placeholder] <  mean)
		{
			below_average++;
		}
		
	}
	cout << "There are " << above_average << " ages above the average." << endl;
	cout << "There are " << below_average << " ages below the average." << endl;

		return 0;
}