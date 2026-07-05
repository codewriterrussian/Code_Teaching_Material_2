# Python 條件判斷複習題：`if`、`elif`、`else`（C Level）

難度說明：本份題目是 **C 等級**，比 A 等級更重視「追蹤流程、判斷順序、除錯、邊界條件、巢狀判斷與小型應用」。

---

## Part A：流程追蹤與輸出判斷

### 1. 請寫出下面程式的輸出結果，並注意哪幾個 `if` 會被執行

```python
x = 12

if x > 10:
    print("A")
if x % 2 == 0:
    print("B")
if x < 5:
    print("C")

print("Done")
```

答案：

```text

```

---

### 2. 請寫出下面程式的輸出結果，並說明為什麼只會進入其中一個分支

```python
score = 75

if score >= 90:
    print("A")
elif score >= 80:
    print("B")
elif score >= 70:
    print("C")
else:
    print("D")
```

答案：

```text

```

說明：

```text

```

---

### 3. 請寫出下面程式的輸出結果，注意 `if` 和 `elif` 的差別

```python
x = 20

if x >= 10:
    print("big")
if x >= 15:
    print("very big")
else:
    print("small")
```

答案：

```text

```

---

### 4. 請寫出下面程式的輸出結果

```python
n = 9

if n % 2 == 0:
    print("even")
elif n % 3 == 0:
    print("three")
elif n % 9 == 0:
    print("nine")
else:
    print("other")
```

答案：

```text

```

請回答：為什麼沒有輸出 `nine`？

```text

```

---

### 5. 請寫出下面程式的輸出結果，並注意縮排

```python
x = -3

if x > 0:
    print("positive")
    print("inside")
print("outside")
```

答案：

```text

```

---

## Part B：條件順序與邊界條件

### 6. 請寫出下面程式在不同輸入下的輸出結果

```python
score = int(input())

if score > 60:
    print("pass")
else:
    print("fail")
```

| 輸入 | 輸出 |
| --- | --- |
| `59` |  |
| `60` |  |
| `61` |  |

---

### 7. 上一題如果希望 `60` 也算及格，應該修改哪一行？

請寫出修改後的判斷式：

```python

```

---

### 8. 請判斷下面程式的分類是否正確。如果不正確，請說明問題

```python
score = int(input())

if score >= 0:
    print("valid")
elif score >= 60:
    print("pass")
else:
    print("invalid")
```

問題說明：

```text

```

---

### 9. 請修正上一題，讓程式可以做到：

- 分數小於 0 或大於 100：輸出 `invalid`
- 分數 60 到 100：輸出 `pass`
- 分數 0 到 59：輸出 `fail`

請寫程式：

```python

```

---

### 10. 請寫一個程式：輸入溫度 `t`

規則：

- `t >= 35`：輸出 `hot`
- `20 <= t < 35`：輸出 `warm`
- `t < 20`：輸出 `cold`

範例輸入：

```text
28
```

範例輸出：

```text
warm
```

請寫程式：

```python

```

---

## Part C：`and`、`or` 與條件組合

### 11. 請寫出下面程式的輸出結果

```python
age = 13
height = 125

if age >= 12 and height >= 120:
    print("OK")
else:
    print("NO")
```

答案：

```text

```

---

### 12. 請寫出下面程式的輸出結果，注意 `and` 會比 `or` 先判斷

```python
x = 5

if x < 3 or x > 10 and x % 2 == 0:
    print("A")
else:
    print("B")
```

答案：

```text

```

---

### 13. 請在下面程式加上括號，讓條件變得更清楚，但不要改變原本意思

```python
if x < 3 or x > 10 and x % 2 == 0:
    print("A")
```

修改後：

```python

```

---

### 14. 請寫一個程式：輸入 `age` 和 `ticket`

規則：

- 年齡至少 12 歲，且票種是 `yes`，輸出 `enter`
- 否則輸出 `stop`

範例輸入：

```text
15 yes
```

範例輸出：

```text
enter
```

請寫程式：

```python

```

---

### 15. 請寫一個程式：輸入消費金額 `money` 和會員狀態 `member`

規則：

- 金額至少 1000，或會員狀態是 `vip`，輸出 `discount`
- 其他情況輸出 `normal`

請寫程式：

```python

```

---

### 16. 請寫一個程式：輸入一個整數 `x`，如果 `x` 在 10 到 99 之間，包含 10 和 99，輸出 `two-digit`，否則輸出 `other`

請寫程式：

```python

```

---

## Part D：多分支分類題

### 17. 請寫一個程式：輸入分數 `score`，輸出等第

規則：

