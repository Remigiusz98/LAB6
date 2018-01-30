# LAB6

#include<iostream>
#include<conio.h>
#include<string>

using namespace std;

string usun_spacje(string tekst) {

	int ii = 0, n;

	string nowy;


	n = tekst.length();
	for (ii = 0; ii < n; ii++)
		if (tekst[ii] != ' ')
			nowy += tekst[ii]; //dodawanie stringow
	return nowy;
}



string odwroc(string tekst)
{
	int i = 0;
	int n;
	string kot;
	n = tekst.length();

	for (int i = 0; i < n; i++)
	{
		kot.insert(i, tekst, n - i - 1, 1); //miejsce wstawienia,tekst,co z tekstu,ile
	}


	return kot;



}



int main() {

	cout << "usun spacje:" << endl;
	string tekst;
	

	getline(cin, tekst);

	cout << usun_spacje(tekst);

	cout <<endl<< "odwroc wyraz:" << endl;
	string tekst2;
	getline(cin, tekst2);
	cout << odwroc(tekst2);

	_getch();
	return 0;
}

















