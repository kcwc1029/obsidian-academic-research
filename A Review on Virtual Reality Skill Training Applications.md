---
tags:
  - Virtual_reality虛擬實境
  - simulation_training模擬訓練
  - content_creation內容創作
  - personalization個人化
APA: Xie, B., Liu, H., Alghofaili, R., Zhang, Y., Jiang, Y., Lobo, F. D., ... & Yu, L. F. (2021). A review on virtual reality skill training applications. Frontiers in Virtual Reality, 2, 645153.
file: "[[A Review on Virtual Reality Skill Training Applications.pdf]]"
重要程度: ✭✭✭✭✭
---
==研究背景==

- 2020年IEEE虛擬現實大會收到創紀錄的論文投稿數量,比前一年(2019年)增長約10%。
	- 根據Merriam Webster辭典[1]對於訓練(train)的定義：
	1. 訓練被定義為培訓者的行為、過程或方法。
	2. 培訓者所獲得的技能、知識或經驗，或者是受過培訓的狀態。

// 討論了虛擬現實（VR）技術在培訓領域的應用和優勢：
根據不同領域，VR可以大幅降低培訓成本，同時增加培訓場景數量。由於VR培訓場景主要涉及計算機生成的3D圖形，VR開發人員可以輕松從現有3D資產創建各種場景，這些場景可反覆用於培訓不同人員。通過互聯網交付，使用場景也更加方便。盡管VR培訓不能保證降低成本,但這些系統為受訓人員帶來的優勢可能會證明投資成本是合理的。

// 強調了VR技術提供的安全、隱私和仿真的優勢，以及它對培訓效果的潛在提升。
VR技術允許受訓者在私人空間中學習。例如：工人可以在家里使用VR學習使用設備或遵循安全程序。這對於那些在真實培訓過程中由於觀察者在場而感到不自在的受訓者尤其重要。然而還是有些培訓情況需要在師長在場的情況下進行，因為他們需要及時反饋受訓者的表現,，警示他們可能存在的問題，包括表現出的負面趨勢。此外，VR培訓提供了一個安全的環境，最大限度地減少了危險情況的暴露[例如火災、爆炸和自然災害]。[2]


// VR培訓應用程序已經開發用於各種領域：
Xie(2006)[3]探討了不同培訓場景的概括描述。他們將虛擬現實安全培訓系統的創建過程與基於場景的設計方法相結合，構建了創建VR培訓體驗的通用框架。
Martin(2009)[4]、Martin和Hughes(2010)[5]開發了用於自動場景生成的軟件，旨在探索場景生成方法的概念設計。
Lin等人(2002)[6]提出了基於VR的培訓系統的架構，以及虛擬培訓任務規劃和一些面向任務的培訓場景模型的介紹，VR培訓的創建流程可粗略地分為三個階段：任務分析，培訓場景草擬和實施。

// 強調任務分析是設計任何培訓目標的基礎，並提到了分層任務分析（HTA）和認知任務分析（CTA）這兩種新方法。

早期的任務分析方法主要關注描述和表示簡單的身體行為和決策，如Gilbreth和Carey提出的therbligs [7]。隨著時間推移,任務分析方法有所改進,能夠描述更複雜的認知任務,如搜索和發現[8]。分層任務分析(HTA)和認知任務分析(CTA)是現代任務分析中最著名和使用最廣泛的方法。HTA關注描述由不同單元組成的「目標」，而CTA則側重於處理意外情況[9]。

==研究背景 VR軟體==

Lovreglio 等人（2020 年）認為VR軟體使用資源使用簡單，易於製作，但受訓者缺乏身臨其境的體驗，因此，培訓結果無法與VR培訓相提並論[10]。

本文針對VR軟體總結兩點
// VR軟體的歷史：
1994年首次推出的虛擬實境建模語言（VRML）旨在開發不依賴耳機的“虛擬世界”。在VRML淡出后，各種其他程式設計語言和工具從它停止的地方開始。其中，我們發現了 2016 年停產的 3DMLW、COLLADA、O3D 和 X3D。如今，遊戲引擎是虛擬實境應用最流行的開發工具之一，具有多個軟體包和軟體開發套件，支援主流VR設備。例如，Unity 3D（Linowes，2015）[11]和虛幻引擎（Whiting和Donaldson，2014） [12] 是受歡迎的選擇。它們都集成了 API，VR 開發人員在安裝相應的 SDK 后可以輕鬆使用。

