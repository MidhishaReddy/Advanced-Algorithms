---
description: Easy
---

# Palindrome Number

**Idea**: We would in general think to convert a number to the string and them compare the reverse of a string. But its consumes space.

Considering digit reversing: We have an overflow issue. The number might be greater than Int-Max. To handle that, we reverse only half of the number and then compare. \
If we apply % operation on number we get last digit.\
If we apply / operation on number we get remaining digits.\
The main logic here is keep working on reverse\
int reverse = reverse \*10+(number%10);

The time complexity here is logn base 10, since we divide the number 10 here the complexity is logn base 10

```java
// Some code
class Solution {
    public boolean isPalindrome(int x) {
      
        int rev =0;
          
        //i should solve this recursively 
        //get the digits seperated by the divide and modulo function.
        //x =121
        //handle the negative numbers
        if(x<0 || x%10 ==0 && x!=0){
            return false;
        }
       while(x>rev){
           int rem = x%10;
             rev = (rev*10)+rem;
             x = x/10;
       }
        if(rev == x || x ==rev/10){
            return true;
        }


        return false;
    }
```
