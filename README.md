# NeetCode

## Arrays & Hashing
![image](https://github.com/user-attachments/assets/5262d534-7f93-4e09-82bb-6072bc13170b)

### Perequisites
1. Dynamic Arrays
2. Hash Usage
3. Hash Implementation
4. Prefix Sums

### 1- [Contains Duplicate](https://neetcode.io/problems/duplicate-integer?list=neetcode150)


Given an integer array nums, return true if any value appears more than once in the array, otherwise return false.


Example 1:

```
Input: nums = [1, 2, 3, 3] 
Output: true

Example 2:

Input: nums = [1, 2, 3, 4]

Output: false 
```
### First Submissions
```
class Solution {
    public boolean hasDuplicate(int[] nums) {
            //Outer loop 
            for (int i = 0; i< nums.length; i++)
                {
            //Inner loop
                    for (int j=i+1; j <nums.length; j++)
                     {
                        //Check if there are duplicates , if esy return true
                        if (nums[i] ==nums[j]) 
                        {
                            return true;
                        }
                     }
                }
            return false;     
        
    }
}
```
