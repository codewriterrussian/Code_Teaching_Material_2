# Python 複習題：`for`、`range()` 與串列（C Level）

難度說明：本份題目以 **C 等級**為主，重點是「追蹤迴圈流程、理解 `range()` 邊界、走訪串列、計數、加總、找最大值與最小值、除錯，以及搭配條件判斷完成小型應用」。

> 作答提醒：
>
> - 除非題目另外說明，請使用 `for` 迴圈。
> - 不使用 `while`。
> - 不使用 `append()`。
> - 找最大值、最小值或總和時，若題目有限制，請不要使用 `max()`、`min()` 或 `sum()`。
> - 先自己作答，再查看最後的參考答案。

---

## Part A：基本概念

### 1. `for` 迴圈主要用來做什麼？

請用自己的話說明：

```text

```

---

### 2. `range(5)` 會依序產生哪些整數？

答案：

```text

```

---

### 3. 為什麼 `range(1, 6)` 不會產生 `6`？

答案：

```text

```

---

### 4. 請補上程式，讓它印出三次 `Python`

```python
for i in __________:
    print("Python")
```

---

### 5. 在下面的迴圈中，變數 `fruit` 每次代表什麼？

```python
fruits = ["apple", "banana", "orange"]

for fruit in fruits:
    print(fruit)
```

答案：

```text

```

---

## Part B：流程追蹤與輸出判斷

### 6. 請寫出下面程式的完整輸出

```python
for i in range(4):
    print(i)

print("finish")
```

答案：

```text

```

---

### 7. 請寫出下面程式的完整輸出

```python
for i in range(2, 7):
    print(i)
```

答案：

```text

```

---

### 8. 請寫出下面程式的完整輸出

```python
for i in range(1, 10, 3):
    print(i)
```

答案：

```text

```

---

### 9. 請寫出下面程式的完整輸出

```python
for i in range(5, 0, -1):
    print(i)

print("go")
```

答案：

```text

```

---

### 10. 請寫出下面程式的完整輸出

```python
animals = ["cat", "dog", "bird"]

for animal in animals:
    print("I see", animal)
```

答案：

```text

```

---

### 11. 請寫出下面程式的完整輸出

```python
numbers = [2, 5, 8, 11]

for number in numbers:
    if number % 2 == 0:
        print(number)
```

答案：

```text

```

---

### 12. 請寫出下面程式的完整輸出，並注意迴圈外的 `print()`

```python
for i in range(3):
    print("inside")

print("outside")
```

答案：

```text

```

---

## Part C：理解與使用 `range()`

### 13. 請寫出可以產生 `3, 4, 5, 6, 7` 的 `range()`

```python
range(________________)
```

---

### 14. 請寫出可以產生 `2, 4, 6, 8, 10` 的 `range()`

```python
range(________________)
```

---

### 15. 請寫出可以產生 `9, 7, 5, 3, 1` 的 `range()`

```python
range(________________)
```

---

### 16. 請完成程式，印出 `1` 到 `n`，包含 `n`

```python
n = int(input())

for i in range(________________):
    print(i)
```

---

### 17. 請完成程式，印出 `0` 到 `n` 之間的偶數，包含可能的 `n`

```python
n = int(input())

for i in range(________________):
    print(i)
```

---

### 18. 下面程式為什麼沒有任何輸出？

```python
for i in range(1, 5, -1):
    print(i)
```

說明：

```text

```

請寫出修改後、可以印出 `5, 4, 3, 2, 1` 的程式：

```python

```

---

## Part D：走訪串列與條件判斷

### 19. 請寫一個迴圈，依序印出串列中的每個名字

```python
names = ["Amy", "Ben", "Cindy"]

# 請接著完成

```

---

### 20. 給定以下串列，只印出正數

```python
numbers = [-4, 7, 0, -2, 9, 3]
```

預期輸出：

```text
7
9
3
```

請寫程式：

```python

```

---

### 21. 給定以下串列，只印出大於或等於 60 的分數

```python
scores = [45, 60, 72, 58, 90]
```

請寫程式：

```python

```

---

### 22. 給定天氣串列，遇到 `晴天` 印出 `戶外活動`，遇到 `雨天` 印出 `室內活動`

```python
weather = ["晴天", "雨天", "雨天", "晴天"]
```

請寫程式：

```python

```

---

### 23. 請寫出下面程式的完整輸出

```python
temps = [20, 24, 18]

for t in temps:
    t = t + 2
    print(t)

print(temps)
```

答案：

```text

```

請說明：為什麼最後的 `temps` 沒有改變？

```text

```

---

### 24. 給定以下串列，印出所有偶數；如果某個數字不是偶數，不要輸出任何內容

