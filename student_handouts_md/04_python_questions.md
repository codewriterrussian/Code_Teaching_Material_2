# Python 綜合複習題：運算子、複合運算子、型態比較與格式化輸出

---

## Part A：運算子進階追蹤 `+ - * / ** // %` 與優先順序

### 1. 請寫出下面程式的輸出結果，注意 `*`、`//`、`%` 會比 `+`、`-` 先計算

```python
print(2 + 3 * 4)
print((2 + 3) * 4)
print(17 - 5 * 2 + 8 // 3)
```

答案：

```text

```

---

### 2. 請寫出下面程式的輸出結果，注意 `**` 的優先順序

```python
print(2 ** 3 * 2)
print(2 * 3 ** 2)
print((2 + 3) ** 2)
```

答案：

```text

```

---

### 3. 請寫出下面程式的輸出結果，並觀察商數與餘數如何還原原本的數字

```python
n = 58
k = 7
q = n // k
r = n % k
print(q)
print(r)
print(q * k + r)
```

答案：

```text

```

---

### 4. 請寫出下面程式的輸出結果，注意 `/` 和 `//` 的差別

```python
print(20 / 4)
print(20 // 4)
print(21 / 4)
print(21 // 4)
```

答案：

```text

```

---

### 5. 請寫一個程式：輸入三個整數 `a b c`，輸出 `(a + b) * c`、`a + b * c`、`(a + b * c) % 10`

範例輸入：

```text
3 4 5
```

範例輸出：

```text
35
23
3
```

請寫程式：

```python

```

---

### 6. 請寫一個程式：輸入一個三位數整數，依序輸出百位、十位、個位

提示：可以使用 `//` 和 `%`。

範例輸入：

```text
728
```

範例輸出：

```text
7
2
8
```

請寫程式：

```python

```

---

## Part B：商數餘數的進階應用題

### 7. 使用者輸入兩個整數 `n k`，代表有 `n` 個物品，每箱最多放 `k` 個。請輸出至少需要幾個箱子

提示：如果不能剛好分完，還需要多一個箱子。

範例輸入：

```text
23 5
```

範例輸出：

```text
5
```

請寫程式：

```python

```

---

### 8. 請寫出下面程式的輸出結果，並注意每一步變數如何改變

```python
x = 35
x = x // 4
print(x)
x = x * 10 + 3
print(x)
x = x % 7
print(x)
```

答案：

```text

```

---

### 9. 請寫一個程式：輸入總秒數，輸出 `小時 分鐘 秒`

範例輸入：

```text
3672
```

範例輸出：

```text
1 1 12
```

請寫程式：

```python

```

---

### 10. 請寫一個程式：輸入一個整數 `x`，輸出 `x` 的平方的十位數

範例輸入：

```text
17
```

說明：`17 ** 2 = 289`，十位數是 `8`。

範例輸出：

```text
8
```

請寫程式：

```python

```

---

## Part C：比較運算子與 `=`、`==`

### 11. 請寫出下面程式的輸出結果

```python
x = 10
print(x == 10)
print(x != 10)
print(x >= 8)
print(x < 5)
```

答案：

```text

```

---

### 12. 請判斷下面兩行的意思有什麼不同

```python
score = 80
score == 80
```

請回答：

```text

```

---

### 13. 請寫一個程式：輸入分數，如果分數大於或等於 60，輸出 `True`

請寫程式：

```python

```

---

### 14. 請寫一個程式：輸入身高，如果身高大於或等於 120，輸出 `True`

請寫程式：

```python

```

---

### 15. 請修正下面錯誤程式，讓它可以判斷輸入數字是否大於 100

錯誤程式：

```python
x = input()
print(x > 100)
```

修正後：

```python

```

---

## Part D：邏輯運算子 `and`、`or` 與運算順序

### 16. 請寫出下面程式的輸出結果

```python
print(True and True)
print(True and False)
print(False or True)
print(False or False)
```

答案：

```text

```

---

### 17. 請寫出下面程式的輸出結果，注意 `and` 會比 `or` 先計算

```python
print(True or False and False)
print(False or True and False)
print((False or True) and False)
```

答案：

```text

```

---

### 18. 請寫一個程式：輸入身高和年齡，身高至少 120 且年齡至少 10，才輸出 `True`

範例輸入：

```text
130 11
```

範例輸出：

```text
True
```

請寫程式：

```python

```

---

### 19. 請寫一個程式：輸入消費金額和是否有會員卡。若消費金額大於等於 300，或會員卡輸入 `yes`，輸出 `True`

範例輸入：

```text
250 yes
```

範例輸出：

```text
True
```

請寫程式：

```python

```

---

### 20. 請寫一個程式：輸入分數，如果分數在 0 到 100 之間，包含 0 和 100，輸出 `True`

