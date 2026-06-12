# Python 40 題概念練習：`print()`、`sep=`、`end=`、`input()`、變數與資料型態

---

## Part A：觀察 `print()` 預設輸出

### 1. 請寫出下面程式的輸出結果

```python
print("Hello", "Python")
```

答案：

```text

```

---

### 2. 請寫出下面程式的輸出結果

```python
print("A", "B", "C")
```

答案：

```text

```

---

### 3. 請寫出下面程式的輸出結果

```python
name = "Tom"
print("Hello", name)
```

答案：

```text

```

---

### 4. 請寫出下面程式的輸出結果

```python
city = "Taipei"
country = "Taiwan"
print(city, country)
```

答案：

```text

```

---

### 5. 請寫出下面程式的輸出結果

```python
x = 3
y = 5
print(x, y)
```

答案：

```text

```

---

## Part B：理解 `sep=`

### 6. 請寫出下面程式的輸出結果

```python
print("A", "B", "C", sep="-")
```

答案：

```text

```

---

### 7. 請寫出下面程式的輸出結果

```python
print("2026", "06", "07", sep="/")
```

答案：

```text

```

---

### 8. 請寫出下面程式的輸出結果

```python
print("Taipei", "Taichung", "Kaohsiung", sep=" -> ")
```

答案：

```text

```

---

### 9. 請寫出下面程式的輸出結果

```python
print("apple", "banana", "orange", sep=", ")
```

答案：

```text

```

---

### 10. 請寫出下面程式的輸出結果

```python
print("ID", "001", sep=":")
```

答案：

```text

```

---

### 11. 請寫出下面程式的輸出結果

```python
print("Python", "is", "fun", sep="***")
```

答案：

```text

```

---

### 12. 請寫出下面程式的輸出結果

```python
print("A", "B", "C", sep="")
```

答案：

```text

```

---

### 13. 請寫出下面程式的輸出結果

```python
print("A", "B", "C", sep=" ")
```

答案：

```text

```

---

### 14. 請寫出下面程式的輸出結果

```python
print("A", "B", "C", sep=" | ")
```

答案：

```text

```

---

### 15. 請寫出下面程式的輸出結果

```python
print(1, 2, 3, sep="+")
```

答案：

```text

```

---

## Part C：比較有沒有 `sep=`

### 16. 下面兩段程式的輸出有什麼不同？

程式 A：

```python
print("A", "B", "C")
```

程式 B：

```python
print("A", "B", "C", sep="-")
```

請回答：

```text

```

---

### 17. 下面兩段程式的輸出有什麼不同？

程式 A：

```python
print("2026", "06", "07")
```

程式 B：

```python
print("2026", "06", "07", sep="/")
```

請回答：

```text

```

---

### 18. 下面兩段程式的輸出有什麼不同？

程式 A：

```python
print("Taipei", "Taiwan")
```

程式 B：

```python
print("Taipei", "Taiwan", sep=", ")
```

請回答：

```text

```

---

### 19. 下面兩段程式的輸出有什麼不同？

程式 A：

```python
print("A", "B", "C", sep="")
```

程式 B：

```python
print("A", "B", "C", sep=" ")
```

請回答：

```text

```

---

### 20. 請說明 `sep=` 的功能是什麼？

請用自己的話回答：

```text

```

---

## Part D：補上正確的 `sep=`

### 21. 請補上 `sep=`，讓輸出變成 `A-B-C`

```python
print("A", "B", "C", sep=____)
```

答案：

```python

```

---

### 22. 請補上 `sep=`，讓輸出變成 `2026/06/07`

```python
print("2026", "06", "07", sep=____)
```

答案：

```python

```

---

### 23. 請補上 `sep=`，讓輸出變成 `Taipei, Taiwan`

```python
print("Taipei", "Taiwan", sep=____)
```

答案：

```python

```

---

### 24. 請補上 `sep=`，讓輸出變成 `apple | banana | orange`

```python
print("apple", "banana", "orange", sep=____)
```

答案：

```python

```

---

### 25. 請補上 `sep=`，讓輸出變成 `123`

```python
print("1", "2", "3", sep=____)
```

答案：

```python

```

---

## Part E：修正錯誤程式

### 26. 請修正下面的程式，讓它可以輸出 `A-B-C`

錯誤程式：

```python
print("A", "B", "C", "-")
```

修正後：

```python

```

---

### 27. 請修正下面的程式，讓它可以輸出 `2026/06/07`

錯誤程式：

```python
print("2026", "06", "07", "/")
```

修正後：

```python

```

---

### 28. 請修正下面的程式，讓它可以輸出 `Taipei, Taiwan`

錯誤程式：

```python
print("Taipei", "Taiwan", ", ")
```

修正後：

```python

```

---

### 29. 請修正下面的程式，讓它可以輸出 `ID:001`

錯誤程式：

```python
print("ID", "001", sep)
```

修正後：

```python

```

---

### 30. 請修正下面的程式，讓它可以輸出 `A/B/C`

錯誤程式：

```python
print("A", "B", "C", sep=/)
```

修正後：

```python

```

---

## Part F：`sep=` 搭配變數

### 31. 請寫出下面程式的輸出結果

```python
year = "2026"
month = "06"
day = "07"
print(year, month, day, sep="/")
```

答案：

```text

```