- 90 到 100：`A`
- 80 到 89：`B`
- 70 到 79：`C`
- 60 到 69：`D`
- 0 到 59：`E`
- 其他數字：`invalid`

請寫程式：

```python

```

---

### 18. 請寫一個程式：輸入一個整數 `n`，判斷它是正數、負數，還是零

輸出規則：

- 正數：`positive`
- 負數：`negative`
- 零：`zero`

請寫程式：

```python

```

---

### 19. 請寫一個程式：輸入一個整數 `n`

規則：

- 如果是 3 和 5 的倍數，輸出 `both`
- 如果只是 3 的倍數，輸出 `three`
- 如果只是 5 的倍數，輸出 `five`
- 否則輸出 `other`

請注意判斷順序。

請寫程式：

```python

```

---

### 20. 請寫一個程式：輸入月份 `m`，輸出季節

規則：

- 3、4、5：`spring`
- 6、7、8：`summer`
- 9、10、11：`autumn`
- 12、1、2：`winter`
- 其他：`invalid`

請寫程式：

```python

```

---

### 21. 請寫一個程式：輸入一個年份 `year`，判斷是否為閏年

簡化規則：

- 能被 4 整除就是閏年，輸出 `leap`
- 否則輸出 `normal`

請寫程式：

```python

```

---

## Part E：巢狀條件判斷

### 22. 請寫出下面程式在不同輸入下的輸出結果

```python
age = int(input())

if age >= 18:
    if age >= 65:
        print("senior")
    else:
        print("adult")
else:
    print("student")
```

| 輸入 | 輸出 |
| --- | --- |
| `15` |  |
| `18` |  |
| `65` |  |

---

### 23. 請把上一題改寫成 `if...elif...else`，不要使用巢狀 `if`

請寫程式：

```python

```

---

### 24. 請寫一個程式：輸入帳號 `user` 和密碼 `password`

規則：

- 如果帳號不是 `admin`，輸出 `wrong user`
- 如果帳號是 `admin`，但密碼不是 `1234`，輸出 `wrong password`
- 如果帳號是 `admin` 且密碼是 `1234`，輸出 `login success`

請用巢狀 `if` 完成。

請寫程式：

```python

```

---

### 25. 請把上一題改寫成不使用巢狀 `if` 的版本

請寫程式：

```python

```

---

## Part F：除錯題

### 26. 下面程式有錯，請修正

錯誤程式：

```python
score = input()

if score >= 60:
    print("pass")
else:
    print("fail")
```

錯誤原因：

```text

```

修正後：

```python

```

---

### 27. 下面程式有錯，請修正

錯誤程式：

```python
x = int(input())

if x > 0
    print("positive")
```

錯誤原因：

```text

```

修正後：

```python

```

---

### 28. 下面程式邏輯有問題，請修正

錯誤程式：

```python
score = int(input())

if score >= 60:
    print("pass")
if score >= 80:
    print("good")
else:
    print("fail")
```

問題：輸入 `70` 時，會輸出什麼？

```text

```

如果想要：

- 80 以上輸出 `good`
- 60 到 79 輸出 `pass`
- 60 以下輸出 `fail`

請修正程式：

```python

```

---

### 29. 下面程式想判斷 `x` 是否等於 10，但寫錯了。請修正

錯誤程式：

```python
x = int(input())

if x = 10:
    print("yes")
else:
    print("no")
```

錯誤原因：

```text

```

修正後：

```python

```

---

### 30. 下面程式的縮排有問題，請修正

錯誤程式：

```python
x = int(input())

if x > 0:
print("positive")
else:
print("not positive")
```

修正後：

```python

```

---

## Part G：小型應用題

### 31. 自動售票機：輸入年齡 `age`

規則：

- 0 到 5 歲：`free`
- 6 到 17 歲：`child ticket`
- 18 到 64 歲：`adult ticket`
- 65 歲以上：`senior ticket`
- 負數：`invalid`

請寫程式：

```python

```

---

### 32. 簡單登入系統：輸入帳號、密碼、驗證碼

規則：

- 帳號必須是 `student`
- 密碼必須是 `python`
- 驗證碼必須是 `8888`
- 三個都正確才輸出 `success`
- 否則輸出 `fail`

請寫程式：

```python

```

---

### 33. 簡單 BMI 分類：輸入 BMI 值

規則：

- 小於 18.5：`underweight`
- 18.5 到小於 24：`normal`
- 24 到小於 27：`overweight`
- 27 以上：`obese`

請寫程式：

```python

```

---

### 34. 輸入三個整數 `a b c`，輸出最大的數字

限制：不要使用 `max()`。

請寫程式：

```python

```

