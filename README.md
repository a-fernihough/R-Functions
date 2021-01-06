# R-Functions
Useful operations I always forget how to do

***
Make within group index (like birth order). Use `arrange` to sort by age or year prior to creation if needed.

```
df %>% 
  group_by(group) %>% 
  mutate(groupid = row_number(group))  
```
