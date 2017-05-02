# Linux

目錄相關指令
> ls : 目錄下的檔案清單
- -l : 檔案的詳細資訊，如 : ls -l。有七項資訊，分別為權限、連結數、擁有者、群組、檔案大小、更動時間、檔案名稱
    - 權限 : x-xxx-xxx-xxx
 (1)d 
    \- : 檔案 
    d : 目錄
    l : 連結
     (2)r w x (擁有者權限)  
     (3)r w x (群組權限)
     (4)r w x (其他人權限)
- -a : 顯示隱藏檔案，如 : ls -a -l (-a -l 可以寫成 -al)。
>. (目錄) : 代表目前所在的目錄

>.\. (目錄) : 代表上層目錄

>cd : 切換目錄。如 : cd ../

>cp : 複製檔案

>mv : 搬移檔案

>rm : 刪除檔案，會再詢問一次是否要刪除此檔案

>-f : 不用再詢問，如 : rm -rf

>man : 查詢指令的操作說明書

>cat : 查看一個檔案的內容，如 : cat /var/log/message，愈加上行號就在後面輸入 -n

> more : 輸出檔案內容分頁顯示。

>touch : 產生空白檔案，如 : touch file1 file2

>mkdir : 建立目錄

>rmdir : 刪除目錄(只能刪除掉空的目錄)，想刪除整個目錄就加上 -r

>pwd : 目前在哪個目錄下

> df : 查看系統各個分割區空間使用情形，後面加 -h 是指顯示單位以KB、MB、GB來表示

> du : 查看磁碟空間使用情形的方法，加 -sh 為顯示總空間 

> echo 'string' > file : 例如，echo 'new data' > file，代表 file這個的內容文字訊息為 new data ，利用 cat 可以叫出文字內容，如 cat file

> grep : 文字篩選，grep <string> ，搜尋含有<string>的字串

> ln -s : 建立連結，ln -s 目標對象 連結名稱。如 ln -s data slink，就是把slink指向data的內容。

> \> : 覆蓋檔案。ex : a > b 

> \>> : 新增資料於檔案尾端。 ex : a >> b

掛載 --> mount -t 檔案類型 設備檔案 掛載至系統目錄

# vim
編輯模式、一般模式、命令模式
>:e 檔案 : 在 vi 中開啟檔案

>:q! : 離開 vi (不儲存更動)

>:w : 儲存內容

>:wq : 儲存內容並離開

>i 或 o 或 a : 進入編輯模式

>[ESC鍵] : 從編輯模式、命令模式退回一般模式

>h : 左移

>j : 下移

>k : 上移

>l : 右移

>w : 移到下一個英文字

>yy : 複製游標所在該行

>p : 貼在下一行

>dd : 刪除游標所在該行

>u : 復原上一次更動

>. : 重複上一個動作

>gg : 移到第一行

>G : 移到最後一行

>:set nu : 顯示行號
