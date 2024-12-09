# Guess-a-number
#include<iostream>
#include<cstdlib> // it has rand functon
#include<ctime> 
using namespace std;  
int main()
{
    srand(time(0));
    int num=(rand()% 50) +1;
    int guess;
    do
    {
        cout<<"enter the guess no. between 1 to 50"<< endl;
        cin>> guess;
        if(guess>num)
          cout<<"guess lower"<<endl;
        else if(guess<num)
           cout<<"guess higher"<<endl;
        else
          cout<<"your guess is correct"<<endl;
    } while (guess!=num);
    
return 0;
}
