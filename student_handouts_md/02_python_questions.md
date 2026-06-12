# Python 綜合練習題：輸入輸出、變數、命名、多變數、序列

---

## Part A：觀察輸出結果

### 1. 請寫出下面程式的輸出結果

```python
print("Python")
```

答案：

```text

```

---

### 2. 請寫出下面程式的輸出結果

```python
print(100)
print(200)
```

答案：

```text

```

---

### 3. 請寫出下面程式的輸出結果

```python
print(10 + 5)
print("10 + 5")
```

答案：

```text

```

---

### 4. 請寫出下面程式的輸出結果

```python
name = "Amy"
print("Hello")
print(name)
```

答案：

```text

```

---

### 5. 請寫出下面程式的輸出結果

```python
x = 7
y = 3
print(x + y)
print(x * y)
```

答案：

```text

```

---

## Part B：變數基本概念

### 6. 請寫出下面程式的輸出結果

```python
score = 80
print(score)
```

答案：

```text

```

---

### 7. 請寫出下面程式的輸出結果

```python
age = 12
age = 13
print(age)
```

答案：

```text

```

---

### 8. 請寫出下面程式的輸出結果

```python
x = 5
x = x + 4
print(x)
```

答案：

```text

```

---

### 9. 請寫出下面程式的輸出結果

```python
a = 2
b = a + 3
a = 10
print(b)
```

答案：

```text

```

---

### 10. 請用一句話說明：變數是什麼？

請回答：

```text

```

---

## Part C：變數命名判斷

### 11. 下面哪一個變數名稱是合法的？請圈出或寫出答案。

```text
A. 2name
B. student_name
C. class
D. my-score
```

答案：

```text

```

---

### 12. 下面哪一個變數名稱比較適合存放「學生年齡」？

```text
A. x
B. aaaa
C. student_age
D. 123age
```

答案：

```text

```

---

### 13. 請修正下面錯誤的變數名稱

錯誤程式：

```python
my name = "Tom"
print(my name)
```

修正後：

```python

```

---

### 14. 請修正下面錯誤的變數名稱

錯誤程式：

```python
3cats = 3
print(3cats)
```

修正後：

```python

```

---

### 15. 請判斷下面程式是否可以執行，並說明原因

```python
user_score = 95
print(user_score)
```

請回答：

```text

```

---

## Part D：input() 與資料型態

### 16. 請寫一個程式，讓使用者輸入名字，然後輸出名字

```python

```

---

### 17. 請寫一個程式，讓使用者輸入學校名稱，然後輸出：`你的學校是 XXX`

範例輸入：

```text
Happy School
```

範例輸出：

```text
你的學校是 Happy School
```

請寫程式：

```python

```

---

### 18. 請寫出下面程式的輸出結果

使用者輸入：

```text
12
```

程式：

```python
x = input()
print(x + x)
```

答案：

```text

```

---

### 19. 請寫出下面程式的輸出結果

使用者輸入：

```text
12
```

程式：

```python
x = int(input())
print(x + x)
```

答案：

```text

```

---

### 20. 為什麼第 18 題和第 19 題的結果不同？

請回答：

```text

```

---

## Part E：bool() 基本觀察

### 21. 請寫出下面程式的輸出結果

```python
print(bool("hello"))
print(bool(""))
```

答案：

```text

```

---

### 22. 請寫出下面程式的輸出結果

```python
print(bool(10))
print(bool(0))
```

答案：

```text

```

---

### 23. 請判斷下面程式的輸出結果

```python
word = "Python"
print(bool(word))
```

答案：

```text

```

---

### 24. 請用自己的話說明：`bool()` 大概是在判斷什麼？

請回答：

```text

```

---

## Part F：一行輸入多個資料 split()

### 25. 請寫出下面程式的輸出結果

使用者輸入：

```text
Tom 13
```

程式：

```python
name, age = input().split()
print(name)
print(age)
```

答案：

```text

```

---

### 26. 請寫一個程式，讓使用者同一行輸入兩個單字，然後分別輸出

範例輸入：

```text
red blue
```

