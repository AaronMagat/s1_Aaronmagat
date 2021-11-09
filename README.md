# s1_Aaronmagat


#include <iostream>
#include <string>

using namespace std;
int main()
{
    string name;
    string Lastname;
    string age;
    int location;
    char userInput;

    cout << "Enter your name and last name:  \n";
    getline(cin, name);
    cout << "Enter your age:  \n";
    getline(cin, age);


    cout << "Enter your location \n";
    cout << "Abu Dahbi for [1] \n Sharjah for [2] \n Ajman for [3] \n Dubai for [4] \n Ras Al Khaimah for [5] \n Umm Al Quwain for [6] \n Fujairah for [7] \n Al Ain for [8] \n Other for [9]" << endl;
    cin >> location;
    switch (location)
    {
    case 1:
        cout << location << " Abu Dhabi, transportation charges are AED 1000\n";
        break;
    case 2:
        cout << location << " Sharjah, transportation charges are AED 500\n";
        break;
    case 3:
        cout << location << " Ajman, transportation charges are AED 390\n";
        break;
    case 4:
        cout << location << " Dubai, transportation charges are AED 650\n";
        break;
    case 5:
        cout << location << " Rak, transportation charges are AED 250\n";
        break;
    case 6:
        cout << location << " Umm Al Quwain, transportation charges are AED 300\n";
        break;
    case 7:
        cout << location << " Fujairah, transportation charges are AED 300\n";
        break;
    case 8:
        cout << location << " Al Ain, transportation charges are AED 1000\n";
        break;
    case 9:
        cout << location << " Other, No transportation available\n";
        return 0;
    default:
        cout << "Invalid input. \n";
    }
    
    cout << "Do you want to avail the transportation? Yes for [Y] No for [N]\n";
    cin >> userInput;

    if (userInput == 'Y'|| userInput == 'y')
    {
        cout << "Confirmed" << endl;
    }
    else if (userInput == 'N' || userInput == 'n')
    {
        cout << "Cancelled" << endl;
    }
    else
    {
        cout << "Incorrect input" << endl;
    }
    return 0;

}

