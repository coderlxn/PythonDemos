#### 根据一个分数找到对应的成绩
```python
import bisect

def grade(socre, breakpoints=[60, 70, 80, 90], grades="FDCBA"):
	i = bisect.bisect(breakpoints, socre)
	return grades[i]
[grade(score) for score in [33, 99, 77, 70, 89, 90, 100]]
# ['F', 'A', 'C', 'C', 'B', 'A', 'A']
```