3D 建模在創建虛擬培訓環境方面也很重要。Unity和Unreal的資源商店中有大量的資源，如3D模型、3D場景和示例專案，使那些可能沒有任何3D建模知識或技能的人更容易創建內容。此外，如果開發人員想要自定義其 3D 內容，他們可以使用高級 3D 建模軟體（如 3ds Max、Maya 和 Blender）來構建和修改 3D 模型。另一方面，虛擬實境週邊網路 （VRPN） （Taylor et al.， 2001）[13] 提供對 VR 系統中使用的各種跟蹤、按鈕、操縱桿、聲音和其他設備的本地或網路訪問。

// VR軟體 - 程式生成技術
程式生成技術也廣泛用於創建虛擬內容，例如虛擬環境、3D 模型和遊戲關卡設計，
其通常是根據定任務創建，針對特定培訓目標為實現目的。例如創建地形[14]、城市[15]和房間佈局[16]等。


// 表格：探索基於場景描述的虛擬現實（VR）相關研究（本文作者從Xie et al. (2021)進行修改）

| 論文名稱                                                                                         | 引用（APA）                                                                                                                                                                                                                                                     | 內容                                                                                                                |
| -------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| A declarative approach to procedural modeling of virtual worlds                              | Smelik, R. M., Tutenel, T., de Kraker, K. J., & Bidarra, R. (2011). A declarative approach to procedural modeling of virtual worlds. _Computers & Graphics_, _35_(2), 352-363.                                                                              | 聲明式建模方法提出互動式程序化草圖技術，讓設計師專注於描述想要建模的內容(what),而不是如何建模(how)                                                           |
| A Survey on Procedural Modelling for Virtual Worlds                                          | Smelik, R. M., Tutenel, T., Bidarra, R., & Benes, B. (2014, September). A survey on procedural modelling for virtual worlds. In _Computer graphics forum_ (Vol. 33, No. 6, pp. 31-50).                                                                      | **程序化建模**自動化地生成內容，有助於電影、遊戲和模擬中的虛擬環境。但在非技術創意人員中仍然存在接受挑戰。                                                           |
| A Survey on the Procedural Generation of Virtual Worlds                                      | Freiknecht, J., & Effelsberg, W. (2017). A survey on the procedural generation of virtual worlds. _Multimodal Technologies and Interaction_, _1_(4), 27.                                                                                                    | 程序化內容生成(PCG)的方法可以幫助開發者在有限的時間和預算內創建逼真、獨特的虛擬環境,為遊戲重新賦予可重玩性。                                                         |
| Synthesizing Personalized Training Programs for Improving Driving Habits via Virtual Reality | Lang, Y., Wei, L., Xu, F., Zhao, Y., & Yu, L. F. (2018, March). Synthesizing personalized training programs for improving driving habits via virtual reality. In _2018 IEEE conference on virtual reality and 3D user interfaces (VR)_ (pp. 297-304). IEEE. | 提出了一種基於虛擬現實的駕駛培訓新方法，可識別用戶的不當駕駛習慣,量身定制包含各種交通事件的虛擬培訓線路來幫助用戶改善，並經用戶研究證明其有效性優於其他培訓方式。                                 |
| # Automatic Synthesis of Virtual Wheelchair Training Scenarios                               | Li, W., Talavera, J., Samayoa, A. G., Lien, J. M., & Yu, L. F. (2020, March). Automatic synthesis of virtual wheelchair training scenarios. In _2020 IEEE Conference on Virtual Reality and 3D User Interfaces (VR)_ (pp. 539-547). IEEE.                   | 提出了一種基於優化的方法,可自動為虛擬現實中的殘疾人輪椅培訓生成虛擬場景,包括realistic家具布局和具有優化長度、轉彎程度、狹窄程度等特征的培訓路徑,用戶研究驗證了該虛擬現實培訓方法可提高殘疾人的輪椅控制熟練度和精準度。 |

