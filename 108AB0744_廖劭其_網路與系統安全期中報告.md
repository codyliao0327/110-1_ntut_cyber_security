班級：資財三乙  
學號：108AB0744  
姓名：廖劭其  

# BIGNOX NOXPLAYER: ANDROID EMULATOR FOR PCS AND MACS

#### BigNox NoxPlayer介紹
NoxPlayer是一款Android模擬器軟體，安裝在Windows或macOS上，就能在電腦上執行Android遊戲。它支援20種語言，號稱在全球150個國家擁有1.5億名用戶。NoxPlayer母公司BigNox的總部則位於香港，也使得NoxPlayer在亞洲地區特別熱門。

#### 供應鏈攻擊事件流程
> 2020.9 駭客透過NoxPlayer更新機制，於用戶執行更新時植入惡意程式
> 2021.1.25 ESET發現此一供應鏈攻擊行動時，旋即通知了BigNox
> 2021.2.4 ESET公告BigNox已推送最新版檔案至更新伺服器

#### 供應鏈攻擊事件內容
駭客滲透了NoxPlayer的更新機制，且儘管NoxPlayer擁有廣大的用戶，卻只有5名使用者收到了惡意更新，而這5名受害者分別位於臺灣、香港與斯里蘭卡。此外，駭客在這些惡意更新中所植入的惡意程式並非用來獲利，而是專注於監控。

#### 供應鏈攻擊者
ESET研究人員認為Gelsemium是針對BigNox的供應鏈攻擊的幕後黑手。對於Gelsemium擅長的手法而言，ESET認為是藉由微軟Office的漏洞與釣魚郵件，來散布用來攻擊的惡意軟體，並且利用Exchange伺服器的RCE漏洞，來進行水坑式攻擊。

#### BigNox採取防護措施
1. 僅透過HTTPS提供更新軟體，降低域名劫持(Domain Hijacking)與中間人攻擊之風險。
2. 透過MD5雜湊值與檔案簽名檢查進行完整性驗證。
3. 採取其他措施，如加密機敏資訊等，避免用戶個人機敏資訊外洩。