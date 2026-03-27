# 🎮 未來學習型態設計書
## 「修真學院」— 融 School 42 法門與 RPG 技能樹於一爐

> 「學如逆水行舟，不進則退；修如登山臨淵，步步為營。」

---

## 壹、核心理念

```mermaid
mindmap
  root((道))
    無師而自通
    同儕而共進
    以項目煉心
    以技能證道
```

| School 42 精髓 | RPG 技能樹要素 | 融合之法 |
|----------------|----------------|----------|
| 無師制 | 自由加點 | 學子自選修煉路徑 |
| 同儕學習 | 公會組隊 | 結伴闖關、互評互助 |
| 專案導向 | 任務副本 | 以實戰項目為升級之道 |
| Piscine 試煉 | 新手村試煉 | 入門關卡篩選心志 |
| 等級制度 | 經驗值系統 | 量化成長、可視進度 |

---

## 貳、技能樹架構

### 總覽

```mermaid
flowchart TD
    subgraph 道心
        ROOT[【道心】Lv.0]
    end
    
    ROOT --> ENG[【器道】<br/>Engineering]
    ROOT --> SCI[【術道】<br/>Science]
    ROOT --> ART[【法道】<br/>Liberal Arts]
    
    ENG --> SW[鑄器・軟體]
    ENG --> CH[煉丹・化學]
    ENG --> HW[機關・硬體]
    
    SCI --> MA[算學・數學]
    SCI --> PH[物理]
    SCI --> BI[生機・生物]
    
    ART --> HU[文心・人文]
    ART --> BU[商略・商業]
    ART --> AR[藝境・藝術]
    
    style ROOT fill:#f9f,stroke:#333,stroke-width:3px
    style ENG fill:#bbf,stroke:#333
    style SCI fill:#bfb,stroke:#333
    style ART fill:#fbb,stroke:#333
```

### 以「鑄器道・軟體」為例

```mermaid
flowchart TD
    subgraph 軟體修煉路徑
        SW[【鑄器・軟體】]
        
        SW --> FE[前端築基<br/>Frontend]
        SW --> BE[後端煉丹<br/>Backend]
        SW --> SYS[系統機關<br/>Systems]
        
        FE --> HTML[HTML<br/>Lv.1]
        FE --> CSS[CSS<br/>Lv.1]
        FE --> JS[JavaScript<br/>Lv.2]
        
        BE --> SQL[SQL<br/>Lv.2]
        BE --> API[API<br/>Lv.3]
        BE --> CLOUD[雲端<br/>Lv.4]
        
        SYS --> LINUX[Linux<br/>Lv.2]
        SYS --> NET[網路<br/>Lv.3]
        SYS --> SEC[安全<br/>Lv.5]
        
        HTML --> REACT[React/Vue<br/>Lv.4]
        CSS --> REACT
        JS --> REACT
        
        SQL --> MICRO[微服務<br/>Lv.5]
        API --> MICRO
        
        LINUX --> DEVOPS[DevOps<br/>Lv.6]
        NET --> DEVOPS
        
        REACT --> FULL[【全棧真人】<br/>Lv.MAX]
        MICRO --> FULL
        DEVOPS --> FULL
    end
    
    style SW fill:#f9f,stroke:#333,stroke-width:2px
    style FULL fill:#ff0,stroke:#333,stroke-width:3px
```

---

## 參、修煉機制

### 一、入門試煉「泳池」(Piscine)

```mermaid
flowchart LR
    subgraph 泳池試煉【28日】
        D1[Day 1-7<br/>基礎語法<br/>獨自摸索]
        D2[Day 8-14<br/>小型項目<br/>同儕互評]
        D3[Day 15-28<br/>團隊副本<br/>存亡之戰]
        
        D1 --> D2 --> D3
    end
    
    D3 -->|通過| PASS[🎉 獲「學徒」身份<br/>正式入道]
    D3 -->|未通過| FAIL[⏳ 三月後可再試]
    
    style PASS fill:#9f9,stroke:#333
    style FAIL fill:#f99,stroke:#333
```

### 二、經驗值與等級

```mermaid
flowchart LR
    subgraph 修煉境界
        L0[凡人<br/>Lv.0]
        L1[學徒<br/>Lv.1-5<br/>0-1000 EXP]
        L2[築基<br/>Lv.6-10<br/>1001-5000 EXP]
        L3[結丹<br/>Lv.11-15<br/>5001-15000 EXP]
        L4[元嬰<br/>Lv.16-20<br/>15001-50000 EXP]
        L5[化神<br/>Lv.21+<br/>50001+ EXP]
        
        L0 -->|泳池試煉| L1
        L1 -->|基礎技能樹| L2
        L2 -->|專精分支| L3
        L3 -->|導師資格| L4
        L4 -->|創建公會| L5
    end
    
    style L0 fill:#ddd
    style L1 fill:#cfc
    style L2 fill:#9f9
    style L3 fill:#ff9
    style L4 fill:#f96
    style L5 fill:#f6f
```