==研究背景 VR硬體==

當前 VR 設備的易用性為 VR 培訓提供了許多好處。Anthes et al. （2016）[17] 總結了最常用的 VR 硬體和軟體。儘管仍存在如翼暈眩等問題，但仍一直在努力實現可用的VR設備。Jensen 和 Konradsen （2018）研究指出頭戴式顯示器（HMD），與其他沉浸程度較低的方法相比，使用 HMD 可以更好地增強認知技能、心理運動技能和情感技能[18]。Iosa等人（2015）通過在老年人中進行治療實驗，證明瞭使用Leap Motion感測器進行亞急性中風康復的可行性[19]。Kinect 感測器經常用於肢體的運動功能恢復訓練[20, 21, 22] 。Bogatinov 等人（2017年）探索了集成 Kinect 感測器以低成本提供槍支射擊訓練場景的可能性[23]。此外，舞蹈（Kyan et al.， 2015）[24]、運動遊戲（Zhang et al.， 2019）[25]、羽毛球（He et al.， 2014）[26]、乒乓球（Liu et al.， 2020）[27]和高爾夫（Lin et al.， 2013）[28]等運動訓練應用通常使用 Kinect 感測器。

Howard （2019）研究了不同VR設備與訓練結果的關係[29]。Papachristos等人（2017），Moro等人（2017）進行了比較不同VR頭盔的教學用途的研究 [30, 31]，並表明Oculus Rift等高端頭戴式顯示器和移動VR頭戴式設備等低端頭戴式顯示器在空間存在感、可用性和訓練結果等方面有一定作用。

==研究背景 急救人員培訓==

急救人員（例如員警、消防員和緊急醫療服務人員）經常面臨在其他工作領域不常見的況狀[32]。急救人員處理關鍵事件的能力與培訓程度正比相關；反之培訓不足可能導致急救人員無法完成任務，甚至可能造成人員傷害。而在現實環境中建立成本過高[33]。而在
虛擬實境中培訓急救人員可以顯著降低培訓成本並提高績效（Koutitas 等人，2020 年）[34]。也有研究證實政府部門已開始使用虛擬訓練作為戰鬥訓練的一部分。例如，紐約員警局 （NYPD） 使用 VR 進行主動射擊訓練（Melnick，2019 年）[35]。

Wilkerson等人（2008）提出洞穴自動虛擬環境CAVE，將立體圖像投射到牆壁和地板上，並增加定向聲音。用於培訓大規模傷亡事件的急救人員。其滿足不受限制的導航與虛擬物件的交互以及放置在環境中的物理物件[36]。

![[截圖 2024-03-31 下午5.01.43.png]]


Conges等人(2020年)提出的EGCERSIS項目,為危機管理團隊(包括警察、消防員和醫生)在關鍵地點進行培訓提供了一個框架,涉及如交通管制、滅火救援、醫療救護等典型任務[37]。並進一步演示營救一名躺在著火的地鐵月臺地板上的受傷男子。Mossel 等人（2017年）提出了一個VR平臺，該平臺可以與班長一起在現場進行身臨其境的急救人員培訓[38]。

而在協作能力的另一方面：團隊領導的培訓更注重領導能力。Mossel et al. （2017） 在他的方法中設計了四個領導力指標：1） PLAN，2） DO，3） CHECK 和 4） ACT。它被稱為PDCA迴圈。具體來說，培訓包括探索現場、做出決策、向請求供應人員下達命令、評估命令結果、識別與計劃的偏差以及調整行動[39]。

急救人員領域的另一個重要VR培訓專案是消防。Backlund 等人（2007 年）介紹了 Sidh，一種遊戲化的消防員培訓模擬器[40]。Heirman等人（2020年）提出了使用擴展現實技術來培訓海軍消防員的建議[41]。Pinto等人（2019）將VR用於氫燃料汽車事故的救援訓練。由於氫氣與一般汽油的特性存在差異，為救援人員的培訓提供了合適的平臺，並分別設立教程模式、培訓模式和認證模式[42]。

