# DesignIdea

- 版面設計和詳細內容請參閱 [Figma](https://www.figma.com/file/YnZizHfB3NIVWfzyog87UG/resl-website-redesign?node-id=0%3A1&t=ZgK18w2rFzxYds1J-1) (**設計並不完全一致**)

- 本專案的[參考來源網站](https://resl.csie.nptu.edu.tw/joomla3/index.php)

## index

- 原先的首頁相當簡易樸素。我參考課程中 Portfolio 的整體架構，並在原頁面中篩選出要展示的內容，以此為出發點來設計首頁

- 這個頁面共計有 **4** 個 section

### header & navbar

- 原本首頁的 `Main Menu` 太多項目，我僅選出了三個較重要的項目並使用 `navbar-nav` 做呈現。
  其餘內容中再選出兩個頁面做額外連結頁面的設計。最後，我將其他剩下的項目則連回原本網站所連回的網址。

- 除了使用 `navbar-nav` 外，其他的項目則隱藏在 `offcanvas` 作為左側選單使用。
  當滑鼠移動到選單上的項目時(`:hover`)，我讓它會有突出的動畫效果，讓使用者知道自己選擇了哪個項目。

### section - home

- 在 `home` 區塊，我選用了來自 [Unsplash](https://unsplash.com/photos/3vVzdb8KKIw) 的照片當作背景圖。同時還將該單位的 logo 和名稱顯示在頁面上，並使其佔據整個版面的 80% 左右。當視窗寬度小於 768px 時，我會將中文名稱隱藏。我使用 [AOS](https://michalsnik.github.io/aos/) JavaScript 函式庫，讓 logo 和名稱有漂浮進入的動畫效果。

### section - about

- 這個區塊的內容參考了原網站的同名區域。我一開始將標題和標語顯示在區塊上方部分，接著使用 Grid Layout 將簡介內容和使用 `Stable Diffusion 1.51` 產生的圖片做成兩欄的內容。在螢幕小於 768px 時，我會讓它變成一欄的內容。

### section - ancmt(Announcement)

- 這個區塊的內容參考了原網站的同名區域。我將標題顯示在區塊上方部分，然後下方使用 `list group` 元件做乘載，但是我還需要透過調整類別來實現想要呈現的效果。為了避免文字內容太長，我為每個 `list-group-item` 都添加 `text-truncate` 類別，使其超出容器時被截斷。

- 我也添加了 `Read more ...` 項目，讓這個區塊看起來有動態內容。點選它後會跳轉到原網站原本的公告頁面。

### section - rt(Research Topics)

- 這個區塊的內容參考了原網站的同名區域。我將標題和標語顯示在區塊上方部分，然後使用 `card` 元件和 Grid Layout 的結合，將四個項目和介紹內容放在區塊中呈現。為了避免文字內容太長，我對每個 card-text 做出針對性的 CSS 修改，使其內容超過三行後便會被截斷。我也添加了 `Read more ...` 按鈕，使使用者可以跳轉到原網站的介紹頁面。

### footer

- 在頁尾的部分，我將原網站首頁的 `指導教授` 和 `聯絡資料` 區塊融合到頁尾的內容中。這個區塊的高度至少會有 175px。根據期末專案的要求，我在頁尾的最右側放上設計者的班級學號姓名。

## equipment

- 這個頁面可以透過 `offcanvas` 選單上的 **實驗室設備** 前往。

- 這個頁面是參考原網站的 [Equipment/實驗室設備](https://resl.csie.nptu.edu.tw/joomla3/index.php/equipment) 頁面所設計的。我們將原先使用條列式呈現的內容，改用 `card` 元件配合 Unsplash 上的數張圖片一起展示。我將 `card-img-top` 經過 CSS 的調整後縮到等寬且超出部分被裁切。圖片容器的高度為整個 `card` 元件的 75%。

- 我在內容的上方添加了 `breadcrumb` 來指示現在使用者在網站的哪個位置。

- 這個頁面共計有 **1** 個 section

## special-topics-course

- 這個頁面可以透過 `offcanvas` 選單上的 **專題課** 前往。

- 這個頁面是參考自原網站的 [Special Topics Course/專題課程](https://resl.csie.nptu.edu.tw/joomla3/index.php/special-topics-course) 頁面所設計的。我只取用了 `專題生的自我修練 - 要加入RESL應有的認知與體認` 區塊的內容做呈現，將其所闡述的內容用 1.25em 和 1.5 倍行高呈現出來。

- 我在內容的上方添加了 `breadcrumb` 來指示現在使用者在網站的哪個位置。

- 這個頁面共計有 **1** 個 section
