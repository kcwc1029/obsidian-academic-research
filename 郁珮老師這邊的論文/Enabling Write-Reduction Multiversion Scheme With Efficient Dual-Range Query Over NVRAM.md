---
APA: Wang, I. J., Liang, Y. P., Chen, T. Y., Chang, Y. H., Chen, B. J., Wei, H. W., & Shih, W. K. (2021). Enabling write-reduction multiversion scheme with efficient dual-range query over NVRAM. IEEE Transactions on Very Large Scale Integration (VLSI) Systems, 29(6), 1244-1256.
tags:
  - write_reduction減少寫入
  - nonvolatile_memory非揮發性記憶體
  - multiversion_indexing_scheme多版本索引方案
  - Efficient_query高效查詢
---
## 研究背景與知識點
### 一 版本森林（Version Forest）**：
- 一種用於管理多版本數據的數據結構，每個節點表示一個數據版本。
- 每個事務提交時，都會生成一個新的版本，並將其插入到版本森林中。每個節點包含了該版本的數據和元數據（例如時間戳）。
- 版本森林通常使用索引來加速版本的查詢和檢索，以便快速地找到特定版本的數據。
### 二 多版本樹（Multiversion Tree）
- 類似於版本森林的數據結構，用於管理多版本數據。
- 不同於版本森林，多版本樹通常將多個版本的數據存儲在同一個節點中，並使用版本號或其他標識來區分不同的版本。
- 多版本樹也常常使用索引來加速版本的查詢和檢索，以便快速地找到特定版本的數據。

### 三 多版本資料庫系統
多版本資料庫系統已成為分析和挖掘的最關鍵的數據管理工具。
原因：數據可以通過多版本索引方案進行查詢。
優勢：提高了索引方案的查詢性、提高多版本資料庫的性能。
==multiversion database systems have become the most critical data management tool for analyzing and mining. As all data in a multiver- sion database will be indexed by a multiversion indexing scheme, boosting the indexing scheme’s query performance will also increase the multiversion database’s performance.==

### 四 MVBT（多版本B樹） 
MVBT（多版本B樹）是一種基於B樹結構開發的多版本索引方案。
核心：允許在同一數據集中存儲多個版本的數據，將數據按照版本號進行組織。
目的：查詢時可以快速定位到特定版本的數據。提高多個版本的數據集中的查詢性能。
優點：提供多版本數據集上最優的查詢性能。
優點：有效地管理多個版本的數據，使其適用於需要跟蹤歷史更改的應用程序。
應用領域：數據庫系統、時間序列數據

### 五 非易失性隨機存取記憶體 （NVRAM）
非易失性隨機存取記憶體 （NVRAM） 被認為是未來十年計算機系統的記憶體/存儲技術，因此在設計 NVRAM 友好的多版本索引方案時應考慮 NVRAM 功能。

＄未解決的問題：
- 在開發多版本索引方案時沒有考慮NVRAM技術的非對稱讀寫成本。由於多版本索引方案會重寫重複資訊以實現高效的多版本化數據查詢，因此會向 NVRAM 空間生成大量寫入流量。
- 所有多版本索引方案都不能同時提供高效的鍵和版本範圍查詢。其不僅在基於NVRAM的系統上，而且在一般系統架構上。



## 研究目的
＄多版本索引方案在使用非易失性隨機存取記憶體(NVRAM)時存在一些缺點：
- 寫入流量大（heavy write traffic）
- 鍵或版本範圍查詢性能較弱（weak-key or version-range-query performance）
==However, modern multiversion indexing schemes have significant drawbacks (e.g., heavy write traffic and weak-key or version-range-query performance)==
儘管存在這些缺點,但從NVRAM具有高存儲單元密度和零靜態功耗的優點來看,NVRAM仍被視為是未來替代動態隨機存取記憶體(DRAM)的一個有前景的候選技術。==with the considerations of high memory cell density and zero-static power consumption, NVRAM has been regarded as a promising candidate to substitute for dynamic random access memory (DRAM) in future computer systems==



＄目前沒有多版本索引方案可以同時提供高效的版本和鍵範圍查詢。