Koutitas et al. （2019） 使用 VR 平台培訓救護車巴士的工作人員，以提高他們的專業能力。有別於一般的救護車訓練，救護車的內部設施較為複雜，對工作任務的專業性要求更高。他們分別在VR和AR中演示了救護車內的訓練環境。使用者研究將受試者分為三個對照組，每個組都處於AR、VR和PowerPoint演示訓練模式。結果顯示AR組和VR組的受試者錯誤率明顯低於PowerPoint演示組[43]。




==研究背景 醫療培訓==

虛擬實境已被用於治療、治療、手術和通過類比損傷來創造體驗。使用設計合理的基於類比的培訓可以顯著減少衛生保健工作者的錯誤並提高患者安全性（Salas 等人，2005 年）[44] 。Hurd 等人（2019 年）探索了 VR 視頻遊戲在弱視治療中的應用[45]。Grantcharov 等人（2004 年）還通過對腹腔鏡膽囊切除術性能的隨機臨床試驗驗證了 VR 訓練優於傳統訓練[46]。也有相關研究證實類似結果[47, 48, 49]。

也曾經應用在鏡像治療中，用於減輕截肢者的患肢疼痛[50, 51, 52]（Fukumori 等人，2014 年，Ambron 等人，2018 年;Willis 等人，2019 年）通過將截肢者置於虛擬環境中並使用數據手套或視覺跟蹤來類比受影響肢體的運動，對截肢者進行虛擬鏡像治療[47, 48]。


VR在戰後恢復方面也顯示出重要用途。Rizzo等人（2014）使用VR系統作為暴露療法（VRET）工具，以說明患有創傷后應激障礙（PTSD）的士兵[53]。也有研究在臨床心理學中的可用性。Kenny等人（2009）以3D角色的形式創建了一個類比創傷后應激障礙的虛擬患者，該角色對臨床醫生的言語和手勢有反應[54]。（Huguet 等人，2016年）以評估沉浸感和臨場感等心理變數評估臨床醫生對吸收經驗的開放性，並創建了一個多智慧體虛擬體驗，類比了一家醫院醫院內的代理人配備了錯誤的溝通模型，以誘發受訓者的壓力[55]。


==引用

