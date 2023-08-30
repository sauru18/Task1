#include<iostream>
#include<cstdlib>
#include<ctime>
using namespace std;
int main()
{
    srand((unsigned int)time(NULL));
    int number=(rand()%100)+1;
    int guess;
    int attempts=0;


    cout << "welcome to the number guessing game" << endl;
    cout <<"let guess number between 1 to 100" <<endl;


    do
    {
        cout <<"enter the guess:";
        cin >>guess;

        attempts++;

        if(guess>number)
        {
            cout <<"too high" <<endl;
        }
        else if(guess<number)
        {
            cout << "too low" <<endl;
        }
        else
        {
            cout <<"congrats you guess the number in: " <<attempts<<"attempts" <<endl;
            break;
        }
    } while (true);
    return 0;
    
    
}
