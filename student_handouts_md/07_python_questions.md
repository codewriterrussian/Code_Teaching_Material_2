# Python 進階複習題：迴圈流程、狀態控制與資料處理

重點是綜合使用 `for`、`while`、`range()`、串列、索引、累加、條件判斷、`break` 與 `continue`。

- 同時追蹤兩個以上的變數。
- 判斷 `break` 和 `continue` 對流程的影響。
- 使用索引比較相鄰資料。
- 設計正確的停止條件。
- 找出不容易發現的迴圈錯誤。
- 完成需要多個步驟的小型程式。

> 作答規則：
>
> - 除非題目另外說明，不使用串列生成式。
> - 不使用 `sum()`、`max()`、`min()`、`count()`、`index()`。
> - 不使用 `sort()` 或 `sorted()`。
> - 可以使用 `append()`。
> - 請先自行追蹤程式，不要立即執行。
> - 本檔只有題目，不附參考答案。

---

## Part A：進階流程追蹤

### 1. 雙變數累積

請寫出完整輸出。

```python
score = 3
bonus = 1

for round_num in range(1, 5):
    score += round_num
    bonus *= 2

    if score % 2 == 0:
        score += bonus

    print(round_num, score, bonus)
```

答案：

```text

```

---

### 2. `continue` 前後的變數更新

請寫出完整輸出。

```python
total = 0

for number in range(2, 11):
    if number % 3 == 0:
        total += 1
        continue

    total += number
    print(number, total)

print("final:", total)
```

答案：

```text

```

---

### 3. `break` 的判斷位置

請寫出完整輸出。

```python
value = 1

for i in range(1, 8):
    value *= 2

    if value > 20:
        break

    print(i, value)

print("end:", value)
```

答案：

```text

```

---

### 4. 倒序 `range()` 與條件組合

請寫出完整輸出。

```python
result = 0

for number in range(15, 2, -3):
    if number % 2 == 0:
        result -= number
    else:
        result += number

    print(result)
```

答案：

```text

```

---

### 5. 串列元素與索引同時使用

請寫出完整輸出。

```python
values = [4, 7, 2, 9]
result = 0

for i in range(len(values)):
    if i % 2 == 0:
        result += values[i]
    else:
        result -= values[i]

    print(i, result)
```

答案：

```text

```

---

### 6. 兩層條件與跳過規則

請寫出完整輸出。

```python
points = 0

for number in range(1, 13):
    if number % 4 == 0:
        continue

    if number % 3 == 0:
        points += 5
    else:
        points += 1

    if points >= 15:
        break

    print(number, points)

print("score:", points)
```

答案：

```text

```

---

## Part B：`while` 狀態追蹤

### 7. 不固定步長的 `while`

請寫出完整輸出。

```python
number = 3

while number < 25:
    print(number)

    if number % 2 == 0:
        number += 5
    else:
        number *= 2
```

答案：

```text

```

---

### 8. `continue` 是否會造成無限迴圈？

觀察程式：

```python
number = 0

while number < 8:
    if number == 3:
        continue

    print(number)
    number += 1
```

請回答：

1. 程式是否會正常結束？
2. 問題發生在哪一個數值？
3. 為什麼會發生？
4. 請修正程式，讓它跳過 `3`，並繼續印出其他數字。

說明：

```text

```

修正後：

```python

```

---

### 9. 生命值變化

請寫出完整輸出。

```python
hp = 31
turn = 0

while hp > 0:
    turn += 1

    if turn % 3 == 0:
        hp += 4
    else:
        hp -= 9

    print(turn, hp)
```

答案：

```text

```

---

### 10. 登入狀態判斷

下列輸入依序為：

```text
hello
000
123
```

請寫出完整輸出，並說明程式總共詢問幾次帳號與幾次密碼。

```python
correct_username = "hello"
correct_password = "123"

ask_username = True
login = False

while not login:
    if ask_username:
        username = input("Username: ")

    password = input("Password: ")

    if username != correct_username:
        print("Unknown user")
    elif password != correct_password:
        print("Wrong password")
        ask_username = False
    else:
        print("Welcome")
        login = True
```

輸出與說明：

```text

```

---

### 11. 哨兵值停止輸入

