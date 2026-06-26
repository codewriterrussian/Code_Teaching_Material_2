# Python Lesson 4–5 綜合複習題：bool、型別轉換、商數餘數、時間換算、比較與邏輯運算

---

## Part A：觀察 `bool()` 與資料型態

### 1. 請寫出下面程式的輸出結果

```python
print(bool("0"))
print(bool(""))
print(bool(0))
print(bool(8))
```

答案：

```text

```

---

### 2. 請寫出下面程式的輸出結果

```python
word = "False"
empty_word = ""
print(bool(word))
print(bool(empty_word))
```

答案：

```text

```

---

### 3. 請寫出下面程式的輸出結果，並簡單說明原因

```python
items = []
items2 = [0]
print(bool(items))
print(bool(items2))
```

答案：

```text

```

---

### 4. 請判斷下面程式是否可以執行，並說明原因

```python
x = input()
print(x + 5)
```

請回答：

```text

```

---

### 5. 請寫出下面程式在輸入 `7` 時的輸出結果

```python
x = input()
print(x * 3)
```

答案：

```text

```

---

## Part B：`int()`、字串與數字運算

### 6. 請寫出下面程式在輸入 `7` 時的輸出結果

```python
x = int(input())
print(x * 3)
```

答案：

```text

```

---

### 7. 請寫出下面程式的輸出結果

```python
a = "4"
b = 5
print(a * b)
print(int(a) * b)
```

答案：

```text

```

---

### 8. 請修正下面程式，讓它可以輸出兩個數字的總和

錯誤程式：

```python
a, b = input().split()
print(a + b)
```

修正後：

```python

```

---

### 9. 請寫一個程式，讓使用者輸入一個整數，輸出它加上 20 的結果

範例輸入：

```text
15
```

範例輸出：

```text
35
```

請寫程式：

```python

```

---

### 10. 請用一句話說明：為什麼 `input()` 後面常常需要加 `int()`？

請回答：

```text

```

---

## Part C：商數 `//` 與餘數 `%`

### 11. 請寫出下面程式的輸出結果

```python
print(29 // 6)
print(29 % 6)
```

答案：

```text

```

---

### 12. 有 95 顆糖果，每袋裝 8 顆。請寫程式輸出可以裝滿幾袋、剩下幾顆

請寫程式：

```python

```

---

### 13. 使用者輸入兩個整數 `total size`，代表總數量與每盒數量。請輸出完整盒數和剩下數量

範例輸入：

```text
53 10
```

範例輸出：

```text
5
3
```

請寫程式：

```python

```

---

### 14. 請寫出下面程式的輸出結果

```python
n = 17
k = 5
print(n // k)
print(n % k)
print((n // k) * k + n % k)
```

答案：

```text

```

---

### 15. 請寫一個程式：輸入一個整數 `x`，輸出 `x` 的平方除以 10 的商數與餘數

範例輸入：

```text
9
```

範例輸出：

```text
8
1
```

請寫程式：

```python

```

---

## Part D：時間與單位換算

### 16. 請寫出下面程式在輸入 `3672` 時的輸出結果

```python
s = int(input())
h = s // 3600
m = s // 60 % 60
sec = s % 60
print(h, m, sec)
```

答案：

```text

```

---

### 17. 請寫一個程式：輸入總分鐘數，轉換成 `小時 分鐘`

範例輸入：

```text
185
```

範例輸出：

```text
3 5
```

請寫程式：

```python

```

---

### 18. 請寫一個程式：輸入總天數，轉換成 `週 天`

範例輸入：

```text
23
```

範例輸出：

```text
3 2
```

請寫程式：

```python

```

---

### 19. 一部影片長度用秒數表示。請輸出它有幾分鐘又幾秒，格式為 `M min S sec`

範例輸入：

```text
125
```

範例輸出：

```text
2 min 5 sec
```

請寫程式：

```python

```

---

