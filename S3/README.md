# Amazon S3 : 檔案儲存服務 (可儲存 文件 文檔 圖片 影片)

(Tutorial 17-23)

## 1.S3 基本建立 :

A.S3 bucket(儲存桶) 建立 :

- Amazon 的資料類型儲存在 bucket 當中,因此首先, 要先在 aws 中建立 bucket.

B.Load 資料進入 AWS : - 將檔案上傳到 S3(ex: xxx.png)

C.可檢查上傳檔案的資訊 : - 如 : aws region(ex:US west)/ 檔案大小(ex:5kb)/ type(ex:png)/URL - (!)重點 : 每個上傳的檔案(物件)都有自己的 URL, 因此可以從 router 中找到它在哪個 bucket 的實體位置,

D.可以設定從瀏覽器中輸入 ROUTER 並瀏覽資料 - Bucket Policy Setting(class19) : 允許同一個檔案路徑下公開藉由 router 存取所有資料

## 2.處理 Permission (AccessDenied)問題 :

    - a.Create bucket -> Block all public access(關掉)
    - b.Make public :
      - Actions -> Make public
    - c.從瀏覽器上測試能否看到 [檔案/物件] (ex:xxx.png)

## 3.S3 versioning : 使用 versioning 幫你版本控制

更改 bucket version : 去 Create Bucket -> Bucket versioning -> bucket -> disable 改成 Enable -> save

## 4.Static webite hosting :

- a.Properties -> Static Webite hosting -> disable 改成 Enable
- b.輸入 index document : 成為網站瀏覽器進入的 Page(ex:index.html)

## 5.Practical(實作) : Upload folder and Image(Ongoing...)

- show Wehelp 2 project and Face-Recognition image
