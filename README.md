' project-for-system-bank '
*******************************************************************************

 #include<iostream>
#include<string >
#include <stdlib.h>
using namespace std;
struct hotel
{
	string name[1000];
	string add[10000];
	string type[10000];
	string nationality[10000];
	int num_card[10000];
	int long num_phon[10000];
	int id[10000];
	int num_room[10000];
	int num_day[10000];
	int price_day;










};
int x;
int postion[1000] = { 0 };
hotel h;
void set_data();
void p();
void change();
void cheek();

int main()
{

	cout << "enter how manay number custmore:" << endl;
	cin >> x;
	cout << "enter day price:" << endl;
	cin >> h.price_day;
	

	 set_data();
	// change();
	cheek();
	p();








}

void set_data()
{

	

	
	for (int i = 0;i < x;i++)
	{
		cout << "enter all data for custmaore:  " << i + 1 << endl << endl << endl;
		
			cout << "   enter name:  " << endl << endl;
			cin >> h.name[i];

			cout << " enter address : " << endl << endl;
			cin >> h.add[i];
		
	
			cout << " enter type sex : " << endl << endl;
			cin >> h.type[i];

		
			cout << "   enter nationilty: " << endl << endl;
			cin >> h.nationality[i];



			cout << "   enter number card:  " << endl << endl;
			cin >> h.num_card[i];


			cout << "  enter number phon : " << endl << endl;
			cin >> h.num_phon[i];

			cout << "  enter  num room: " << endl << endl;
			cin >> h.num_room[i];
			cout << "enter postion room if enter 1:>>revresed of 0:>>not revresed:" << endl;
			cin >> postion[i];

		

			cout << "   enter id:  " << endl << endl;

			cin >> h.id[i];
			cout << "   enter number day: " << endl << endl;
			cin >> h.num_day[i];
		

	}







}

void p()
{

	for (int i = 0;i < x;i++)
	{
		cout << "all the data:   " << i + 1 << endl;

		cout << "name:" << h.name[i] << endl;
		cout << "address:" << h.add[i] << endl;
		cout << "type sex:" << h.type[i] << endl;
		cout << "nationilty:" << h.nationality[i] << endl;
		cout << "num card:" << h.num_card[i] << endl;
		cout << "num phon:" << h.num_phon[i] << endl;
		cout << "id:" << h.id[i] << endl;
		cout << "num day:" << h.num_day[i] << endl;
		cout << "num room:" << h.num_room[i] << endl;


		cout << "**********************************************" << endl << endl;











	}







}


void change()
{

	int y;
	int po;
	string n;
	int long card;
	int long phon;
	int day;
	cout << "enter how manay number change:" << endl;
	cin >> y;
	for (int i = 0;i < y;i++)
	{


		cout << "enter position:" << endl;
		cin >> po;
		cout << "enter name:" << endl;
		cin >> n;
		cout << "enter number card:" << endl;
		cin >> card;
		cout << "enter number phon:" << endl;
		cin >> phon;
		cout << "enter number days:" << endl;
		cin >> day;
		h.name[po] = n;
		h.num_card[po] = card;
		h.num_phon[po] = phon;
		h.num_day[po] = day;








	}










}


void cheek()
{

	int u;
	cout << "enter how manay numner cheek:" << endl;
	cin >> u;
	for (int i = 0;i < u;i++)
	{
		int w;
		cout << "enter postion:" << endl;
		cin >> w;
		if (postion[w]== 1)

			cout << "revresed:" << endl;

		else
			cout << "not revresed:" << endl;




	}


















}



