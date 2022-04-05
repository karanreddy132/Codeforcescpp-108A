# Codeforcescpp-108A
#include <bits/stdc++.h>
using namespace std;
 
int main() {
	string s;
	cin >> s;
	stringstream geek(s.substr(0, 2));
	stringstream geek1(s.substr(3, 2));
	int x(0), y(0);
	geek >> x;
	geek1 >> y;
	do{
    y++;
    if(y==60){
      x++;
      y=0;
    }
    if(x==24){
      x=0;
    }
  }while((x%10)*10+x/10!=y);
  cout << x/10 << x%10 << ":" << y/10 << y%10;
	return 0;
}