對於某些應用程式（例如，網路物理系統、監控和人群計算[15]）會定期從終端設備收集數據，收集的數據將在存儲系統中作為不同版本進行管理。這種數據管理將成為資料庫系統設計的一個重大問題。⭢多版本資料庫系統採用多版本索引方案，其目的是有效地維護多版本資料庫中版本數據的索引。==multiversion database systems employ a multiversion indexing scheme, whose purpose is to effectively maintain the index of version data in a multiversion database.

- 關於MVBT的部分：Backer等[2]提出了一種基於B樹結構開發的多版本B樹，即MVBT，提供了幾乎最優的查詢性能。NVRAM在過去幾年中被視為下一代記憶體/存儲技術，因此在其設計中並未研究非對稱讀/寫成本。==Backer et al. [2] proposed a mul- +tiversion B -tree, namely MVBT, that is developed based on +1A computer architecture includes NVRAM to be its memory or storage. the B -tree structure. Although MVBT offers asymptotically optimal query performance, the asymmetric read/write cost has not been studied in its design since NVRAM is regarded as a next-generation memory/storage technology in the past few years.==
> [!QUESTION] 老師我有問題
> 您在這篇有提到先提到「Backer等[2]提出了一種基於B樹結構開發的多版本B樹，即MVBT，並提供最優的查詢性能。」接著論述「NVRAM在過去幾年中被視為下一代記憶體/存儲技術，因此在其設計中並未研究非對稱讀/寫成本。」
> 
> 想訊問這兩個之間的關係？
- SEMI方案：Kuan等[4]，[5]針對NVRAM的空間利用率和版本範圍查詢性能提出一種節省空間的多版本索引方案SEMI。但SEMI是針對嵌入式多版本索引方案，並不能應用於具有許多數據鍵的資料庫系統。==Kuan et al. [4], [5] presented a space-efficient multiversion indexing scheme, called SEMI, that aimed to improve the space utilization and the version-range-query performance of MVBT scheme on NVRAM storage. Nevertheless, the SEMI is targeted on an embedded multiversion indexing scheme, so it cannot be applied to the database system with many data keys. In other words, the SEMI cannot yield efficient key-range-query performance.==
## 研究方法
- 提出一種具有高效雙範圍查詢的減寫多版本索引方案，即Duery。通過開發和集成多版本樹結構和版本林，在多版本索引方案中支援高效的雙範圍查詢。當使用者想要執行完全匹配查詢和鍵範圍查詢時，Duery 會將使用者請求分派給多版本樹結構，因為多版本樹可以提供高鍵範圍查詢性能。==Duery empowers efficient dual- range queries in a multiversion indexing scheme by developing and integrating a multiversion tree structure and version forest. While users want to perform an exact-match query and a key-range query, Duery will dispatch the user request to the multiversion tree structure because the multiversion tree can provide high key-range-query performance.==
- 不同的是，版本林將處理版本範圍查詢，因為它將屬於同一索引的版本數據聚合在一起。考慮到非對稱讀寫成本，Duery帶來了基於指標的拆分機制，以減少NVRAM的寫入流量，從而降低寫入延遲和能耗。==Differently, the version forest will deal with a version-range query because it aggregates the version data belonging to the same index together. With the consideration of the asymmetric read/write cost, Duery brings a pointer-based split mechanism to reduce the amount of write traffic to NVRAM so as to decrease the write latency and energy consumption. According to our experimental results, Duery can effectively reduce the amount of write traffic to NVRAM storage compared with a naive hybrid indexing scheme.==

## 研究結果
- 我們的方案有效減少了多版本索引方案產生的寫入 NVRAM 的流量。它通過整合提議的版本森林和多版本樹，提供了高效的雙範圍查詢。==our scheme effectively reduces the amount of write traffic generated by the multiversion indexing scheme to NVRAM. It offers efficient dual-range queries by consolidating the proposed version forest and the multiversion tree==

＄成就：
- 本文首先確定了基於 NVRAM 的計算機系統上的多版本資料庫索引方案中的 dualrange（即鍵和版本範圍）查詢效率問題。
- 在基於NVRAM的多版本資料庫索引方案設計中，提出了雙範圍查詢（簡稱Duery）綜合考慮了雙範圍查詢效率和寫入減少。
- 提出的Duery不僅減少了11%的NVRAM存儲的寫入流量，而且將密鑰和版本範圍查詢效率提高了44%。