### 三、經驗獲取之道

```mermaid
pie title 經驗值來源分佈
    "項目副本" : 45
    "同儕互動" : 30
    "特殊成就" : 25
```

| 類別 | 行為 | 經驗值 |
|------|------|--------|
| **項目副本** | 完成項目 | +100 |
| | 優秀評價 | +50 |
| | 團隊副本 | +200 |
| | 挑戰副本 | +300 |
| **同儕互動** | 評審他人 | +20 |
| | 被評優秀 | +30 |
| | 解答提問 | +15 |
| | 組隊加成 | ×1.5 |
| **特殊成就** | 首次通關 | +50 |
| | 連續簽到 | +10/日 |
| | 技能滿級 | +500 |
| | 跨界融合 | +1000 |

---

## 肆、項目副本系統

### 副本類型

```mermaid
flowchart TD
    subgraph 副本系統
        SOLO[【單人副本】<br/>⭐~⭐⭐⭐<br/>基礎練習・機器評審]
        TEAM[【組隊副本】<br/>⭐⭐⭐~⭐⭐⭐⭐<br/>2-5人協作・職業配合]
        GUILD[【公會戰】<br/>⭐⭐⭐⭐⭐<br/>跨公會競賽・企業題目]
        BOSS[【世界BOSS】<br/>⭐⭐⭐⭐⭐+<br/>開源專案・社會問題]
        
        SOLO --> TEAM --> GUILD --> BOSS
    end
    
    style SOLO fill:#cfc
    style TEAM fill:#9cf
    style GUILD fill:#fc9
    style BOSS fill:#f66
```

### 副本範例：「築網者」

```mermaid
flowchart TD
    subgraph 副本：築網者
        INFO[📋 副本信息<br/>前置：HTML Lv2, CSS Lv2, JS Lv1<br/>等級：築基期 Lv.6+<br/>時限：14日]
        
        TASK[📌 任務目標]
        T1[☐ 響應式設計]
        T2[☐ 至少三個頁面]
        T3[☐ 動態效果]
        T4[☐ 部署上線]
        
        REVIEW[🔍 評審方式<br/>三位同儕互評 + AI 代碼檢測]
        
        REWARD[🎁 獎勵]
        R1[基礎：+150 EXP]
        R2[優秀：+50 EXP +「築網者」稱號]
        R3[卓越：+100 EXP + 名人堂展示]
        
        INFO --> TASK
        TASK --> T1 & T2 & T3 & T4
        T1 & T2 & T3 & T4 --> REVIEW
        REVIEW --> REWARD
        REWARD --> R1 & R2 & R3
    end
```

---

## 伍、同儕互評機制

```mermaid
sequenceDiagram
    participant A as 學子A
    participant S as 系統
    participant R1 as 評審甲（同級）
    participant R2 as 評審乙（高一級）
    participant R3 as 評審丙（隨機）
    
    A->>S: 提交作品
    S->>S: 隨機分配三位評審
    
    par 同時評審
        S->>R1: 分配評審任務
        S->>R2: 分配評審任務
        S->>R3: 分配評審任務
    end
    
    R1->>S: 提交評分
    R2->>S: 提交評分
    R3->>S: 提交評分
    
    S->>S: 取中位數計算最終分數
    S->>A: 返回評審結果
```

### 評審獎懲

| 行為 | 結果 |
|------|------|
| 認真評審、給出建設性意見 | +20 EXP |
| 評審結果與最終一致 | +10 EXP（準確獎勵）|
| 敷衍評審 | -10 EXP、降低評審權重 |
| 惡意評審 | 禁止評審資格 30 日 |

---

## 陸、公會系統

```mermaid
flowchart TD
    subgraph 公會機制
        CREATE[創建條件<br/>結丹期 Lv.11+<br/>需 5 人以上]
        
        FUNC[公會功能]
        F1[💬 專屬討論區]
        F2[⚔️ 組隊副本加成]
        F3[📋 公會任務]
        F4[👨‍🏫 師徒系統]
        F5[🛠️ 公會技能]
        
        TYPE[公會類型]
        G1[鑄器閣<br/>純軟體]
        G2[煉丹谷<br/>純化學]
        G3[算學宗<br/>純數學]
        G4[混元派<br/>跨領域]
        
        CREATE --> FUNC
        FUNC --> F1 & F2 & F3 & F4 & F5
        CREATE --> TYPE
        TYPE --> G1 & G2 & G3 & G4
    end
    
    style G1 fill:#9cf
    style G2 fill:#f9c
    style G3 fill:#cf9
    style G4 fill:#fc9
```