```python
values = [13, 18, 22, 35, 40]
```

請寫程式：

```python

```

---

## Part E：計數、加總、最大值與最小值

### 25. 請寫出下面程式的完整輸出

```python
numbers = [3, 6, 9, 12]
count = 0

for number in numbers:
    if number % 2 == 0:
        count = count + 1

print(count)
```

答案：

```text

```

---

### 26. 給定以下串列，計算正數有幾個

```python
numbers = [-3, 5, 0, 7, -1, 8]
```

限制：不使用 `len()` 判斷答案。

請寫程式：

```python

```

---

### 27. 給定以下串列，計算所有數字的總和

```python
numbers = [4, 7, 2, 9]
```

限制：不使用 `sum()`。

請寫程式：

```python

```

---

### 28. 輸入整數 `n`，計算 `1` 到 `n` 的總和

例如輸入 `5`，輸出 `15`。

限制：不使用 `sum()`。

請寫程式：

```python

```

---

### 29. 輸入整數 `n`，分別計算 `1` 到 `n` 的奇數和與偶數和

輸出格式：

```text
odd: 奇數和
even: 偶數和
```

請寫程式：

```python

```

---

### 30. 給定以下串列，找出最大值

```python
numbers = [14, 3, 27, 9, 21]
```

限制：不使用 `max()`。

請寫程式：

```python

```

---

### 31. 給定以下串列，找出最小值

```python
numbers = [12, -4, 7, 0, -9, 5]
```

限制：不使用 `min()`。

請寫程式：

```python

```

---

## Part F：除錯題

### 32. 下面程式想印出 `0, 1, 2, 3`，但少印了一個數字。請修正

錯誤程式：

```python
for i in range(3):
    print(i)
```

修正後：

```python

```

---

### 33. 下面程式有語法錯誤。請指出原因並修正

錯誤程式：

```python
for i in range(5)
    print(i)
```

錯誤原因：

```text

```

修正後：

```python

```

---

### 34. 下面程式想印出所有偶數，但縮排錯誤。請修正

錯誤程式：

```python
numbers = [1, 2, 3, 4]

for number in numbers:
if number % 2 == 0:
print(number)
```

修正後：

```python

```

---

### 35. 下面程式想計算偶數數量，但答案永遠不正確。請修正

錯誤程式：

```python
numbers = [2, 5, 8, 11, 14]

for number in numbers:
    count = 0
    if number % 2 == 0:
        count = count + 1

print(count)
```

問題說明：

```text

```

修正後：

```python

```

---

### 36. 下面程式想找最大值，但初始值的設定方式可能產生錯誤。請修正

錯誤程式：

```python
numbers = [-8, -3, -12, -5]
largest = 0

for number in numbers:
    if number > largest:
        largest = number

print(largest)
```

問題說明：

```text

```

修正後：

```python

```

---

## Part G：小型應用題

### 37. 星星階梯

輸入整數 `n`，印出 `n` 層星星。

範例輸入：

```text
4
```

範例輸出：

```text
*
**
***
****
```

請寫程式：

```python

```

---

### 38. 統計晴天

給定天氣串列，計算 `晴天` 有幾天。

```python
weather = ["晴天", "陰天", "晴天", "雨天", "晴天", "陰天"]
```

預期輸出：

```text
3
```

請寫程式：

```python

```

---

### 39. 合格人數與最高分

給定分數串列：

```python
scores = [56, 81, 73, 92, 48, 65]
```

請同時完成：

1. 計算大於或等於 60 分的人數。
2. 找出最高分。

限制：不使用 `max()`。

輸出格式：

```text
pass count: 合格人數
highest: 最高分
```

請寫程式：

```python

```

---

### 40. 數字分類統計

輸入整數 `n`，檢查 `1` 到 `n` 的所有整數，分別統計：

- 偶數有幾個
- 奇數有幾個
- 3 的倍數有幾個

輸出格式：

```text
even: 偶數數量
odd: 奇數數量
multiple of 3: 3 的倍數數量
```

請寫程式：

```python

```

---

### 41. 簡易計算機

輸入兩個整數 `a b` 和一個運算符號 `op`。

規則：

- `+`：輸出加法結果
- `-`：輸出減法結果
- `*`：輸出乘法結果
- `/`：輸出除法結果
- 其他符號：輸出 `Invalid operator`

範例輸入：

```text
7 4 *
```

範例輸出：

```text
28
```

請寫程式：

```python

```

---

### 42. 字串重複與換行

請只使用一個 `print()`，印出以下結果：

```text
go
go
go
go
```

提示：可以使用 `"\n"` 和字串重複。

請寫程式：

```python

```


---