---

### 32. 請寫出下面程式的輸出結果

```python
first = "Tom"
last = "Chen"
print(first, last, sep="-")
```

答案：

```text

```

---

### 33. 請寫出下面程式的輸出結果

```python
city = "Taipei"
country = "Taiwan"
print(city, country, sep=", ")
```

答案：

```text

```

---

### 34. 請寫出下面程式的輸出結果

```python
a = 10
b = 20
c = 30
print(a, b, c, sep=" + ")
```

答案：

```text

```

---

### 35. 請寫出下面程式的輸出結果

```python
word1 = "I"
word2 = "love"
word3 = "Python"
print(word1, word2, word3, sep=" ")
```

答案：

```text

```

---

## Part G：自己寫程式

### 36. 請讓使用者輸入年、月、日，並用 `/` 連接輸出

範例輸入：

```text
2026
06
07
```

預期輸出：

```text
2026/06/07
```

請寫程式：

```python

```

---

### 37. 請讓使用者輸入三個城市，並用 ` -> ` 連接輸出

範例輸入：

```text
Taipei
Taichung
Kaohsiung
```

預期輸出：

```text
Taipei -> Taichung -> Kaohsiung
```

請寫程式：

```python

```

---

### 38. 請讓使用者輸入姓和名，並用空格連接輸出

範例輸入：

```text
Chen
Tom
```

預期輸出：

```text
Chen Tom
```

請寫程式：

```python

```

---

### 39. 請讓使用者輸入商品名稱和價格，並用 `: ` 連接輸出

範例輸入：

```text
Apple
30
```

預期輸出：

```text
Apple: 30
```

請寫程式：

```python

```

---

### 40. 請讓使用者輸入三個字母，並讓它們中間不要有任何空格

範例輸入：

```text
A
B
C
```

預期輸出：

```text
ABC
```

請寫程式：

```python

```

---

# 參考答案

## Part A

### 1.

```text
Hello Python
```

### 2.

```text
A B C
```

### 3.

```text
Hello Tom
```

### 4.

```text
Taipei Taiwan
```

### 5.

```text
3 5
```

---

## Part B

### 6.

```text
A-B-C
```

### 7.

```text
2026/06/07
```

### 8.

```text
Taipei -> Taichung -> Kaohsiung
```

### 9.

```text
apple, banana, orange
```

### 10.

```text
ID:001
```

### 11.

```text
Python***is***fun
```

### 12.

```text
ABC
```

### 13.

```text
A B C
```

### 14.

```text
A | B | C
```

### 15.

```text
1+2+3
```

---

## Part C

### 16.

程式 A 會用預設空格分隔，所以輸出 `A B C`。  
程式 B 使用 `sep="-"`，所以輸出 `A-B-C`。

### 17.

程式 A 會輸出 `2026 06 07`。  
程式 B 使用 `sep="/"`，所以輸出 `2026/06/07`。

### 18.

程式 A 會輸出 `Taipei Taiwan`。  
程式 B 使用 `sep=", "`，所以輸出 `Taipei, Taiwan`。

### 19.

程式 A 使用 `sep=""`，所以三個字中間沒有空格，輸出 `ABC`。  
程式 B 使用 `sep=" "`，所以三個字中間有空格，輸出 `A B C`。

### 20.

`sep=` 是用來設定 `print()` 中多個輸出項目之間的分隔符號。  
如果沒有寫 `sep=`，Python 預設會用一個空格分隔。

---

## Part D

### 21.

```python
print("A", "B", "C", sep="-")
```

### 22.

```python
print("2026", "06", "07", sep="/")
```

### 23.

```python
print("Taipei", "Taiwan", sep=", ")
```

### 24.

```python
print("apple", "banana", "orange", sep=" | ")
```

### 25.

```python
print("1", "2", "3", sep="")
```

---

## Part E

### 26.

```python
print("A", "B", "C", sep="-")
```

### 27.

```python
print("2026", "06", "07", sep="/")
```

### 28.

```python
print("Taipei", "Taiwan", sep=", ")
```

### 29.

```python
print("ID", "001", sep=":")
```

### 30.

```python
print("A", "B", "C", sep="/")
```

---

## Part F

### 31.

```text
2026/06/07
```

### 32.

```text
Tom-Chen
```

### 33.

```text
Taipei, Taiwan
```

### 34.

```text
10 + 20 + 30
```

### 35.

```text
I love Python
```

---

## Part G

### 36.

```python
year = input()
month = input()
day = input()
print(year, month, day, sep="/")
```

### 37.

```python
city1 = input()
city2 = input()
city3 = input()
print(city1, city2, city3, sep=" -> ")
```

### 38.

```python
last_name = input()
first_name = input()
print(last_name, first_name, sep=" ")
```

### 39.

```python
item = input()
price = input()
print(item, price, sep=": ")
```

### 40.

```python
a = input()
b = input()
c = input()
print(a, b, c, sep="")
```

---

# 教學提醒

如果學生不會 `sep=`，可以先讓他記住這句話：

```text
sep 是放在 print() 裡面，用來決定「逗號和逗號中間要放什麼」。
```

例如：

```python
print("A", "B", "C", sep="-")
```

意思是：

```text
A 和 B 中間放 -
B 和 C 中間也放 -
所以結果是 A-B-C
```
