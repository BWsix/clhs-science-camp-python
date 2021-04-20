# 科學營 - python課程

## 大綱

- [python的規則](#rules)
- [變數 / 輸入輸出 / 資料型別](#var_io_type)
- [四則運算](#calculate)
- [布林 / if else / 大於小於](#bool_if_else)
- [while loop](#while-loop)
- [猜數字遊戲](#guess_num_game)

## python的規則 <a name = "rules"></a>

***一開始時，畫面在我們這邊***

- python有很多特性是其他語言沒有的
  - 反之亦然
- 執行的規則
  => 上至下，左至右
- "=" 與 "==" 的差異
  *先不要詳細介紹*
  - "=" 是跟變數有關
  - "==" 是數學的等於

***講完後切還畫面***

## 變數 / 輸入輸出 / 資料型別 <a name = "var_io_type"></a>

- [變數 / print() / input()](#0101)
- [型別](#0102)
- [再談input() / 用type()確認型別](#0103)
- [型別的轉換](#0104)

### 變數 / print() / input() <a name = "0101"></a>

***拿到畫面後會有下面這段程式碼，開始講解接下來的內容前先請同學試試看***

```python
name = input()
print(name)
```

***收回來並開始講解***

- input()
  => 用來讀取使用者的輸入
  - *先講這樣就好*
- 變數
  => 儲存資料
  - 取名限制
    - 數字不可在第一個字元
    - 不可有任何符號( 除了底線 : _ )
  - 如何取名
    - 要取有意義的單字
    - 避開保留字
      - python預設的語法
      - *先舉例 input 就好*
- print()
  => 印出東西
  - print(如何印出, 多個東西)
    - ***把剛才的程式改成*** :

      ```python
      name = input()
      print('hello', name)
      ```

      *先不解釋 'hello' 為何要用引號包起來*

### 型別 <a name = "0102"></a>

*把剛才的 <code>print('hello', name)</code> 單印號刪掉*
*變成 <code>print(hello, name)</code>*

***發現出錯後接著講字串***

- str : 字串
  - 被" "包圍
    => 可以是 '單引號' 或是 "雙引號"
  - **為何要被包圍**
    => 不包圍的話python會以為他是變數
    - *再刪掉一次，並看錯誤訊息寫甚麼*
- int : 整數
- float : 小數

### 再談input() / 用type()確認型別 <a name = "0103"></a>

- input()
  - input('可以加文字，但只限字串')
  - 回傳型別為str
- type()
  - *用type()檢驗 int, str, float*
  - *用type()檢驗 input()*

### 型別的轉換 <a name = "0104"></a>

- int()
  - int(str)
  - int(float)
- str()
  - str(int)
  - str(float)

***把剛剛的程式改成***

```python
number_a = int(input())
number_b = int(input())

print(number_a + number_b)
```

## 四則運算 <a name = "calculate"></a>

- "+ - * /"
  - int 類型可以用全部
  - str 類型可以用 "+ - *"

```python
name = input()
print('hello ' + name)
```

## 布林 / if else / 大於小於<a name = "bool_if_else"></a>

- True / False
  - 介紹==
    - 同類型的可以比

    ```python
    name = input()
    print(name == 'admin')
    ```

- if

  ```python
  if True:
    print('true')

  if False:
    print('false')
  ```

- 介紹縮排
  - 格數要一致
  - 一般會是4或2格(我都用兩格)

- else
  - 如果if沒有被執行才會被執行
  - else後面不能接東西
  - 如果要多個判斷, 用elif(當作自己查的練習題)

  ```python
  if True:
    print('true')
  else: #分別加上else
    print('first else')

  if False:
    print('false')
  else: #分別加上else
    print('second else')
  ```

  - 練習
    1. 用input()讀入數字
    1. 用int()轉成"int型態"
    1. 如果等於10, 用print()印出"等於"
    1. 否則, 用print()印出"不等於"

    ```python
    number = int(input())
    if number == 10:
      print('number is 10')
    elif number == 20:
      print('number is 20')
    else:
      print('不等於')
    ```

- 大於小於
  - 跟==很像, 可以接在if後面
    - \>, <, >=, <=, ==, !=

    ```python
    number = int(input())
    if number > 10:
      print('大於')
    else:
      print('小於')
    ```


## while loop <a name = "while-loop"></a>


## 猜數字遊戲 <a name = "guess_num_game"></a>

```python

rand_num = 10 # 要猜的數字

while True: # 以下會重複執行
  user_input = int(input())

  if user_input > rand_num:
    print("猜錯了! 再小一點")

  if user_input < rand_num:
    print("猜錯了! 再大一點")

  if user_input == rand_num:
    print("Bingo!")
    break
```
