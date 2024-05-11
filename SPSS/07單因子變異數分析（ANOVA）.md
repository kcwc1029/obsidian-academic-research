## 適用於
自變數Ｘ：名目尺度
依變數Ｙ：計量尺度
- 自變數只有兩個（性別），使用t檢定
- 自變數超過兩個（性別），使用變異數分析


## 定義
- 檢定因子各水準的母體平均數，是否相等的統計方式。
- ANOVA是用來檢定多組平均數是否相等的問題，而非在檢定變異數相等的問題。

## 範例
- 大二、大三、大四學生的學習滿意度是否一樣？
- 不同職業的消費者，對否家連鎖咖啡廳的忠誠度是否有顯著差異？
- 不同生產線的產品不良率是否相同？

## 變異數概念分析圖

![upgit_20240507_1715069949.png](https://raw.githubusercontent.com/kcwc1029/obsidian-upgit-image/main/2024/05/upgit_20240507_1715069949.png)


## 為什麼要用ANOVA，而不是t檢定

若使用t檢定比較，則得一一比對。假設有三個因子，則要做3!=6次比較。
若以信心水準0.95來說，做六次等於(0.95)^6 = 0.735，信心水準會降低。
若使用ANOVA，則可以一次搞定。

## ANOVA基本假設

- 每個因子母體均為常態分配。
- 每個因子母體變異數想等。
- 抽自各母體的各組隨機樣本互為獨立。  

## ANOVA計算邏輯

總變異（SST） = 組間變異（SSB） + 組內變異（SSE）
總變異（SST）= 平方和（所有觀測值 - 總平均）

![upgit_20240507_1715071263.png](https://raw.githubusercontent.com/kcwc1029/obsidian-upgit-image/main/2024/05/upgit_20240507_1715071263.png)

![upgit_20240507_1715071401.png](https://raw.githubusercontent.com/kcwc1029/obsidian-upgit-image/main/2024/05/upgit_20240507_1715071401.png)




## 事後比較方法
- Scheffé 檢定則是一個保守且通用的選擇，但在顯著性檢定上較為嚴格。
- 如果你的資料符合同質性假設且變異較均勻，可以考慮使用 Duncan 檢定
- 如果資料不符合同質性假設，則可以考慮使用 Tamhane 檢定。

## 作法
範例檔：/SPSS/Employee data.sav
【分析】⭢【比較平均數】⭢【單因數變異數分析】

![upgit_20240507_1715072688.png](https://raw.githubusercontent.com/kcwc1029/obsidian-upgit-image/main/2024/05/upgit_20240507_1715072688.png)

## 分析
- 描述F值（ANOVA就是看F值得）
- 查看各個單因子的描述統計（平均數、標準差）
- 查看變異數的同質性測試：直接看顯著性
- 查看變異數分析：直接看顯著性
- 針對有顯著的，去看多重比較（T2法）

![upgit_20240507_1715073346.png](https://raw.githubusercontent.com/kcwc1029/obsidian-upgit-image/main/2024/05/upgit_20240507_1715073346.png)

![upgit_20240507_1715073692.png](https://raw.githubusercontent.com/kcwc1029/obsidian-upgit-image/main/2024/05/upgit_20240507_1715073692.png)


 