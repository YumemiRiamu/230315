# 230315

사용 코드

``` 
#include <iostream>

 using namespace std;

 
class CPnt 
 
{
  
 
int w, h;

 
public:
 
CPnt (int _w, int _h)
  {
    w = _w;
    h = _h;
  } 
 
CPnt ()
  {
    w = 0;
    h = 0;
  } 
 
 
void PrPt ()
  {
    cout << w + h << '\n';
  } 
 
 
 
CPnt operator+ (CPnt r)
  {
    
 
CPnt t;
    
 
t.w = w + r.w;
    
 
t.h = h + r.h;
    
 
return (t);
  
 
}

 
};


 
int
main () 
 
{
  
 
CPnt p1 (1, 1), p2 (2, 2), p3;
  
 
    //p3 = p1.operator+(p2);
    
p3 = p1 + p2;
  
 
p3.PrPt ();
  
 
 
return 0;

 
}
```

실행 결과 
![캡처](https://user-images.githubusercontent.com/93495684/225244543-e609a8e3-4a7a-4001-8cb4-a65a201e204d.PNG)


