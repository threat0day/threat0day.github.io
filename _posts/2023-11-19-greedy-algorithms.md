# Пример реализации жадного алгоритма
Суть - наиболее оптимально принять решение на каждом шаге

```python
money_variants = {
    100: 0,
    20: 0,
    15: 0,
    10: 0,
    5: 0,
    3: 0,
    1: 0
}
 
points = 109412
 
for money in money_variants.keys():
    while money <= points > 0:
        points -= money
        money_variants[money] += 1
 
print(money_variants)
```
Теги: [алгоритмы]