請寫程式：

```python

```

---

## Part E：字串與串列的 `+`、`*`

### 21. 請寫出下面程式的輸出結果

```python
s1 = "hello"
s2 = "hi"
print(s1 + s2)
print(s2 * 3)
```

答案：

```text

```

---

### 22. 請判斷下面程式是否可以完整執行，並說明原因

```python
print("hi" * 2)
print("hi" * "2")
```

請回答：

```text

```

---

### 23. 請寫出下面程式的輸出結果

```python
l1 = [123]
l2 = [456]
print(l1 + l2)
print(l1 * 3)
```

答案：

```text

```

---

### 24. 請寫一個程式：輸入一個名字，輸出 `hi 名字`

範例輸入：

```text
Tom
```

範例輸出：

```text
hi Tom
```

請寫程式：

```python

```

---

### 25. 請寫一個程式：輸入一個字串和一個整數，輸出重複後的字串

範例輸入：

```text
ha 4
```

範例輸出：

```text
hahahaha
```

請寫程式：

```python

```

---

## Part F：複合運算子 `+= -= *= /= //= %=`

### 26. 請寫出下面程式的輸出結果

```python
x = 5
x += 3
print(x)
```

答案：

```text

```

---

### 27. 請寫出下面程式的輸出結果

```python
money = 100
money -= 30
print(money)
```

答案：

```text

```

---

### 28. 請寫出下面程式的輸出結果

```python
score = 10
score *= 2
print(score)
```

答案：

```text

```

---

### 29. 請寫出下面程式的輸出結果

```python
number = 23
number %= 5
print(number)
```

答案：

```text

```

---

### 30. 請用一句話說明：`x += 1` 和 `x = x + 1` 的關係

請回答：

```text

```

---

### 31. 請判斷 `>=` 是不是複合運算子，並說明原因

請回答：

```text

```

---

## Part G：不同資料型態的比較

### 32. 請寫出下面程式的輸出結果

```python
print(10 == "10")
print(10 == 10)
print("hello" != "Hello")
```

答案：

```text

```

---

### 33. 請判斷下面程式是否可以執行，並說明原因

```python
print("10" > 3)
```

請回答：

```text

```

---

### 34. 請寫出下面程式的輸出結果，並簡單說明原因

```python
print("10" < "2")
```

答案：

```text

```

---

### 35. 請修正下面錯誤程式，讓它可以判斷輸入年齡是否大於或等於 18

錯誤程式：

```python
age = input("請輸入年齡：")
print(age >= 18)
```

修正後：

```python

```

---

### 36. 請寫出下面程式的輸出結果

```python
print(True == True)
print(True == False)
print(True == "True")
```

答案：

```text

```

---

## Part H：特殊字元與 `%` 格式化

### 37. 請寫出下面程式的輸出結果

```python
print("A\nB")
```

答案：

```text

```

---

### 38. 請寫出下面程式的輸出結果

```python
print("%d" % 20)
print("%s" % 20)
print("%f" % 5)
```

答案：

```text

```

---

### 39. 請寫出下面程式的輸出結果

```python
print("%.2f" % 5)
print("%.3f" % 7)
```

答案：

```text

```

---

### 40. 請寫一個程式：輸入一個整數價格，輸出小數點後固定兩位

範例輸入：

```text
30
```

範例輸出：

```text
30.00
```

請寫程式：

```python

```

---

### 41. 請寫一個程式：輸入一個浮點數 BMI，輸出到小數點後一位

範例輸入：

```text
22
```

範例輸出：

```text
22.0
```

請寫程式：

```python

```

---

## Part I：`.format()` 格式化

### 42. 請寫出下面程式的輸出結果

```python
print("{} {}".format(20, "Hi"))
print("{1} {0}".format("A", "B"))
```

答案：

```text

```

---

### 43. 請寫出下面程式的輸出結果

```python
print("{2}-{0}-{1}".format("A", "B", "C"))
```

答案：

```text

```

---

### 44. 請寫一個函式：回傳 `Hello, name!` 的格式

範例：

```python
q44_name_format("Amy")
```

應該回傳：

```text
Hello, Amy!
```

請寫函式：

```python
def q44_name_format(name):
    
```

---

### 45. 請寫一個函式：回傳 `name: score` 的格式

範例：

```python
q45_score_format("Amy", 90)
```

應該回傳：

```text
Amy: 90
```

請寫函式：

```python
def q45_score_format(name, score):
    
```

---

### 46. 請寫一個函式：回傳三個資料，中間用逗號和一個空格隔開

範例：

```python
q46_three_data(20, 15.5, "Hi")
```

應該回傳：

```text
20, 15.5, Hi
```

請寫函式：

```python
def q46_three_data(a, b, c):
    
```

