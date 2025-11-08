
<img width="5400" height="2383" alt="Code Karaoke-min" src="https://github.com/user-attachments/assets/b93e02e6-6468-4a00-9a9e-a00bc0e4cb0f" />



# level-2-code-karaoke
Level 2 questions for code karaoke event, there are 2 questions write the program and test it with examples in those questions and upload in fork 
# Question 1:
1.Tow Sum:
Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.
You may assume that each input would have exactly one solution, and you may not use the same element twice.
You can return the answer in any order.
 
# Example 1:
Input: nums = [2,7,11,15], target = 9
Output: [0,1]
Explanation: Because nums[0] + nums[1] == 9, we return [0, 1].

# Example 2:
Input: nums = [3,2,4], target = 6
Output: [1,2]

# Example 3:
Input: nums = [3,3], target = 6
Output: [0,1]

# CODE:
nums = [2, 7, 11, 15]
target = 9

for i in range(len(nums)):
    for j in range(i + 1, len(nums)):
        if nums[i] + nums[j] == target:
            print("Indices:", [i, j])
            print("Numbers:", nums[i], "and", nums[j])
            break

# OUTPUT:
<img width="1248" height="577" alt="Screenshot 2025-11-08 105557" src="https://github.com/user-attachments/assets/08a77ae8-79c2-40f5-bdfb-6a38d0b43b4e" />



# Question 2:
1. Palindrome Number:

Given an integer x, return true if x is a palindrome, and false otherwise.
 
# Example 1:
Input: x = 121
Output: true
Explanation: 121 reads as 121 from left to right and from right to left.
# Example 2:
Input: x = -121
Output: false
Explanation: From left to right, it reads -121. From right to left, it becomes 121-. Therefore it is not a palindrome.
# Example 3:
Input: x = 10
Output: false
Explanation: Reads 01 from right to left. Therefore it is not a palindrome.


# CODE:
x=121
og=x
sum=0
while x>0:
    rem=x%10
    sum=sum*10+rem
    x=x//10
og=x
if og ==sum:
    print("true")
else:
    print("false")

# OUTPUT:
<img width="1350" height="404" alt="Screenshot 2025-11-08 104847" src="https://github.com/user-attachments/assets/2456db34-4d7a-4685-8526-54ef5f8011f0" />