[1] https://www.merriam-webster.com/dictionary/training
[2] Conges, A., Evain, A., Benaben, F., Chabiron, O., & Rebiere, S. (2020, March). Crisis management exercises in virtual reality. In _2020 IEEE Conference on Virtual Reality and 3D User Interfaces Abstracts and Workshops (VRW)_ (pp. 87-92). IEEE.
[3] Xie, H., Tudoreanu, E., & Shi, W. (2006). Development of a virtual reality safety-training system for construction workers. _Digital library of construction informatics and information technology in civil engineering and construction_, 1-9.
[4] Martin, G., Schatz, S., Bowers, C., Hughes, C. E., Fowlkes, J., & Nicholson, D. (2009, October). Automatic scenario generation through procedural modeling for scenario-based training. In _Proceedings of the human factors and ergonomics society annual meeting_ (Vol. 53, No. 26, pp. 1949-1953). Sage CA: Los Angeles, CA: SAGE Publications.
[5] Martin, G. A., & Hughes, C. E. (2010, April). A scenario generation framework for automating instructional support in scenario-based training. In _Proceedings of the 2010 Spring Simulation Multiconference_ (pp. 1-6).
[6] Lin, F., Ye, L., Duffy, V. G., & Su, C. J. (2002). Developing virtual environments for industrial training. _Information sciences_, _140_(1-2), 153-170.
[7] Gilbreth, F. B., & Carey, E. G. (2013). _Cheaper by the Dozen_. Open Road Media.
[8] Xie, B., Liu, H., Alghofaili, R., Zhang, Y., Jiang, Y., Lobo, F. D., ... & Yu, L. F. (2021). A review on virtual reality skill training applications. Frontiers in Virtual Reality, 2, 645153.
[9] Salmon, P., Jenkins, D., Stanton, N., & Walker, G. (2010). Hierarchical task analysis vs. cognitive work analysis: comparison of theory, methodology and contribution to system design. _Theoretical Issues in Ergonomics Science_, _11_(6), 504-531.
[10] Lovreglio, R., Duan, X., Rahouti, A., Phipps, R., & Nilsson, D. (2021). Comparing the effectiveness of fire extinguisher virtual reality and video training. _Virtual Reality_, _25_(1), 133-145.
[11] Linowes, J. (2015). _Unity virtual reality projects_. Packt Publishing Ltd.
[12] Whiting, N., & Donaldson, N. (2014). Lessons from Integrating the Oculus Rift into Unreal Engine 4. In _Oculus Connect Developers Conference_.
[13] Taylor, R. M., Hudson, T. C., Seeger, A., Weber, H., Juliano, J., & Helser, A. T. (2001, November). VRPN: a device-independent, network-transparent VR peripheral system. In _Proceedings of the ACM symposium on Virtual reality software and technology_ (pp. 55-61).
[14] Smelik, R. M., De Kraker, K. J., Tutenel, T., Bidarra, R., & Groenewegen, S. A. (2009, June). A survey of procedural methods for terrain modelling. In _Proceedings of the CASA workshop on 3D advanced media in gaming and simulation (3AMIGAS)_ (Vol. 2009, pp. 25-34). sn.
[15] Parish, Y. I., & Müller, P. (2001, August). Procedural modeling of cities. In _Proceedings of the 28th annual conference on Computer graphics and interactive techniques_ (pp. 301-308).
[16] Yu, L. F., Yeung, S. K., Tang, C. K., Terzopoulos, D., Chan, T. F., & Osher, S. J. (2011). Make it home: automatic optimization of furniture arrangement. _ACM Transactions on Graphics (TOG)-Proceedings of ACM SIGGRAPH 2011, v. 30,(4), July 2011, article no. 86_, _30_(4).
[17] Anthes, C., García-Hernández, R. J., Wiedemann, M., and Kranzlmüller, D. (2016). “State of the Art of Virtual Reality Technology”, in IEEE Aerospace Conf., Big Sky, MT, 1–19.
[18] Jensen, L., & Konradsen, F. (2018). A review of the use of virtual reality head-mounted displays in education and training. _Education and Information Technologies_, _23_, 1515-1529.
[19] Iosa, M., Morone, G., Fusco, A., Castagnoli, M., Fusco, F. R., Pratesi, L., & Paolucci, S. (2015). Leap motion controlled videogame-based therapy for rehabilitation of elderly patients with subacute stroke: a feasibility pilot study. _Topics in stroke rehabilitation_, _22_(4), 306-316.
[20] Bao, X., Mao, Y., Lin, Q., Qiu, Y., Chen, S., Li, L., ... & Huang, D. (2013). Mechanism of Kinect-based virtual reality training for motor functional recovery of upper limbs after subacute stroke. _Neural regeneration research_, _8_(31), 2904-2913.
[21]Sin, H., & Lee, G. (2013). Additional virtual reality training using Xbox Kinect in stroke survivors with hemiplegia. _American journal of physical medicine & rehabilitation_, _92_(10), 871-880.
[22] |Park, D. S., Lee, D. G., Lee, K., & Lee, G. (2017). Effects of virtual reality training using Xbox Kinect on motor function in stroke survivors: a preliminary study. _Journal of Stroke and Cerebrovascular Diseases_, _26_(10), 2313-2319.
[23] Bogatinov, D., Lameski, P., Trajkovik, V., & Trendova, K. M. (2017). Firearms training simulator based on low cost motion tracking sensor. _Multimedia tools and applications_, _76_, 1403-1418.
[24] Kyan, M., Sun, G., Li, H., Zhong, L., Muneesawang, P., Dong, N., ... & Guan, L. (2015). An approach to ballet dance training through ms kinect and visualization in a cave virtual reality environment. _ACM Transactions on Intelligent Systems and Technology (TIST)_, _6_(2), 1-37.
[25] Zhang, Y., Xie, B., Huang, H., Ogawa, E., You, T., & Yu, L. F. (2019, May). Pose-guided level design. In _Proceedings of the 2019 CHI Conference on Human Factors in Computing Systems_(pp. 1-12).
[26] He, Z. D., Hu, R. M., & Xu, J. C. (2014). The development of badminton auxiliary training system based on Kinect motion capture. _Advanced Materials Research_, _926_, 2735-2738.
[27] Liu, H., Wang, Z., Mousas, C., & Kao, D. (2020, November). Virtual reality racket sports: Virtual drills for exercise and training. In _2020 IEEE International Symposium on Mixed and Augmented Reality (ISMAR)_ (pp. 566-576). IEEE.
[28] Lin, Y. H., Huang, S. Y., Hsiao, K. F., Kuo, K. P., & Wan, L. T. (2013). A kinect-based system for golf beginners’ training. In _Information Technology Convergence: Security, Robotics, Automations and Communication_ (pp. 121-129). Springer Netherlands.
[29] Howard, M. C. (2019). Virtual reality interventions for personal development: A meta-analysis of hardware and software. _Human–Computer Interaction_, _34_(3), 205-239.
[30] Papachristos, N. M., Vrellis, I., & Mikropoulos, T. A. (2017, July). A comparison between oculus rift and a low-cost smartphone VR headset: immersive user experience and learning. In _2017 IEEE 17th International Conference on Advanced Learning Technologies (ICALT)_ (pp. 477-481). IEEE.
[31] Moro, C., Štromberga, Z., & Stirling, A. (2017). Virtualisation devices for student learning: Comparison between desktop-based (Oculus Rift) and mobile-based (Gear VR) virtual reality in medical and health science education. _Australasian journal of educational technology_, _33_(6).
[32] Reichard, A. A., & Jackson, L. L. (2010). Occupational injuries among emergency responders. _American journal of industrial medicine_, _53_(1), 1-11.
[33] Karabiyik, U., Mousas, C., Sirota, D., Iwai, T., & Akdere, M. (2019). A virtual reality framework for training incident first responders and digital forensic investigators. In _Advances in Visual Computing: 14th International Symposium on Visual Computing, ISVC 2019, Lake Tahoe, NV, USA, October 7–9, 2019, Proceedings, Part II 14_ (pp. 469-480). Springer International Publishing.
[34] Koutitas, G., Smith, S., & Lawrence, G. (2021). Performance evaluation of AR/VR training technologies for EMS first responders. _Virtual Reality_, _25_(1), 83-94.
[35] Melnick, K. (2019). NYPD uses location-based VR for active shooter training. _VR Scout_.
[36]  Wilkerson, W., Avstreih, D., Gruppen, L., Beier, K. P., & Woolliscroft, J. (2008). Using immersive simulation for training first responders for mass casualty incidents. _Academic emergency medicine_, _15_(11), 1152-1159

