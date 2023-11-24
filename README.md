# Guessing-Number-game
#Codsoft
#include<iostream>
#include<cstdlib>
using namespace std;
int main(){
int x=rand()%100 +1;
//cout<<"The random number is "<<x<<endl;

cout<<"my Guessed number "<<endl;
  int n;
int tries=0;
do{
  
cout<<"Enter the Guessed Number ";
cin>>n;
tries++;

    if(x<n){
     cout<<"Guessing is too high"<<endl;
     
    }
    else if(x>n){
        cout<<"Guessing is too low"<<endl;
        
    }
    else{
        cout<<"You guessed it right"<<endl;
        break;
    }



}while(x!=n);
cout<<"Number of tries "<<tries<<endl;

return 0;
}