程式會依序收到以下整數：

```text
5
-2
7
0
9
```

請寫出最後輸出。

```python
total = 0
valid_count = 0

while True:
    number = int(input())

    if number == 0:
        break

    if number < 0:
        continue

    total += number
    valid_count += 1

print(total)
print(valid_count)
```

答案：

```text

```

---

## Part C：串列與索引處理

### 12. 計算相鄰上升次數

給定串列：

```python
numbers = [3, 7, 5, 8, 8, 12, 4]
```

計算後一個數字比前一個數字大的次數。

本例中：

- `3 → 7` 是上升。
- `5 → 8` 是上升。
- `8 → 12` 是上升。

預期輸出：

```text
3
```

請寫程式：

```python

```

---

### 13. 找出第一次下降的位置

給定串列：

```python
numbers = [2, 5, 9, 11, 8, 13]
```

找出第一次出現「後一個數字小於前一個數字」的位置，並輸出較小數字的索引。

預期輸出：

```text
4
```

限制：找到後必須使用 `break` 停止搜尋。

請寫程式：

```python

```

---

### 14. 交錯加減

完成函式：

```python
def alternating_total(numbers):
    # 索引 0、2、4、... 的數字相加
    # 索引 1、3、5、... 的數字相減
    return None
```

Example:

```python
alternating_total([10, 3, 6, 2, 5])
```

計算方式：

```text
10 - 3 + 6 - 2 + 5
```

應回傳：

```text
16
```

請完成：

```python
def alternating_total(numbers):
    # TODO
    return None
```

---

### 15. 產生差值串列

完成函式：

```python
def differences(numbers):
    # 回傳每組相鄰數字的「後者減前者」
    return None
```

Example:

```python
differences([4, 9, 6, 10])
```

應回傳：

```text
[5, -3, 4]
```

請完成：

```python
def differences(numbers):
    # TODO
    return None
```

---

### 16. 壓縮連續重複資料

完成函式，只保留每一段連續重複資料的第一個值。

Example:

```python
compress_adjacent([1, 1, 1, 3, 3, 2, 2, 5])
```

應回傳：

```text
[1, 3, 2, 5]
```

注意：

```python
compress_adjacent([1, 2, 1])
```

應回傳：

```text
[1, 2, 1]
```

請完成：

```python
def compress_adjacent(values):
    # TODO
    return None
```

---

### 17. 修改指定索引的資料

給定：

```python
scores = [55, 72, 48, 91, 63]
```

請直接修改原串列：

- 小於 `60` 的分數加 `10`。
- 大於或等於 `90` 的分數改成 `100`。
- 其他分數不變。

預期結果：

```text
[65, 72, 58, 100, 63]
```

請寫程式：

```python

```

---

### 18. 找出最長連續正數段

完成函式，回傳串列中最長的「連續正數」長度。

Example:

```python
longest_positive_run([2, 5, -1, 3, 4, 8, 0, 7])
```

各段正數長度為：

```text
2、3、1
```

應回傳：

```text
3
```

請完成：

```python
def longest_positive_run(numbers):
    # TODO
    return None
```

---

## Part D：除錯與程式修復

### 19. 預期跳過偶數，但結果錯誤

錯誤程式：

```python
number = 1

while number <= 10:
    if number % 2 == 0:
        continue

    print(number)
    number += 1
```

請回答：

1. 程式在哪裡卡住？
2. 為什麼？
3. 修正後應印出 `1、3、5、7、9`。

問題說明：

```text

```

修正後：

```python

```

---

### 20. 錯誤的相鄰比較範圍

下面程式想比較每一組相鄰元素，但會出現錯誤。

```python
values = [4, 6, 3, 8]

for i in range(len(values)):
    if values[i + 1] > values[i]:
        print("up")
```

請回答：

1. 會出現什麼類型的問題？
2. 問題發生在最後一次迴圈的哪個索引？
3. 請修正 `range()`。

說明：

```text

```

修正後：

```python

```

---

### 21. `break` 放錯位置

下面程式想找出第一個大於 `20` 的數字。

```python
numbers = [8, 15, 23, 19, 30]

for number in numbers:
    if number > 20:
        found = number
    break

print(found)
```

請說明問題並修正。