### 20. 請寫一個程式：輸入總小時數，轉換成 `天 小時`

範例輸入：

```text
80
```

範例輸出：

```text
3 8
```

請寫程式：

```python

```

---

## Part E：比較運算與 `=`、`==`、`!=`

### 21. 請寫出下面程式的輸出結果

```python
a = 12
b = "12"
print(a == b)
print(str(a) == b)
print(a != int(b))
```

答案：

```text

```

---

### 22. 請判斷下面兩行的意思有什麼不同

```python
score = 80
score == 80
```

請回答：

```text

```

---

### 23. 請寫一個程式：輸入分數，如果分數大於等於 60，輸出 `True`

請寫程式：

```python

```

---

### 24. 請寫一個程式：輸入一個整數，判斷它是否不等於 0

範例輸入：

```text
5
```

範例輸出：

```text
True
```

請寫程式：

```python

```

---

### 25. 請修正下面錯誤程式，讓它可以判斷輸入數字是否大於 100

錯誤程式：

```python
x = input()
print(x > 100)
```

修正後：

```python

```

---

## Part F：邏輯運算 `and`、`or` 與括號

### 26. 請寫出下面程式的輸出結果

```python
print(True and False)
print(True or False)
print(False or False)
```

答案：

```text

```

---

### 27. 請寫出下面程式的輸出結果，注意 `and` 和 `or` 的順序

```python
print(False or True and False)
print((False or True) and False)
print(True and False or True)
```

答案：

```text

```

---

### 28. 請寫一個程式：輸入年齡和身高，年齡大於等於 12 且身高大於 140，才輸出 `True`

範例輸入：

```text
13 150
```

範例輸出：

```text
True
```

請寫程式：

```python

```

---

### 29. 請寫一個程式：輸入年齡，如果年齡小於 6 或大於等於 65，輸出 `True`

請寫程式：

```python

```

---

### 30. 登入檢查：正確帳號是 `cat`，正確密碼是 `meow123`。請讓使用者同一行輸入帳號和密碼，兩個都正確才輸出 `True`

請寫程式：

```python

```

---

## Part G：字串重複、字串相加與串列相加

### 31. 請寫出下面程式的輸出結果

```python
word = "go"
print(word * 4)
print(word + "!")
```

答案：

```text

```

---

### 32. 請判斷下面程式是否可以完整執行，並說明原因

```python
print("A" + 3)
print("A" * 3)
```

請回答：

```text

```

---

### 33. 請寫出下面程式的輸出結果

```python
a = [1, 2]
b = ["x", "y"]
print(a + b)
print(b + a)
```

答案：

```text

```

---

### 34. 請寫一個程式：輸入一個符號和一個整數，輸出該符號重複後的結果

範例輸入：

```text
# 5
```

範例輸出：

```text
#####
```

請寫程式：

```python

```

---

### 35. 請用字串重複輸出下面圖形，不要一個一個手打星號

目標輸出：

```text
****
********
************
```

請寫程式：

```python

```

---

## Part H：綜合應用題

### 36. 自動售票機：一張票 45 元。輸入投入金額，輸出可以買幾張票、剩下多少元

範例輸入：

```text
200
```

範例輸出：

```text
4
20
```

請寫程式：

```python

```

---

### 37. 課堂分組：輸入學生人數和每組人數，輸出是否剛好分完

提示：如果餘數是 0，代表剛好分完。

請寫程式：

```python

```

---

### 38. 請修正下面錯誤程式，讓它可以正確判斷輸入數字是否在 1 到 50 之間，包含 1 和 50

錯誤程式：

```python
x = input()
print(x >= 1 and x <= 50)
```

修正後：

```python

```

---

### 39. 請寫一個程式：輸入一個單字和一個整數 `n`。如果 `n > 0` 且單字不是空字串，輸出 `True`

請寫程式：

```python

```

---

### 40. 小挑戰：輸入總秒數，先輸出它是否剛好是整分鐘，再輸出它換算後的 `分鐘 秒`

