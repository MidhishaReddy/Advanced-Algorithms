# Page 1

```java
// Some code
Public int KaratsubaAlgo(int x, int y){
//base case: if it’s a single digit return the product directly:
If(x<10 && y<10) return X*Y;
else 
//recursive call:
{
//get the length of both x and y and find the maximum length's of those two:
int n = Math.max(x.len,y.len);
int half = n/2;
//the algorithm's multiplication is divided into:
a = x/10*half;//left part of the number x
b = x%10*half;//right part of the number x
c = y/10*half;//left part of the number y
d = y%10*half;//right part of the number y
//first product: call the function now with a, c
ac = KaratsubaAlgo(a,c);
//second product: call the function with b and d
bd = karatsubaAlgo(b,d);
//third part:
sum_ad_bc = karatsuba(a+b,c+d)-ac-bd;

//return the result:
return ac *(10*(2*half))+(sum_ad_bc*10*)+bd;
}
```