問題說明：

```text

```

修正後：

```python

```

---

### 22. 累加器在錯誤的位置重設

下面程式想計算每個數字的各位數字總和。

例如 `352` 的各位數字總和是 `3 + 5 + 2 = 10`。

錯誤程式：

```python
number = 352

while number > 0:
    digit_sum = 0
    digit_sum += number % 10
    number //= 10

print(digit_sum)
```

請說明錯誤並修正。

問題說明：

```text

```

修正後：

```python

```

---

### 23. 條件順序導致規則無法執行

規則：

- 可以被 `6` 整除時印出 `Six`。
- 否則，可以被 `3` 整除時印出 `Three`。
- 否則，可以被 `2` 整除時印出 `Two`。

錯誤程式：

```python
number = 12

if number % 3 == 0:
    print("Three")
elif number % 2 == 0:
    print("Two")
elif number % 6 == 0:
    print("Six")
```

請說明為什麼不會印出 `Six`，並修正條件順序。

說明：

```text

```

修正後：

```python

```

---

### 24. 空串列的初始值問題

下面函式想找出第一個負數，但空串列時會出現問題。

```python
def first_negative(numbers):
    answer = numbers[0]

    for number in numbers:
        if number < 0:
            answer = number
            break

    return answer
```

請修改函式，使它：

- 找到第一個負數時回傳該數字。
- 沒有負數時回傳 `None`。
- 空串列時也回傳 `None`。

請完成：

```python
def first_negative(numbers):
    # TODO
    return None
```

---

## Part E：D–E Level 小型應用

### 25. 有限次數密碼驗證

設定正確密碼為 `"2468"`。

使用者最多可以輸入三次：

- 輸入正確時印出 `Access granted`，並立即停止。
- 三次都錯時印出 `Account locked`。
- 成功後不可再要求輸入。

請使用 `while` 和 `break`。

```python

```

---

### 26. 數字猜測提示

設定答案：

```python
answer = 37
```

讓使用者持續輸入整數：

- 太小時印出 `Too low`。
- 太大時印出 `Too high`。
- 正確時印出 `Correct`，並停止。
- 同時記錄總共猜了幾次，最後印出次數。

請寫程式：

```python

```

---

### 27. 第一個符合兩個條件的數字

從 `100` 開始往上尋找第一個同時符合下列條件的整數：

- 可以被 `7` 整除。
- 除以 `5` 的餘數是 `2`。

找到後輸出該數字並停止。

限制：

- 使用迴圈。
- 不可直接手算後只印答案。

請寫程式：

```python

```

---

### 28. 購物預算模擬

給定商品價格：

```python
prices = [120, 80, 250, 60, 140, 90]
budget = 500
```

依序購買商品：

- 商品價格小於 `100` 時，跳過不買。
- 如果買下目前商品會超過預算，立刻停止購物。
- 否則扣除價格，並記錄購買件數。

最後輸出：

```text
items: 購買件數
remaining: 剩餘預算
```

請寫程式：

```python

```

---

### 29. 連續錯誤偵測

給定作答紀錄：

```python
answers = [True, False, False, True, False, False, False, True]
```

請找出是否曾出現連續三次 `False`：

- 有出現時，輸出第三次錯誤的索引並停止。
- 沒有出現時，輸出 `No warning`。

本例預期輸出：

```text
6
```

請寫程式：

```python

```

---

### 30. 簡易提款流程

初始餘額：

```python
balance = 1000
```

使用者重複輸入提款金額：

- 輸入 `0` 時結束。
- 輸入負數時印出 `Invalid amount`，並跳過。
- 提款金額大於餘額時印出 `Insufficient funds`，不扣款。
- 合法提款時扣除餘額並印出新餘額。
- 餘額變成 `0` 時自動停止。

請寫程式：

```python

```

---

### 31. 檢查是否為質數

完成函式：

```python
def is_prime(n):
    # n 小於 2 時回傳 False
    # 檢查是否存在 2 到 n-1 之間的因數
    # 找到因數後可以立刻停止
    return None
```

Examples:

```python
is_prime(2)
```

回傳：

```text
True
```

```python
is_prime(15)
```

回傳：

```text
False
```

請完成：

