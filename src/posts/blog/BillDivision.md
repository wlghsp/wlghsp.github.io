---
title: "해커랭크 Bill Division"
category: "Algorithm"
date: "2022-02-06 22:00:00 +09:00"
desc: "해커랭크 Bill Division 문제"

---

- https://www.hackerrank.com/challenges/bon-appetit/problem

## Solution


```python
def bonAppetit(bill, k, b):
    del bill[k]
    sumofBill = 0
    for i in bill:
        sumofBill += i
    change = b - sumofBill / 2
    result = "Bon Appetit" if change == 0 else int(change)
    print(result)


bill = [3, 10, 2, 9]  # 메뉴
k = 1  # 먹지 않은 메뉴
b = 12  # 낸 금액
bonAppetit(bill, k, b)


```