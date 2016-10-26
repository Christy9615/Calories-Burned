# Calories-Burned


#include <iostream>
#include <iomanip>
using namespace std;

int main()
{
    //correct decimal to 2 and declare cal burned per minute
    const int DEC_DIGITS=2;
    const float cal = 3.6;
    // for loop of every 5 minutes calories burned
    for(int minute=5; minute<=30; minute+=5)
    {
        float calories;
        calories = cal * minute;
        
        cout <<"Total calories you burned for "<< minute <<" are ";
        cout << setprecision(DEC_DIGITS)<< fixed<< calories << " Cal."<< endl;
    }
    

    return 0;
}