範例輸出：

```text
red
blue
```

請寫程式：

```python

```

---

### 27. 請寫一個程式，讓使用者同一行輸入兩個整數，輸出它們的和

範例輸入：

```text
8 9
```

範例輸出：

```text
17
```

請寫程式：

```python

```

---

### 28. 下面程式為什麼會輸出 `89`，不是 `17`？

使用者輸入：

```text
8 9
```

程式：

```python
a, b = input().split()
print(a + b)
```

請回答：

```text

```

---

## Part G：一行定義多個變數

### 29. 請寫出下面程式的輸出結果

```python
x, y = 4, 6
print(x)
print(y)
```

答案：

```text

```

---

### 30. 請寫出下面程式的輸出結果

```python
first, second = "tea", "cake"
print(first)
print(second)
```

答案：

```text

```

---

### 31. 請使用一行程式建立 `width = 5` 和 `height = 8`，並輸出兩個變數的乘積

請寫程式：

```python

```

---

### 32. 請判斷下面程式是否正確，並說明原因

```python
x, y = 10
print(x)
print(y)
```

請回答：

```text

```

---

### 33. 請判斷下面程式是否正確，並說明原因

```python
x, y = 10, 20, 30
print(x)
print(y)
```

請回答：

```text

```

---

## Part H：序列與變數覆蓋

### 34. 請寫出下面程式的輸出結果

```python
x = 1
x = 2
x = 3
print(x)
```

答案：

```text

```

---

### 35. 請寫出下面程式的輸出結果

```python
money = 100
money = money - 30
money = money + 10
print(money)
```

答案：

```text

```

---

### 36. 請寫出下面程式的輸出結果

```python
x = 2
y = x + 5
x = y * 3
print(x)
print(y)
```

答案：

```text

```

---

### 37. 請寫出下面程式的輸出結果

```python
name = "Amy"
print(name)
name = "Ben"
print(name)
```

答案：

```text

```

---

### 38. 請用一句話說明：程式為什麼要由上而下看？

請回答：

```text

```

---

## Part I：括號與執行順序

### 39. 請寫出下面程式的輸出結果

```python
print(2 + 3 * 4)
```

答案：

```text

```

---

### 40. 請寫出下面程式的輸出結果

```python
print((2 + 3) * 4)
```

答案：

```text

```

---

### 41. 請寫出下面程式的輸出結果

```python
x = 10
x = (x + 2) * 3
print(x)
```

答案：

```text

```

---

### 42. 下面兩段程式的輸出有什麼不同？

程式 A：

```python
print(10 - 2 * 3)
```

程式 B：

```python
print((10 - 2) * 3)
```

請回答：

```text

```

---

## Part J：綜合寫程式

### 43. 讓使用者輸入一個整數，輸出它加 100 的結果

範例輸入：

```text
25
```

範例輸出：

```text
125
```

請寫程式：

```python

```

---

### 44. 讓使用者輸入一個整數，先乘以 3，再減掉 2，最後輸出結果

範例輸入：

```text
5
```

範例輸出：

```text
13
```

請寫程式：

```python

```

---

### 45. 讓使用者同一行輸入「姓名 年齡」，輸出兩行資料

範例輸入：

```text
Ivy 14
```

範例輸出：

```text
姓名：Ivy
年齡：14
```

請寫程式：

```python

```

---

### 46. 讓使用者同一行輸入「數量 單價」，輸出總價

範例輸入：

```text
3 50
```

範例輸出：

```text
150
```

請寫程式：

```python

```

---

### 47. 讓使用者輸入目前分數，程式把分數加 5 分後輸出

範例輸入：

```text
80
```

範例輸出：

```text
85
```

請寫程式：

```python

```

---

### 48. 讓使用者輸入一個名字，先輸出原本名字，再把名字改成 `Python Learner`，最後輸出新名字

範例輸入：

```text
Kevin
```

範例輸出：

```text
Kevin
Python Learner
```

請寫程式：

```python

```

---

### 49. 讓使用者輸入兩個整數 `a b`，先輸出 `a + b`，再輸出 `a * b`