---

### 35. 輸入三個整數 `a b c`，判斷是否可以形成三角形

規則：任兩邊相加都必須大於第三邊。

- 可以形成三角形：輸出 `triangle`
- 否則輸出 `not triangle`

請寫程式：

```python

```

---

### 36. 輸入一個整數 `n`，判斷它是幾位數

規則：

- 0 到 9：`one digit`
- 10 到 99：`two digits`
- 100 到 999：`three digits`
- 其他：`other`

請寫程式：

```python

```

---

## Part H：綜合挑戰題

### 37. 運費計算：輸入購物金額 `money` 和是否為會員 `member`

規則：

- 如果會員是 `yes`，且金額大於等於 500，輸出 `free shipping`
- 如果會員是 `yes`，但金額小於 500，輸出 `shipping 60`
- 如果不是會員，但金額大於等於 1000，輸出 `free shipping`
- 其他情況輸出 `shipping 100`

請寫程式：

```python

```

---

### 38. 考試結果：輸入筆試分數 `written` 和口試分數 `oral`

規則：

- 兩科都至少 60：輸出 `pass`
- 只有筆試不及格：輸出 `written fail`
- 只有口試不及格：輸出 `oral fail`
- 兩科都不及格：輸出 `both fail`

請寫程式：

```python

```

---

### 39. 簡易計算機：輸入兩個整數 `a b` 和一個運算符號 `op`

規則：

- `op` 是 `+`：輸出 `a + b`
- `op` 是 `-`：輸出 `a - b`
- `op` 是 `*`：輸出 `a * b`
- `op` 是 `/`：輸出 `a / b`
- 其他符號：輸出 `invalid`

範例輸入：

```text
8 3 *
```

範例輸出：

```text
24
```

請寫程式：

```python

```

---

### 40. 數字特徵判斷：輸入一個整數 `n`

規則：

- 如果 `n` 是偶數且大於 100，輸出 `big even`
- 如果 `n` 是偶數但不大於 100，輸出 `small even`
- 如果 `n` 是奇數且大於 100，輸出 `big odd`
- 如果 `n` 是奇數但不大於 100，輸出 `small odd`

請寫程式：

```python

```

---

# 參考答案

## Part A

### 1.

```text
A
B
Done
```

### 2.

```text
C
```

說明：

```text
if...elif...else 只會執行第一個符合條件的分支。score 是 75，不符合 90 和 80，但符合 70，所以輸出 C 後就結束整組判斷。
```

### 3.

```text
big
very big
```

### 4.

```text
three
```

說明：

```text
因為 n = 9 先符合 n % 3 == 0，所以執行 three。elif 後面的條件不會再判斷。
```

### 5.

```text
outside
```

---

## Part B

### 6.

| 輸入 | 輸出 |
| --- | --- |
| `59` | `fail` |
| `60` | `fail` |
| `61` | `pass` |

### 7.

```python
if score >= 60:
```

### 8.

```text
不正確。因為 score >= 0 放在最前面，只要分數是 0 以上，就會先輸出 valid，後面的 score >= 60 永遠沒有機會被執行。
```

### 9.

```python
score = int(input())

if score < 0 or score > 100:
    print("invalid")
elif score >= 60:
    print("pass")
else:
    print("fail")
```

### 10.

```python
t = int(input())

if t >= 35:
    print("hot")
elif t >= 20:
    print("warm")
else:
    print("cold")
```

---

## Part C

### 11.

```text
OK
```

### 12.

```text
B
```

### 13.

```python
if x < 3 or (x > 10 and x % 2 == 0):
    print("A")
```

### 14.

```python
age, ticket = input().split()
age = int(age)

if age >= 12 and ticket == "yes":
    print("enter")
else:
    print("stop")
```

### 15.

```python
money, member = input().split()
money = int(money)

if money >= 1000 or member == "vip":
    print("discount")
else:
    print("normal")
```

### 16.

```python
x = int(input())

if x >= 10 and x <= 99:
    print("two-digit")
else:
    print("other")
```

也可以寫成：

```python
x = int(input())

if 10 <= x <= 99:
    print("two-digit")
else:
    print("other")
```

---

## Part D

### 17.

```python
score = int(input())

if score < 0 or score > 100:
    print("invalid")
elif score >= 90:
    print("A")
elif score >= 80:
    print("B")
elif score >= 70:
    print("C")
elif score >= 60:
    print("D")
else:
    print("E")
```

### 18.

```python
n = int(input())

if n > 0:
    print("positive")
elif n < 0:
    print("negative")
else:
    print("zero")
```

### 19.

