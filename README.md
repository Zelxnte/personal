//How it works:
//So, what happens is the user is prompted to enter a value.
//S/he enters is, and the statement check if it is between the range of 10k to 100k.

//If it is, it checks for the category which it fits in (from the previous code for the calculations).

//After it decides, it calculates the value accordingly.

//But at the same time, **IF** the user enters "-1", it still has to display this message:
//[Loan range: $10000 - $100000]
//Enter loan amount (-1 to quit): $1

****************************************************
code fragment 1:


#include <iostream>
#include <iomanip>

using namespace std;

int
main()
{
    double loanAmt = 0;
    double depositAmt = 0;
a
//Prompt for input
    cout << "\nEnter the loan amount: $";
    cin >> loanAmt;

//Calculations

    if (loanAmt >= 10000 && <= 24999)
        depositAmt = depositAmt + (loanAmt*(5/100));
    else if (loanamt >= 25000 && <= 39999)
        depositAmt = depositAmt + (loanAmt*(10/100));
    else if (loanamt >= 40000 && <= 55000)
        depositAmt = depositAmt + (loanAmt*(15/100));
   else
        cout << "\nInvalid loan amount!" << endl;

    cout << "The required deposit is: $" << depositAmt << endl;


return 0;
}


************************************************
code fragment 2:


 cout << "[Loan range: RM10000 - RM100000]\nEnter loan amount (-1 to quit): $";

    //Condition for accepting input from user. If it does not meet, loop the prompting
    while ((cin >> loanamt) && loanamt != -1)
        {
            if (loanamt < 10000 || loanamt > 100000)
                cout << "\nInvalid loan amount!\nPlease re-enter the loan amount: $";
            else
                cout << "\nEnter loan amount (-1 to quit): $";
        }
    //Message that displays when the user decides to terminate the program
    cout << "\n[Loan range: $10000 - $100000]\nEnter loan amount (-1 to quit): $" << loanamt << endl;
