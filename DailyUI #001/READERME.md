# DailyUI #001

## 前言

最近開始著墨前端的部分，發現想要呈現的畫面，除了javascript外，連基本的CSS、html排版都無法快速的手刻出來，目前實力大概就套套bootstrap，看到不錯的效果或動畫就複製過來改改的程度而已。

目標是要達到想要甚麼畫面就能快速地刻出來(不套bootstrap)，故用`DailyUI 100`寫個100天來增加我的前端實力。

## 預期完成功能

~~1. 水平垂直置中~~
2. Facebook, Google, GitHub 登入按鈕
3. 密碼強度的Bar
4. 註冊送出loading動畫
5. 當打字時，input預設字移動到旁邊
6. 與LogIn形成兩個Tab
7. 畫面從中往外展開

## 筆記

### 1. 水平垂直置中

先把預設的寬度與長度做出來，若寬為`400px`，則`margin-left`回推`-200px`達到置中的效果，因爲是以左上角的點為基準。

```css=
width: 400px;
height: 400px;
position: absolute;
left: 50%;
top: 50%;
margin-left: -200px;
margin-top: -200px;
```

### 2. 陰影效果

- `text-shadow`
- `box-shadow`

為了使Sign Up的邊框與背景有個區隔，呈現有點浮起來的感覺，所以加入陰影效果`box-shadow: 0px 0px 30px grey;`，參數分別為：X座標、Y座標、模糊度、陰影顏色


> [CSS3 Shadow Effects](https://www.w3schools.com/css/css3_shadows.asp)

### 3. 輸入欄位美化

- `border: none;` // 讓整個邊框消失
- `outline: none;` // 讓點擊的外框消失
- `background: transparent;` // 背景透明
- `border-bottom:1px solid #757575;` // 劃下底線，參數依序為：粗度、類型、顏色

### 4. 按鈕美化

- `border-radius:40px;` // 讓按鈕變回滑
- `border-color: #1AB188;` // 按鈕邊框顏色
- `.btn:hover` // 滑鼠游標碰到事件
- `.btn:focus` // 滑鼠點擊事件

## 總結

> [GitHub]()