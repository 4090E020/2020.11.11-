***問答

```
###解釋 communication protocol(簡稱協定 protocol)
1.通信協定（英語：Communications Protocol，也稱傳輸協定）在電信領域中指的是，在任何物理媒介中允許兩個或多個在傳輸系統中的終端之間傳播資訊的系統標準，也是指電腦通信或網路裝置的共同語言。
```
```
###Why Layering? (為何要分層 ?)
2.分層的目的是利用層次結構可以把開放系統的資訊交換問題分解到一系列容易控制的軟硬體模組－層中，而各層可以根據需要獨立進行修改或擴充功能，同時，有利於個不同製造廠家的裝置互連，也有利於大家學習、理解資料通訊網路。
```
```
###列出 OSI Model 與 TCP/IP protocol對應圖
3.應用層(Application layer)-------------->       應用層   
  展示層(Presentation layer)------------->
  會議層(Session layer)------------------>  Application layer
  
  傳輸層(Transport layer)----------------> 傳輸層Transport layer
  
  網路層(Network layer)------------------> 網路層 Internet layer
  
  資料連結層(Data link layer)------------> 連結層
  實體層(Physical layer)-----------------> Link layer
  ```
  ```
  應用層（Application Layer）提供為應用軟體而設計的介面，以設定與另一應用軟體之間的通訊
  表達層（Presentation Layer）把數據轉換為能與接收者的系統格式相容並適合傳輸的格式。
  會議層（Session Layer）負責在數據傳輸中設定和維護電腦網路中兩台電腦之間的通訊連接。
  傳輸層（Transport Layer）把傳輸表頭（TH）加至數據以形成數據包。傳輸表頭包含了所使用的協定等傳送資訊。
  網路層（Network Layer）決定數據的路徑選擇和轉寄，將網路表頭（NH）加至數據包，以形成封包。網路表頭包含了網路資料。
  資料連結層（Data Link Layer）負責網路尋址、錯誤偵測和改錯。
  實體層（Physical Layer）在局部區域網路上傳送資料框（Data Frame），它負責管理電腦通訊裝置和網路媒體之間的互通。
  ```
  ```
 簡述 下列協定的功能 與特色並說明它們 運作在 TCP/IP的哪一層?
 4.題目:HTTP
(A)英文全名
HyperText Transfer Protocol                                             
(B)運作在那一層?
應用層（application layer）                                            
(C)主要功能
提供一種發布和接收HTML頁面的方法
```
```
題目:HTTPS
(A)英文全名
HyperText Transfer Protocol Secure                                       
(B)運作在那一層?
應用層（application layer）
(C)主要功能
主要作用是在不安全的網路上建立一個安全信道，並可在使用適當的加密套件和伺服器憑證可被驗證且可被信任時，對竊聽和中間人攻擊提供合理的防護。
```
```
題目:TELNET
(A)英文全名
(B)運作在那一層?
應用層（application layer）
(C)主要功能
一種應用層協定，使用於網際網路及區域網中，使用虛擬終端機的形式，提供雙向、以文字字串為主的命令列介面互動功能
```
```
題目:SSH
(A)英文全名
Secure Shell
(B)運作在那一層?
應用層（application layer）
(C)主要功能
一種加密的網路傳輸協定，可在不安全的網路中為網路服務提供安全的傳輸環境。
```
```
題目:DNS
(A)英文全名
Domain Name System
(B)運作在那一層?
應用層（application layer）
(C)主要功能
是網際網路的一項服務。它作為將域名和IP位址相互對映的一個分散式資料庫，能夠使人更方便地存取網際網路。
```
```
題目:IP
(A)英文全名
Internet Protocol
(B)運作在那一層?
網路層（network layer）
(C)主要功能
任務僅僅是根據源主機和目的主機的位址來傳送資料
```
```
題目:ICMP
(A)英文全名
Internet Control Message Protocol
(B)運作在那一層?
網路層（network layer）
(C)主要功能
它用於網際網路協定（IP）中傳送控制訊息，提供可能發生在通訊環境中的各種問題回饋。
```
```
5.TCP VS UDP

TCP
(1)英文全名為Transmission Control Protocol
(2)reliable(可靠)
(3)通常在每個TCP報文段中都有一對序號和確認號。TCP報文傳送者稱自己的位元組流的編號為序號（sequence number），稱接收到對方的位元組流編號為確認號。TCP報文的接收者為了確保可靠性，在接收到一定數量的連續位元組流後才傳送確認。


(4)Client -----syn---->  Server
        
       syn-ack
       
   Client  -----ack--->  Server
```
```
   UDP
   (1)英文全名為User Datagram Protocol
   (2)unreliable
```
```
###簡述下列網路設備  主要功能 與 特色 及 運作在 OSI哪一層
6.題目:HUB
(A)運作在OSI那一層?
實體層
(B)主要功能
是指將多條乙太網路雙絞線或光纖集合連接在同一段物理媒介下的裝置
```
```
題目:Repeater
(A)運作在OSI那一層?
實體層
(B)主要功能
一個將輸入訊號增強放大的類比裝置，而不考慮輸入訊號種類
```
```
題目:Switch
(A)運作在OSI那一層?
資料連結層
(B)主要功能
是一種網路硬體，通過報文交換接收和轉發資料到目標裝置，它能夠在電腦網路上連接不同的裝置
```
```
題目: Bridge
(A)運作在OSI那一層?
資料連結層
(B)主要功能
一種網路裝置，負責網路橋接
```
```
題目:Router
(A)運作在OSI那一層?
網路層
(B)主要功能
是一種電訊網路裝置，提供路由與轉送兩種重要機制，可以決定封包從來源端到目的端所經過的路由路徑
```
```
題目:L3 Switch
(A)運作在OSI那一層?
資料連結層
(B)主要功能
可以對 VLAN 做更有效的管制，讓廣播封包不會無限制的傳送
```
```
題目:Proxy 
(A)運作在OSI那一層?
應用層
(B)主要功能
是一種特殊的網路服務，允許一個（一般為客戶端）通過這個服務與另一個網路終端（一般為伺服器）進行非直接的連接
```
```
###簡述下列 簡述下列 address(位址 )的意義 與定義 在 OSI Model哪一層
7.PORT address
(1)在電腦網路中是一種經由軟體建立的服務，在一個電腦作業系統中扮演通訊的端點（endpoint）。每個通訊埠都會與主機的IP位址及通訊協定關聯。
(2)位於傳輸層
```
```
IP address
(1)是網際協定（Internet Protocol）中用於標識傳送或接收資料報的裝置的一串數字。
(2)網路層
```
```
MAC address
(1)它是一個用來確認網路裝置位置的位址
(2)資料鏈結層
```

  





















































