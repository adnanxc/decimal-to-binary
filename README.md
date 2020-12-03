# decimal-to-binary


#include <iostream>
using namespace std;
int main(){

    int a[32];
    int x , n;
    int i = 0;
    cout << "Enter a decimal number: ";
    cin >> x;
    n = x;

    while(n > 0){

        a[i] = n % 2;
        n = n / 2;
        i++;
    }

    cout << "Decimal: " << x << " & Binary: ";

    for(int j=i-1; j>=0 ; j--){
        cout << a[j];
    }


    return 0;
}