[37] Conges, A., Evain, A., Benaben, F., Chabiron, O., & Rebiere, S. (2020, March). Crisis management exercises in virtual reality. In _2020 IEEE Conference on Virtual Reality and 3D User Interfaces Abstracts and Workshops (VRW)_ (pp. 87-92). IEEE.


[38] Mossel, A., Froeschl, M., Schoenauer, C., Peer, A., Goellner, J., and Kaufmann, H. (2017). “Vronsite: Towards Immersive Training of First Responder Squad Leaders in Untethered Virtual Reality”, in IEEE Virtual Reality, Los Angeles, CA, March 18, 2017 (New York, NY: IEEE), 357–358. doi:10.1109/VR.2017. 7892324

[39] Mossel, A., Froeschl, M., Schoenauer, C., Peer, A., Goellner, J., & Kaufmann, H. (2017, March). VROnSite: Towards immersive training of first responder squad leaders in untethered virtual reality. In _2017 IEEE Virtual Reality (VR)_ (pp. 357-358). IEEE.
[40] Backlund, P., Engstrom, H., Hammar, C., Johannesson, M., & Lebram, M. (2007, July). Sidh–a game based firefighter training simulation. In _2007 11th International Conference Information Visualization (IV'07)_ (pp. 899-907). IEEE.
[41] Cha, M., Han, S., Lee, J., & Choi, B. (2012). A virtual reality based fire training simulator integrated with fire dynamics data. _Fire safety journal_, _50_, 12-24.
[42] Pinto, D., Peixoto, B., Gonçalves, G., Melo, M., Amorim, V., and Bessa, M. (2019). “Developing Training Applications for Hydrogen Emergency Response Training”, in 2019 International Conference on Graphics and Interaction (ICGI), Faro, Portugal, Nov 21, 2019 (New York, NY: IEEE), 130–136. doi:10.1109/ICGI47575.2019.8955091
[43] Koutitas, G., Smith, K. S., Lawrence, G., Metsis, V., Stamper, C., Trahan, M., & Lehr, T. (2019, June). A virtual and augmented reality platform for the training of first responders of the ambulance bus. In _Proceedings of the 12th ACM International Conference on Pervasive Technologies Related to Assistive Environments_ (pp. 299-302).


[44] Salas, E., Wilson, K. A., Burke, C. S., and Priest, H. A. (2005). Using Simulation- Based Training to Improve Patient Safety: What Does it Take? Jt. Comm. J. Qual. Patient Saf. 31, 363–371. doi:10.1016/s1553-7250(05)31049-x

[45] Hurd, O., Kurniawan, S., & Teodorescu, M. (2019, March). Virtual reality video game paired with physical monocular blurring as accessible therapy for amblyopia. In _2019 IEEE Conference on Virtual Reality and 3D User Interfaces (VR)_ (pp. 492-499). IEEE.
[46] Grantcharov, T. P., Kristiansen, V. B., Bendix, J., Bardram, L., Rosenberg, J., & Funch-Jensen, P. (2004). Randomized clinical trial of virtual reality simulation for laparoscopic skills training. _Journal of British Surgery_, _91_(2), 146-150.
[47] Taffinder, N., Sutton, C., Fishwick, R. J., McManus, I. C., & Darzi, A. (1998). Validation of virtual reality to teach and assess psychomotor skills in laparoscopic surgery: results from randomised controlled studies using the MIST VR laparoscopic simulator. In _Medicine meets virtual reality_ (pp. 124-130). IOS Press.
[48] Seymour, N. E., Gallagher, A. G., Roman, S. A., O’brien, M. K., Bansal, V. K., Andersen, D. K., & Satava, R. M. (2002). Virtual reality training improves operating room performance: results of a randomized, double-blinded study. _Annals of surgery_, _236_(4), 458-464.
[49] Gurusamy, K. S., Aggarwal, R., Palanivelu, L., and Davidson, B. R. (2009). Virtual Reality Training for Surgical Trainees in Laparoscopic Surgery. Cochrane Database Syst. Rev. 1, CD006575. doi:10.1002/14651858.cd006575.pub2
[50] Fukumori, S., Gofuku, A., Isatake, K., & Sato, K. (2014, October). Mirror thrapy system based virtual reality for chronic pain in home use. In _IECON 2014-40th Annual Conference of the IEEE Industrial Electronics Society_ (pp. 4034-4039). IEEE.
[51] Ambron, E., Miller, A., Kuchenbecker, K. J., Buxbaum, L. J., & Coslett, H. (2018). Immersive low-cost virtual reality treatment for phantom limb pain: evidence from two cases. _Frontiers in neurology_, _9_, 337238.
[52] Gurusamy, K. S., Aggarwal, R., Palanivelu, L., & Davidson, B. R. (2009). Virtual reality training for surgical trainees in laparoscopic surgery. _Cochrane database of systematic reviews_, (1).
[53] Rizzo, A., Hartholt, A., Grimani, M., Leeds, A., & Liewer, M. (2014). Virtual reality exposure therapy for combat-related posttraumatic stress disorder. _Computer_, _47_(7), 31-37.
[54] Kenny, P. G., Parsons, T. D., and Rizzo, A. A. (2009). “Human Computer Interaction in Virtual Standardized Patient Systems,” in Human-Computer Interaction. Interacting in Various Application Domains. Editor J. A. Jacko (Berlin, Heidelberg: Springer Berlin Heidelberg)), 514–523. doi:10.1007/978-3- 642-02583-9_56
[55] Huguet, L., Lourdeaux, D., Sabouret, N., & Ferrer, M. H. (2016, April). Perturbed Communication in a Virtual Environment to Train Medical Team Leaders. In _MMVR_ (pp. 146-149).



