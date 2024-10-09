---
title: Neetcode Duplicate Integer
date: 2024-10-09 23:06:32
tags:
  - Neetcode
  - Coding
categories:
  - Programming
---
## Problem
Given an integer array nums, return true if any value appears more than once in the array, otherwise return false.

#### Example 1
```plain text
Input: nums = [1, 2, 3, 3]

Output: true
```

#### Example 2
```plain text
Input: nums = [1, 2, 3, 4]

Output: false
```

## Note & Code

{% note default  %}
LeetCode會自動生成測試案例和測試框架，因此只要寫處理問題的class就好。（NeetCode同理）
{% endnote %}

#### Solution

```cpp
class Solution{
	public:
		bool containsDuplicate(vector<int>& nums){
			unordered_set<int> hushset;
		
			for(int i=0 ; i<nums.size() ; i++){
				if(hushset.count(nums[i])){
					return true;
			}
			
			hushset.insert(num[i]);
	}
	return false;
};
```
