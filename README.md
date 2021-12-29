#include <iostream>
using namespace std;
int main()
{
	for (int i = 0; i < 10; i++)
	{
		for (int j = 0; j < 10; j++)
		{
			if (i + j >= 9 && i >= j)
				cout << "^^^-";
			else
				cout << "    ";
		}
		cout << endl;
	}
	for (int i = 0; i < 7; i++)
	{
		for (int j = 0; j < 8; j++)
		{

			if (i >= 0 && i <= 2 && (j == 2 || j == 5))
				cout << "     ";
			else
				cout << "|###|";
		}
		if (i < 3)
		{
			for (int k = 0; k <= i; k++)
				cout << "^^^-";
		}
		else if (i < 7)
			for (int j = 0; j < 2; j++)
			{
				cout << "|###|";
			}
		cout << endl;
	}
}
