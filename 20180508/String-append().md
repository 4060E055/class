
### 字串的附加
```
#include <iostream>
using namespace std;

int main()
{
  string s1("Welcome");
  s1.append(" to CPP"); 
  cout << s1 << endl; 
}
```
```
string s1("Welcome");
s1.append(" to CPP"); 
cout << s1 << endl; 
```
```
string s2("Welcome");
s2.append(" to C and Cpp", 3, 6); 
cout << s2 << endl;
```
```
string s3("Welcome");
s3.append(" to C and Cpp", 7); 
cout << s3 << endl; 
```
```
string s4("Welcome"); 
s4.append(14, 'F'); 
cout << s4 << endl; 
```


```
#include <iostream>
#include <string>

int main ()
{
  std::string str;
  std::string str2="Writing ";
  std::string str3="print 10 and then 5 more";

  // used in the same order as described above:
  str.append(str2);                       // "Writing "
  str.append(str3,6,3);                   // "10 "
  str.append("dots are cool",5);          // "dots "
  str.append("here: ");                   // "here: "
  str.append(10u,'.');                    // ".........."
  str.append(str3.begin()+8,str3.end());  // " and then 5 more"
  str.append<int>(5,0x2E);                // "....."

  std::cout << str << '\n';
  return 0;
}
```
### 從螢幕讀取字串
```
#include<iostream>
using namespace std;

int main()
{
	string number,name; 
	cout<<"請輸入學號：";
	cin>>number; 
	cout<<"請輸入姓名：";
	cin>>name; 
	cout<<"你的學號 姓名為："<<number<<" "<<name<<endl; 
 } 
 
```
[作業2]從螢幕輸入姓名學號要顯示姓名學號
![執行畫面](0508.png)


```
string city;
cout << "Enter a city: ";
getline(cin, city, '\n'); // Same as getline(cin, city)
cout << "You entered " << city << endl;
```



```

```


```

```
