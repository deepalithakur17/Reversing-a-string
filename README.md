# Reversing-a-string
reversing a string by recursion

#include<bits/stdc++.h>
using namespace std;

void solve(string& str,int i,int j)
{
    if(i>j)
    {
        return ;
    }
    swap(str[i],str[j]);
    i++;
    j--;
    solve(str,i,j);
}

int main()
{

    string str;
    cout<<"enter a string: ";
    cin>>str;
    solve(str,0,str.length()-1);
    cout<<str;
}
