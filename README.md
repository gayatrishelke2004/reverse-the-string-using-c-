#include <iostream>
#include <string.h>
using namespace std;

string revstr(string &s) {
    int i, len, temp;
    len = s.length();
    if(len%2 != 0)
    {
        for(i = 0;i <= len/2;i++)
        {
            temp = s[i];
            s[i] = s[len - i - 1];
            s[len - i - 1] = temp;
        }
        return s;
    }
    if(len%2 == 0)
    {
        for(i = 0;i < len/2;i++)
        {
            temp = s[i];
            s[i] = s[len - i - 1];)
{
            s[len - i - 1] = temp;
        }
        return s;
    }
}
int main(
    string str;   

    cout << "enter string : " ;
    getline(cin,str);
   


cout << "Before reversing the string: " << str;
    
    cout<< "\nAfter reversing the string: " << revstr(str);
return 0;
}
