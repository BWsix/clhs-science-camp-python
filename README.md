# 科學營 - python課程

## 大綱 / 簡報完成進度

- [ ] [python的規則](#rules)
- [ ] [變數 / 輸入輸出 / 資料型別](#var_io_type)
- [ ] [四則運算](#calculate)
- [ ] [布林 / if else / 大於小於](#bool_if_else)
- [ ] [while loop](#while-loop)
- [ ] [猜數字遊戲](#guess_num_game)

## python的規則 <a name = "rules"></a>

***一開始時，畫面在我們這邊***

- python有很多特性是其他語言沒有的
  - 反之亦然
- 執行的規則
  => 上至下，左至右
- "=" 與 "==" 的差異
  *先不要詳細介紹*
  - "=" 不是數學的等於
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

## 四則運算 <a name = "calculate"></a>


## 布林 / if else / 大於小於<a name = "bool_if_else"></a>


## while loop <a name = "while-loop"></a>


## 猜數字遊戲 <a name = "guess_num_game"></a>

