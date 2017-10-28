# 共享 data 平台

#### 在資料爆炸的年代，我們卻沒有容易取得 data 的管道，因此提供一個共享 data 的平台，一個人爬蟲力量有限，合作爬蟲力量無限。各位可以在這上面，update 自己爬到的 data ，download 其他人分享的 data。<br>
平台網址：http://114.34.138.146/phpmyadmin/ <br>
每天約新增 15 萬筆 data。最新 data 在 ptt_data1.0 中，目前超過 400 萬筆。<br>
本人 10/16 要去當兵了(一年)T.T。該平台會繼續開著，爬蟲方面設定排程繼續進行。issues 方面，會盡可能利用假日回應。<br>

<!--資料科學家是當今最紅的職業，根據 CareerCast.com 網站，2016 best job is data scientist。
問題是，要如何成為資料科學家？資料取得不易，沒資料幾乎不可能成為資料科學家，，，，，，，，， -->

## UPDATE
#### 2017/10/11
1. py_connect_sql_example.py 中，將 origin_data 改為 ptt_data1.0，更改資料庫，origin_data 將不再更新，預計 10 天後，ptt_data1.0 資料量將超越 origin_data。<br>
#### 2017/10/10
1. 提高爬蟲效率，預計一天新增 15 萬筆 data ( 過去一天 4 萬筆 )。<br>
#### 2017/10/9 
1. 由於 origin_data 中，資料不夠完善，有小缺失，因此我重新爬取 data，放在 ptt_data1.0 中，並加入 guest 讀取權限。<br>
   另外 origin_data 依然會開放，但不進行更新，各位可以先進行 text mining，之後再更改資料庫即可，如有不便請多多包涵。
2. 推文內容部分，如果有興趣，可以由 data 欄位 origin_article 進行 data clean ，額外提取。<br>
   未來我也會進行 data clean，並公開 code 與 data，但是可能需要一段時間，有興趣的朋友可自行嘗試。


[history_Update](https://github.com/f496328mm/Crawler_and_Share/blob/master/history_Update.md)<br><br><br><br><br>

<!--
## 2017/10/3 
公開密碼，權限為：可自由取得 SQL 中的 data，該程式中已將格式轉為 dataframe ，利於分析。-->


## 附件
1. py_connect_sql_example.py，可自由取得 SQL 中的 data，該程式中已將格式轉為 dataframe ，利於分析。
2. upload_clean_data.py，可上傳 data 的帳號，提供各位進行 data clean 後，一個上傳/分享的管道，這樣就不需要每個人都進行 data clean，合作的概念。程式中提供一個 建立 data file 和上傳 data 的範例。
3. sql.py 提供 python 連接 MYSQL 教學，有中英註解，如果不清楚再 email 詢問我。
4. craw_ptt.py 提供爬取 PTT 文章，並且上傳到 MYSQL code，附上中文註解，不過 code 中並沒有設定密碼，會有 ERROR，帳號密碼請參考 py_connect_sql_example.py。
<br><br>


由於這是我個人架設的平台，資源有限，請不要進行惡意攻擊。另外同一時間使用人數過多，速度上可能會降低，請多包涵。<br><br>
e-mail : samlin266118@gmail.com <br>
連接網址為 : http://114.34.138.146/phpmyadmin/ <br>
user : guest <br>
password : 123 <br>
### PS: 在爬取文章部分，可能出現小錯誤，因此其中一個欄位 origin_article ，提供最原始的 data，如果有錯誤可額外進行提取，基本上99%的資料都是正確的。
<br><br><br><br><br>
歡迎有同樣熱情的朋友協助我，共同合作，由於我是資料分析( 數學系 )出身，並沒有 PHP、SQL 等專業知識，目前只是個雛形，沒有前端，後端部分也只是剛開始，因此需要這方面的夥伴，歡迎 email 討論。未來朝 open 的方向進行，目前資源不足，請多包涵。
<br><br>
<!--匯出請選擇 "test" 樣板，將會匯出所有 data ， csv 檔， big 5 編碼 -->


## 目前超過 400 萬筆 data ，持續更新中<br><br>

|SQL name|DATA 筆數|類別|
|--------|----|-|
|AdvEduUK|10||
|AllTogether|70,000||
|Aquarius|10||
|Aries|10||
|Aviation|10||
|BabyMother|123,000||
|BabyProducts|10||
|baking|17,000||
|Baseball|10||
|biker|10||
|Boy_Girl|68,000||
|Broken_heart|23,300|情感分析|
|BuyTogether|76,500||
|Cancer|10||
|Capricornus|18||
|car|76,188||
|CarShop|5,000||
|CATCH|19||
|cookclub|69,303||
|couple|13,800||
|creditcard|49,000||
|DC_SALE|4||
|Diary|20||
|DistantLove|20||
|Dreamland|20||
|EngTalk|9,700||
|e_shopping|70,000|購物買賣|
|Finance|19,000||
|Food|124,832||
|Gossiping|507,854|八卦版|
|happy|23,727|情感分析|
|HardwareSale|79,301|購物買賣|
|Hate|74,164|情感分析|
|HomeTeach|19|工作相關資訊|
|home_sale|21,565|購物買賣|
|Japan_Travel|34,463||
|job|8,827|工作相關資訊|
|JOB_Hunting|6,600|工作相關資訊|
|Lifeismoney|20|購物買賣|
|Lonely|20,359|情感分析|
|love|20,000|情感分析|
|Lucky|18,000|情感分析|
|MacShop|20|購物買賣|
|Marginalman|20|情感分析|
|MenTalk|96,943|聊天機器人|
|MobileComm|20|購物買賣|
|movie|18||
|Oversea_Job|713|工作相關資訊|
|part_time|20|工作相關資訊|
|PC_Shopping|66,728|購物買賣|
|prozac|20|情感分析|
|Sad|26,017|情感分析|
|SayLove|13,000|情感分析|
|Self_Healin|13,000||
|Soft_Job|20|工作相關資訊|
|SorryPub|18,227|情感分析|
|Stock|20||
|TaiwanJobs|20|工作相關資訊|
|talk|62,078|聊天機器人|
|Tech_Job|51,368|工作相關資訊|
|toberich|23,536||
|WomenTalk|85,307|聊天機器人|