範例輸入：

```text
125
```

範例輸出：

```text
False
2 5
```

請寫程式：

```python

```

---

# 參考答案

## Part A

### 1.

```text
True
False
False
True
```

### 2.

```text
True
False
```

### 3.

```text
False
True

items 是空串列，所以是 False。
items2 裡面有一個元素 0，所以是 True。
```

### 4.

```text
不可以正確執行。input() 讀進來的是字串，x + 5 會讓字串和整數相加，造成錯誤。應該先用 int() 轉成整數。
```

### 5.

```text
777
```

---

## Part B

### 6.

```text
21
```

### 7.

```text
44444
20
```

### 8.

```python
a, b = map(int, input().split())
print(a + b)
```

### 9.

```python
x = int(input())
print(x + 20)
```

### 10.

```text
因為 input() 讀進來的資料預設是字串，如果要做數學運算，需要先轉成整數。
```

---

## Part C

### 11.

```text
4
5
```

### 12.

```python
candies = 95
bag_size = 8
print(candies // bag_size)
print(candies % bag_size)
```

### 13.

```python
total, size = map(int, input().split())
print(total // size)
print(total % size)
```

### 14.

```text
3
2
17
```

### 15.

```python
x = int(input())
square = x ** 2
print(square // 10)
print(square % 10)
```

---

## Part D

### 16.

```text
1 1 12
```

### 17.

```python
total_minutes = int(input())
hours = total_minutes // 60
minutes = total_minutes % 60
print(hours, minutes)
```

### 18.

```python
total_days = int(input())
weeks = total_days // 7
days = total_days % 7
print(weeks, days)
```

### 19.

```python
total_seconds = int(input())
minutes = total_seconds // 60
seconds = total_seconds % 60
print(minutes, "min", seconds, "sec")
```

### 20.

```python
total_hours = int(input())
days = total_hours // 24
hours = total_hours % 24
print(days, hours)
```

---

## Part E

### 21.

```text
False
True
False
```

### 22.

```text
score = 80 是把 80 放進 score 這個變數。
score == 80 是判斷 score 是否等於 80，結果會是 True 或 False。
```

### 23.

```python
score = int(input())
print(score >= 60)
```

### 24.

```python
x = int(input())
print(x != 0)
```

### 25.

```python
x = int(input())
print(x > 100)
```

---

## Part F

### 26.

```text
False
True
False
```

### 27.

```text
False
False
True
```

### 28.

```python
age, height = map(int, input().split())
print(age >= 12 and height > 140)
```

### 29.

```python
age = int(input())
print(age < 6 or age >= 65)
```

### 30.

```python
account, password = input().split()
print(account == "cat" and password == "meow123")
```

---

## Part G

### 31.

```text
gogogogo
go!
```

### 32.

```text
不可以完整執行。第一行 "A" + 3 會錯，因為字串不能直接和整數用 + 相加。程式會停在第一行，所以第二行不會執行。
```

### 33.

```text
[1, 2, 'x', 'y']
['x', 'y', 1, 2]
```

### 34.

```python
symbol, count = input().split()
count = int(count)
print(symbol * count)
```

### 35.

```python
print("*" * 4)
print("*" * 8)
print("*" * 12)
```

---

## Part H

### 36.

```python
money = int(input())
price = 45
print(money // price)
print(money % price)
```

### 37.

```python
students, group_size = map(int, input().split())
print(students % group_size == 0)
```

### 38.

```python
x = int(input())
print(x >= 1 and x <= 50)
```

也可以寫成：

```python
x = int(input())
print(1 <= x <= 50)
```

### 39.

```python
word = input()
n = int(input())
print(n > 0 and bool(word))
```

### 40.

```python
total_seconds = int(input())
print(total_seconds % 60 == 0)
minutes = total_seconds // 60
seconds = total_seconds % 60
print(minutes, seconds)
```

---