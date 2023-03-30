# Two sum

Input - array of integers and the target sum we are searching for&#x20;

output - two indices where we find the integers

Idea: Use a hashMap\
get the second number , as we have the first number and the sum of two numbers \
diff = target -nums\[i]

```java
// Some code
public int[] twoSum(int[] nums, int target){
int[] result = new int[2];
int diff=0;
HashMap<Integer, Integer> map = new HashMap<>();

for(int i =0; i<nums.length; i++){
    
    diff = target-nums[i];
    if(map.ContainsKey(diff)){
        result[0] = i;
        result[1] = map.get(diff);
    }
    else 
        map.add(nums[i],i);
    }
return result;
}
```
