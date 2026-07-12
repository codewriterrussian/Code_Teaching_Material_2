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

# 參考答案

> 建議完成所有題目後再查看。

## Part A

### 1.

```text
for 迴圈可以讓一段程式重複執行，也可以依序取出串列中的每個元素。
```

### 2.

```text
0, 1, 2, 3, 4
```

### 3.

```text
因為 range() 的 stop 不包含在產生的數字中，所以會在 6 之前停止。
```

### 4.

```python
for i in range(3):
    print("Python")
```

### 5.

```text
fruit 每次代表 fruits 串列中目前被取出的元素，依序是 apple、banana 和 orange。
```

---

## Part B

### 6.

```text
0
1
2
3
finish
```

### 7.

```text
2
3
4
5
6
```

### 8.

```text
1
4
7
```

### 9.

```text
5
4
3
2
1
go
```

### 10.

```text
I see cat
I see dog
I see bird
```

### 11.

```text
2
8
```

### 12.

```text
inside
inside
inside
outside
```

---

## Part C

### 13.

```python
range(3, 8)
```

### 14.

```python
range(2, 11, 2)
```

### 15.

```python
range(9, 0, -2)
```

### 16.

```python
n = int(input())

for i in range(1, n + 1):
    print(i)
```

### 17.

```python
n = int(input())

for i in range(0, n + 1, 2):
    print(i)
```

### 18.

說明：

```text
開始值是 1，結束方向需要往較大的數字前進，但 step 是 -1，方向相反，因此 range() 不會產生任何數字。
```

修正後：

```python
for i in range(5, 0, -1):
    print(i)
```

---

## Part D

### 19.

```python
names = ["Amy", "Ben", "Cindy"]

for name in names:
    print(name)
```

### 20.

```python
numbers = [-4, 7, 0, -2, 9, 3]

for number in numbers:
    if number > 0:
        print(number)
```

### 21.

```python
scores = [45, 60, 72, 58, 90]

for score in scores:
    if score >= 60:
        print(score)
```

### 22.

```python
weather = ["晴天", "雨天", "雨天", "晴天"]

for day in weather:
    if day == "晴天":
        print("戶外活動")
    elif day == "雨天":
        print("室內活動")
```

### 23.

```text
22
26
20
[20, 24, 18]
```

說明：

```text
t 只是每次迴圈暫時取得的值。修改 t 不會直接修改原本串列中的元素。
```

### 24.

```python
values = [13, 18, 22, 35, 40]

for value in values:
    if value % 2 == 0:
        print(value)
```

---

## Part E

### 25.

```text
2
```

### 26.

```python
numbers = [-3, 5, 0, 7, -1, 8]
count = 0

for number in numbers:
    if number > 0:
        count = count + 1

print(count)
```

### 27.

```python
numbers = [4, 7, 2, 9]
total = 0

for number in numbers:
    total = total + number

print(total)
```

### 28.

```python
n = int(input())
total = 0

for i in range(1, n + 1):
    total = total + i

print(total)
```

### 29.

```python
n = int(input())
odd_total = 0
even_total = 0

for i in range(1, n + 1):
    if i % 2 == 0:
        even_total = even_total + i
    else:
        odd_total = odd_total + i

print("odd:", odd_total)
print("even:", even_total)
```

### 30.

```python
numbers = [14, 3, 27, 9, 21]
largest = numbers[0]

for number in numbers:
    if number > largest:
        largest = number

print(largest)
```

### 31.

```python
numbers = [12, -4, 7, 0, -9, 5]
smallest = numbers[0]

for number in numbers:
    if number < smallest:
        smallest = number

print(smallest)
```

---

## Part F

### 32.

```python
for i in range(4):
    print(i)
```

### 33.

錯誤原因：

```text
for 迴圈那一行的最後少了冒號。
```

修正後：

```python
for i in range(5):
    print(i)
```

### 34.

```python
numbers = [1, 2, 3, 4]

for number in numbers:
    if number % 2 == 0:
        print(number)
```

### 35.

問題說明：

```text
count 被放在迴圈內，每次處理新的數字時都會重新變成 0，因此無法累積數量。
```

修正後：

```python
numbers = [2, 5, 8, 11, 14]
count = 0

for number in numbers:
    if number % 2 == 0:
        count = count + 1

print(count)
```

### 36.

問題說明：

```text
所有數字都是負數，但 largest 從 0 開始，因此沒有任何數字能更新 largest，最後會錯誤地輸出 0。
```

修正後：

```python
numbers = [-8, -3, -12, -5]
largest = numbers[0]

for number in numbers:
    if number > largest:
        largest = number

print(largest)
```

---

## Part G

### 37.

```python
n = int(input())

for i in range(1, n + 1):
    print("*" * i)
```

### 38.

```python
weather = ["晴天", "陰天", "晴天", "雨天", "晴天", "陰天"]
sunny_count = 0

for day in weather:
    if day == "晴天":
        sunny_count = sunny_count + 1

print(sunny_count)
```

### 39.

```python
scores = [56, 81, 73, 92, 48, 65]
pass_count = 0
highest = scores[0]

for score in scores:
    if score >= 60:
        pass_count = pass_count + 1

    if score > highest:
        highest = score

print("pass count:", pass_count)
print("highest:", highest)
```

### 40.

```python
n = int(input())
even_count = 0
odd_count = 0
multiple_of_three_count = 0

for i in range(1, n + 1):
    if i % 2 == 0:
        even_count = even_count + 1
    else:
        odd_count = odd_count + 1

    if i % 3 == 0:
        multiple_of_three_count = multiple_of_three_count + 1

print("even:", even_count)
print("odd:", odd_count)
print("multiple of 3:", multiple_of_three_count)
```


### 41.

```python
a, b, op = input().split()
a = int(a)
b = int(b)

if op == "+":
    print(a + b)
elif op == "-":
    print(a - b)
elif op == "*":
    print(a * b)
elif op == "/":
    print(a / b)
else:
    print("Invalid operator")
```

### 42.

```python
print("go\n" * 3 + "go")
```