```python
n = int(input())

if n % 3 == 0 and n % 5 == 0:
    print("both")
elif n % 3 == 0:
    print("three")
elif n % 5 == 0:
    print("five")
else:
    print("other")
```

### 20.

```python
m = int(input())

if m == 3 or m == 4 or m == 5:
    print("spring")
elif m == 6 or m == 7 or m == 8:
    print("summer")
elif m == 9 or m == 10 or m == 11:
    print("autumn")
elif m == 12 or m == 1 or m == 2:
    print("winter")
else:
    print("invalid")
```

### 21.

```python
year = int(input())

if year % 4 == 0:
    print("leap")
else:
    print("normal")
```

---

## Part E

### 22.

| 輸入 | 輸出 |
| --- | --- |
| `15` | `student` |
| `18` | `adult` |
| `65` | `senior` |

### 23.

```python
age = int(input())

if age >= 65:
    print("senior")
elif age >= 18:
    print("adult")
else:
    print("student")
```

### 24.

```python
user, password = input().split()

if user == "admin":
    if password == "1234":
        print("login success")
    else:
        print("wrong password")
else:
    print("wrong user")
```

### 25.

```python
user, password = input().split()

if user != "admin":
    print("wrong user")
elif password != "1234":
    print("wrong password")
else:
    print("login success")
```

---

## Part F

### 26.

錯誤原因：

```text
input() 讀進來的是字串，不能直接和整數 60 比較大小，需要先轉成 int。
```

修正後：

```python
score = int(input())

if score >= 60:
    print("pass")
else:
    print("fail")
```

### 27.

錯誤原因：

```text
if 條件式後面少了冒號 :。
```

修正後：

```python
x = int(input())

if x > 0:
    print("positive")
```

### 28.

輸入 `70` 時會輸出：

```text
pass
fail
```

修正後：

```python
score = int(input())

if score >= 80:
    print("good")
elif score >= 60:
    print("pass")
else:
    print("fail")
```

### 29.

錯誤原因：

```text
= 是指定值，== 才是判斷是否相等。if 後面要放條件判斷，不可以用 x = 10。
```

修正後：

```python
x = int(input())

if x == 10:
    print("yes")
else:
    print("no")
```

### 30.

```python
x = int(input())

if x > 0:
    print("positive")
else:
    print("not positive")
```

---

## Part G

### 31.

```python
age = int(input())

if age < 0:
    print("invalid")
elif age <= 5:
    print("free")
elif age <= 17:
    print("child ticket")
elif age <= 64:
    print("adult ticket")
else:
    print("senior ticket")
```

### 32.

```python
user, password, code = input().split()

if user == "student" and password == "python" and code == "8888":
    print("success")
else:
    print("fail")
```

### 33.

```python
bmi = float(input())

if bmi < 18.5:
    print("underweight")
elif bmi < 24:
    print("normal")
elif bmi < 27:
    print("overweight")
else:
    print("obese")
```

### 34.

```python
a, b, c = map(int, input().split())

largest = a
if b > largest:
    largest = b
if c > largest:
    largest = c

print(largest)
```

也可以寫成：

```python
a, b, c = map(int, input().split())

if a >= b and a >= c:
    print(a)
elif b >= a and b >= c:
    print(b)
else:
    print(c)
```

### 35.

```python
a, b, c = map(int, input().split())

if a + b > c and a + c > b and b + c > a:
    print("triangle")
else:
    print("not triangle")
```

### 36.

```python
n = int(input())

if 0 <= n <= 9:
    print("one digit")
elif 10 <= n <= 99:
    print("two digits")
elif 100 <= n <= 999:
    print("three digits")
else:
    print("other")
```

---

## Part H

### 37.

```python
money, member = input().split()
money = int(money)

if member == "yes":
    if money >= 500:
        print("free shipping")
    else:
        print("shipping 60")
else:
    if money >= 1000:
        print("free shipping")
    else:
        print("shipping 100")
```

### 38.

```python
written, oral = map(int, input().split())

if written >= 60 and oral >= 60:
    print("pass")
elif written < 60 and oral < 60:
    print("both fail")
elif written < 60:
    print("written fail")
else:
    print("oral fail")
```

### 39.

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
    print("invalid")
```

### 40.

```python
n = int(input())

if n % 2 == 0:
    if n > 100:
        print("big even")
    else:
        print("small even")
else:
    if n > 100:
        print("big odd")
    else:
        print("small odd")
```

也可以寫成：

```python
n = int(input())

if n % 2 == 0 and n > 100:
    print("big even")
elif n % 2 == 0:
    print("small even")
elif n > 100:
    print("big odd")
else:
    print("small odd")
```