---

## 柒、成就與稱號

```mermaid
flowchart LR
    subgraph 成就系統
        A1[🏊 泳池倖存者<br/>通過入門試煉<br/>+100 EXP]
        A2[📝 代碼詩人<br/>連續30日提交<br/>專屬頭像框]
        A3[👨‍🏫 良師益友<br/>評審100次獲好評<br/>評審權重×2]
        A4[🌐 跨界真人<br/>三領域達Lv.10<br/>+2000 EXP]
        A5[🚀 開源先鋒<br/>PR被知名專案合併<br/>全服公告]
        A6[💡 問題終結者<br/>解答500個問題<br/>專屬稱號色]
        A7[👑 公會之主<br/>公會達100人<br/>創建副本權限]
    end
```

---

## 捌、技術實現架構

```mermaid
flowchart TD
    subgraph 前端
        FE[Vue/React<br/>前端界面]
    end
    
    subgraph 後端
        BE[Node.js<br/>後端服務]
    end
    
    subgraph AI
        AI_ENGINE[LLM API<br/>AI 引擎]
    end
    
    subgraph 資料庫層
        DB1[(PostgreSQL<br/>用戶資料)]
        DB2[(MongoDB<br/>項目評審)]
        DB3[(Redis<br/>技能樹引擎)]
    end
    
    subgraph 基礎設施
        SANDBOX[Docker + K8s<br/>代碼沙盒與自動評測]
    end
    
    FE <--> BE
    BE <--> AI_ENGINE
    BE --> DB1 & DB2 & DB3
    BE --> SANDBOX
    
    style FE fill:#42b883
    style BE fill:#68a063
    style AI_ENGINE fill:#f9c
    style SANDBOX fill:#2496ed
```

---

## 玖、與傳統教育之比較

```mermaid
radar
    title 學習模式比較
    labels 教師依賴度, 自主程度, 協作強度, 反饋速度, 遊戲化程度, 實戰導向
    data 傳統學校: 90, 20, 30, 20, 10, 30
    data School_42: 10, 90, 90, 80, 40, 90
    data 修真學院: 10, 85, 95, 95, 95, 90
```

| 維度 | 傳統學校 | School 42 | 修真學院（本設計） |
|------|----------|-----------|-------------------|
| 教師 | 必需 | 無 | 無，但有「導師」玩家 |
| 課表 | 固定 | 自由 | 自由 + 推薦路徑 |
| 評量 | 考試 | 同儕互評 | 同儕 + AI 雙軌 |
| 動機 | 外在（分數）| 內在（興趣）| 遊戲化（成就感）|
| 進度 | 統一 | 自主 | 自主 + 可視化 |
| 協作 | 少 | 核心 | 核心 + 公會強化 |
| 反饋 | 延遲 | 即時 | 即時 + 量化 |

---

## 拾、未來展望

### 階段性目標

```mermaid
gantt
    title 開發路線圖
    dateFormat  YYYY-MM
    section MVP
    基礎技能樹           :2026-04, 2026-06
    單人副本系統         :2026-05, 2026-07
    經驗值系統           :2026-05, 2026-06
    section Beta
    同儕互評機制         :2026-07, 2026-09
    公會系統             :2026-08, 2026-10
    section 1.0
    企業合作             :2026-10, 2027-01
    世界BOSS             :2026-11, 2027-02
    section 2.0
    AI個人化推薦         :2027-02, 2027-06
    跨校聯盟             :2027-04, 2027-08
```

### 商業模式

```mermaid
flowchart TD
    subgraph 營收來源
        FREE[🆓 免費層<br/>基礎技能樹・單人副本]
        SUB[💎 訂閱層（月費）<br/>高級副本・公會功能・AI導師]
        ENT[🏢 企業層<br/>人才招聘・專屬副本・實習媒合]
        EDU[🎓 機構層<br/>學校/培訓機構授權]
    end
    
    FREE --> SUB --> ENT
    FREE --> EDU
    
    style FREE fill:#9f9
    style SUB fill:#99f
    style ENT fill:#f99
    style EDU fill:#ff9
```

---

## 結語

> 此設計取 School 42「無師自通、同儕共進」之精神，
> 融 RPG 技能樹「可視成長、成就驅動」之妙法，
> 冀望打造一學習型態，使學子如遊戲般沉浸，如修仙般精進。
>
> **「道可道，非常道；學可學，非常學。」**

---

## 授權

MIT License

## 作者

由 AI 助手協助設計，2026年3月

## 參考資料

- [School 42 Official](https://42.fr/)
- [Peer-to-Peer Learning](https://en.wikipedia.org/wiki/Peer_learning)
- [Gamification in Education](https://en.wikipedia.org/wiki/Gamification_of_learning)
- [MermaidJS Documentation](https://mermaid.js.org/)