```python
def is_prime(n):
    # TODO
    return None
```

---

### 32. 第一個不重複的字元

完成函式，回傳字串中第一個只出現一次的字元。

限制：不使用 `count()`。

Example:

```python
first_unique_char("aabbcddee")
```

應回傳：

```text
c
```

若所有字元都重複，回傳 `None`。

請完成：

```python
def first_unique_char(text):
    # TODO
    return None
```

---

### 33. 數字反轉

完成函式，不可把整數轉成字串。

```python
def reverse_number(n):
    # 使用 while、%、// 完成
    return None
```

Example:

```python
reverse_number(4072)
```

應回傳：

```text
2704
```

請完成：

```python
def reverse_number(n):
    # TODO
    return None
```

---

### 34. 數字是否為回文

利用數字反轉概念，判斷正整數從左讀和從右讀是否相同。

Examples:

```python
is_number_palindrome(1221)
```

回傳：

```text
True
```

```python
is_number_palindrome(1231)
```

回傳：

```text
False
```

限制：不可把數字轉成字串。

請完成：

```python
def is_number_palindrome(n):
    # TODO
    return None
```

---

### 35. 最長不下降連續段

完成函式，回傳串列中最長的「不下降連續段」長度。

不下降代表後一個數字大於或等於前一個數字。

Example:

```python
longest_non_decreasing_run([2, 2, 5, 3, 4, 4, 7, 1])
```

連續段為：

```text
[2, 2, 5]
[3, 4, 4, 7]
[1]
```

應回傳：

```text
4
```

請完成：

```python
def longest_non_decreasing_run(numbers):
    # TODO
    return None
```

---

## Part F：綜合挑戰

### 36. 學生成績趨勢分析

給定：

```python
scores = [62, 68, 68, 73, 59, 64, 70]
```

請完成：

1. 計算分數上升的次數。
2. 計算分數下降的次數。
3. 計算分數不變的次數。
4. 找出第一次下降後的分數索引。
5. 不使用 `count()`。

輸出格式：

```text
up: 上升次數
down: 下降次數
same: 不變次數
first drop index: 索引
```

請寫程式：

```python

```

---

### 37. 遊戲關卡模擬

初始設定：

```python
energy = 25
coins = 0
```

關卡難度：

```python
levels = [4, 7, 3, 9, 5, 8]
```

規則：

- 每進入一關，消耗等同關卡難度的能量。
- 難度小於 `5` 的關卡不獲得金幣。
- 難度為 `5` 到 `7` 時獲得 `10` 枚金幣。
- 難度大於 `7` 時獲得 `20` 枚金幣。
- 如果進入下一關前的能量不足以支付該關消耗，停止遊戲。
- 最後輸出完成關卡數、剩餘能量與金幣。

請寫程式：

```python

```

---

### 38. 連續登入失敗鎖定

輸入多組帳號與密碼，規則如下：

- 正確帳號：`student`
- 正確密碼：`python`
- 帳號錯誤時印出 `Unknown account`。
- 帳號正確但密碼錯誤時印出 `Wrong password`。
- 連續三次失敗時印出 `Locked` 並停止。
- 登入成功時印出 `Login success` 並停止。
- 任一次成功前的所有錯誤都算失敗。

請使用 `while`。

```python

```

---

### 39. 資料清理

給定：

```python
readings = [12, -1, 15, 999, 18, -3, 20, 21]
```

規則：

- 負數是無效資料，跳過。
- `999` 代表感測器停止，遇到後立刻停止讀取。
- 有效資料加入新的串列。
- 同時計算有效資料總和與數量。
- 最後輸出有效資料串列與平均值。
- 若沒有有效資料，輸出 `No valid data`。

請寫程式：

```python

```

---

### 40. 自訂挑戰：設計測試資料

請為以下函式設計至少 **5 組測試資料**，必須包含：

- 一般情況。
- 只有一個元素。
- 全部相同。
- 一開始就下降。
- 最長不下降段出現在最後。

```python
def longest_non_decreasing_run(numbers):
    # 已由第 35 題完成
    pass
```

請填寫：

```python
# Test 1:

# Test 2:

# Test 3:

# Test 4:

# Test 5:
```

並在每組測試旁寫出預期答案。