---

## Part J：綜合應用題

### 47. 自動飲料機：一杯飲料 35 元。輸入投入金額，輸出可以買幾杯，以及剩下多少元

範例輸入：

```text
120
```

範例輸出：

```text
3
15
```

請寫程式：

```python

```

---

### 48. 簡單成績單：輸入姓名和分數，輸出格式為 `姓名 - 分數`，並另外輸出是否及格

範例輸入：

```text
Ben 85
```

範例輸出：

```text
Ben - 85
True
```

請寫程式：

```python

```

---

# 參考答案

## Part A

### 1.

```text
14
20
9
```

### 2.

```text
16
18
25
```

### 3.

```text
8
2
58
```

### 4.

```text
5.0
5
5.25
5
```

### 5.

```python
a, b, c = map(int, input().split())
print((a + b) * c)
print(a + b * c)
print((a + b * c) % 10)
```

### 6.

```python
n = int(input())
print(n // 100)
print(n // 10 % 10)
print(n % 10)
```

---

## Part B

### 7.

```python
n, k = map(int, input().split())
print((n + k - 1) // k)
```

也可以寫成：

```python
n, k = map(int, input().split())
boxes = n // k
if n % k != 0:
    boxes += 1
print(boxes)
```

### 8.

```text
8
83
6
```

### 9.

```python
total_seconds = int(input())
hours = total_seconds // 3600
minutes = total_seconds // 60 % 60
seconds = total_seconds % 60
print(hours, minutes, seconds)
```

### 10.

```python
x = int(input())
square = x ** 2
print(square // 10 % 10)
```

---

## Part C

### 11.

```text
True
False
True
False
```

### 12.

```text
score = 80 是把 80 放進 score 這個變數。
score == 80 是判斷 score 是否等於 80，結果會是 True 或 False。
```

### 13.

```python
score = int(input())
print(score >= 60)
```

### 14.

```python
height = int(input())
print(height >= 120)
```

### 15.

```python
x = int(input())
print(x > 100)
```

---

## Part D

### 16.

```text
True
False
True
False
```

### 17.

```text
True
False
False
```

### 18.

```python
height, age = map(int, input().split())
print(height >= 120 and age >= 10)
```

### 19.

```python
money, member = input().split()
money = int(money)
print(money >= 300 or member == "yes")
```

### 20.

```python
score = int(input())
print(score >= 0 and score <= 100)
```

也可以寫成：

```python
score = int(input())
print(0 <= score <= 100)
```

---

## Part E

### 21.

```text
hellohi
hihihi
```

### 22.

```text
不可以完整執行。第一行可以執行，會輸出 hihi；第二行會錯，因為字串不能乘以字串，只能乘以整數。
```

### 23.

```text
[123, 456]
[123, 123, 123]
```

### 24.

```python
name = input()
print("hi " + name)
```

### 25.

```python
word, count = input().split()
count = int(count)
print(word * count)
```

---

## Part F

### 26.

```text
8
```

### 27.

```text
70
```

### 28.

```text
20
```

### 29.

```text
3
```

### 30.

```text
x += 1 和 x = x + 1 意思相同，都是把 x 原本的值加 1 後再存回 x。
```

### 31.

```text
不是。>= 是比較運算子，用來判斷左邊是否大於或等於右邊，結果是 True 或 False，不會更新變數。
```

---

## Part G

### 32.

```text
False
True
True
```

### 33.

```text
不可以執行。"10" 是字串，3 是整數，字串和整數不能直接比較大小。
```

### 34.

```text
True

因為這是字串比較，不是數字大小比較。Python 會先比較第一個字元，"1" 排在 "2" 前面，所以結果是 True。
```

### 35.

```python
age = int(input("請輸入年齡："))
print(age >= 18)
```

### 36.

```text
True
False
False
```

---

## Part H

### 37.

```text
A
B
```

### 38.

```text
20
20
5.000000
```

### 39.

```text
5.00
7.000
```

### 40.

```python
price = int(input())
print("%.2f" % price)
```

### 41.

```python
bmi = float(input())
print("%.1f" % bmi)
```

---

## Part I

### 42.

```text
20 Hi
B A
```

### 43.

```text
C-A-B
```

### 44.

```python
def q44_name_format(name):
    return "Hello, {}!".format(name)
```

### 45.

```python
def q45_score_format(name, score):
    return "{}: {}".format(name, score)
```

### 46.

```python
def q46_three_data(a, b, c):
    return "{}, {}, {}".format(a, b, c)
```

---

## Part J

### 47.

```python
money = int(input())
price = 35
print(money // price)
print(money % price)
```

### 48.

```python
name, score = input().split()
score = int(score)
print("{} - {}".format(name, score))
print(score >= 60)
```

---