範例輸入：

```text
4 7
```

範例輸出：

```text
11
28
```

請寫程式：

```python

```

---

### 50. 小挑戰：讓使用者輸入一個整數 `x`，依序做下面三件事：

1. 先把 `x` 加 10
2. 再把 `x` 乘以 2
3. 最後輸出 `x`

範例輸入：

```text
5
```

範例輸出：

```text
30
```

請寫程式：

```python

```

---

# 參考答案

## Part A

### 1.

```text
Python
```

### 2.

```text
100
200
```

### 3.

```text
15
10 + 5
```

### 4.

```text
Hello
Amy
```

### 5.

```text
10
21
```

---

## Part B

### 6.

```text
80
```

### 7.

```text
13
```

### 8.

```text
9
```

### 9.

```text
5
```

### 10.

```text
變數可以想成一個有名字的盒子，用來存放資料。
```

---

## Part C

### 11.

```text
B. student_name
```

### 12.

```text
C. student_age
```

### 13.

```python
my_name = "Tom"
print(my_name)
```

### 14.

```python
cats3 = 3
print(cats3)
```

也可以寫成：

```python
three_cats = 3
print(three_cats)
```

### 15.

```text
可以執行。user_score 是合法的變數名稱，底線可以用在變數名稱中。
```

---

## Part D

### 16.

```python
name = input()
print(name)
```

### 17.

```python
school = input()
print("你的學校是", school)
```

### 18.

```text
1212
```

### 19.

```text
24
```

### 20.

```text
第 18 題的 x 是字串，所以 x + x 是文字接起來。第 19 題先用 int() 轉成整數，所以 x + x 是數學加法。
```

---

## Part E

### 21.

```text
True
False
```

### 22.

```text
True
False
```

### 23.

```text
True
```

### 24.

```text
bool() 可以用來觀察一個資料在判斷時會被當成 True 還是 False。
```

---

## Part F

### 25.

```text
Tom
13
```

### 26.

```python
word1, word2 = input().split()
print(word1)
print(word2)
```

### 27.

```python
a, b = input().split()
a = int(a)
b = int(b)
print(a + b)
```

也可以寫成：

```python
a, b = map(int, input().split())
print(a + b)
```

### 28.

```text
a 和 b 是字串，所以 a + b 會把文字接在一起，變成 89。要做數學加法，需要先轉成 int。
```

---

## Part G

### 29.

```text
4
6
```

### 30.

```text
tea
cake
```

### 31.

```python
width, height = 5, 8
print(width * height)
```

### 32.

```text
不正確。左邊有兩個變數 x, y，但是右邊只有一個值 10。
```

### 33.

```text
不正確。左邊有兩個變數，但是右邊有三個值，數量不一致。
```

---

## Part H

### 34.

```text
3
```

### 35.

```text
80
```

### 36.

```text
21
7
```

### 37.

```text
Amy
Ben
```

### 38.

```text
因為 Python 會按照程式碼出現的順序執行，後面的指定可能會改變前面的資料。
```

---

## Part I

### 39.

```text
14
```

### 40.

```text
20
```

### 41.

```text
36
```

### 42.

```text
程式 A 先算 2 * 3，所以結果是 4。程式 B 先算括號中的 10 - 2，所以結果是 24。
```

---

## Part J

### 43.

```python
x = int(input())
print(x + 100)
```

### 44.

```python
x = int(input())
x = x * 3 - 2
print(x)
```

### 45.

```python
name, age = input().split()
print("姓名：" + name)
print("年齡：" + age)
```

或：

```python
name, age = input().split()
print("姓名：", name, sep="")
print("年齡：", age, sep="")
```

### 46.

```python
count, price = map(int, input().split())
print(count * price)
```

### 47.

```python
score = int(input())
score = score + 5
print(score)
```

### 48.

```python
name = input()
print(name)
name = "Python Learner"
print(name)
```

### 49.

```python
a, b = map(int, input().split())
print(a + b)
print(a * b)
```

### 50.

```python
x = int(input())
x = x + 10
x = x * 2
print(x)
```

---