---
layout:     post
title:      "记录生活,记录你"
subtitle:   "分享生活中的美好"
date:       2018-05-25 16:43:00
author:     "Godlovezk"
header-img: "img/in-post/post-eleme-pwa/eleme-at-io.jpg"
header-mask: 0.3
catalog:    true
tags:
    - Life
    - The Beautiful
---

```javascript
public static int[] TwoSum(int[] nums ,int terget)
        {
            for (int i = 0; i < nums.Length ; i++)
            {
                for (int j = i+1; j <nums.Length; j++)
                {
                    if (nums [i]+nums[j]==terget)
                    {
                        int[] a = { i, j };
                        return a;
                    }
                }
              
               
            }
            return null;
        }
        
        public static  int[] TwoSums(int[] nums,int target)
        {
            List<int> list = new List<int>();
            int[] res = new int[2];
            for (int i = 0; i < nums.Length; i++)
            {
                if (list.Contains(target-nums[i]))
                {
                    res[0] = list.IndexOf(target - nums[i]);
                    res[1] = i;
                    break;
                }
                else
                {
                    list.Add(nums[i]);
                }
            }
            return res;
        } ]  

```