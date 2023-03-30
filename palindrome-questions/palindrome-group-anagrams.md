# Palindrome- Group anagrams

**Idea:**&#x20;

1. Loop through the stings in the set of strings .
2. Sort the string&#x20;
3. check if is there in the hashmap&#x20;
4. Iterate throught the hashmap and the put the value into the result array.
5. Return the result array

```java
// Some code
Permutations:
class Solution {
    public List<List<String>> groupAnagrams(String[] strs) {
        
        //the result to be retured is list of list so lets create a outpu that way
     
        //Create a hashmap to store this string with the corresponding combination values
        HashMap<String, List<String>> map = new HashMap<>();

        //get each string from the list of input strings:
        for(String s : strs){
            //convert to a characters array for it to be sorted:
            char[] c = s.toCharArray();
            //sort the character array:
            Arrays.sort(c);

            //Store this sorted array to a new variable called
            String sorted =  String.valueOf(c);

            //Check if the this sorted string is in the hashmap
            if(!map.containsKey(sorted))
                //add to the hashmap
                  map.put(sorted, new ArrayList<>());
                map.get(sorted).add(s);
        }
        return new ArrayList<>(map.values());
    }
}
```
