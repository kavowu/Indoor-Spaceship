# PICT 技術故事網站

一個關於光觸媒技術(PICT)從科學發現到現代應用的故事型銷售網站。

## 網站結構

```
pict-story-website/
├── index.html              # 首頁
├── pages/
│   ├── story.html         # 技術演進頁面
│   ├── firewall.html      # 三道防火牆頁面
│   ├── comparison.html    # 市場對比頁面
│   └── pict.html          # PICT優勢頁面
├── css/
│   ├── styles.css         # 全局樣式
│   ├── story.css          # 技術演進頁面樣式
│   ├── firewall.css       # 三道防火牆頁面樣式
│   ├── comparison.css     # 市場對比頁面樣式
│   └── pict.css           # PICT優勢頁面樣式
├── js/
│   └── main.js            # 主要JavaScript功能
└── images/
    └── [圖像文件]
```

## 功能特性

### 1. 首頁 (index.html)
- Hero區域：展示太空艙主題的大型背景圖像
- 技術演進時間軸：展示1967-2016年的光觸媒發展歷程
- 新型建築區域：解釋現代建築的挑戰
- 三道防火牆預覽：介紹安全檢驗標準

### 2. 技術演進頁面 (pages/story.html)
- 六個章節詳細講述光觸媒技術的完整歷史
- 從1967年科學發現到2020年代的應用
- 包含圖像、文字和關鍵信息

### 3. 三道防火牆頁面 (pages/firewall.html)
- 詳細解釋三道安全防火牆的科學標準
- 對比市場上常見的問題與PICT的解決方案
- 包含安全濃度動態平衡模型公式

### 4. 市場對比頁面 (pages/comparison.html)
- 完整的對比表格：RGF、虛假品牌、選擇性披露品牌、PICT
- 詳細分析各品牌的優缺點
- 強調PICT的唯一優勢

### 5. PICT優勢頁面 (pages/pict.html)
- 四大核心優勢：產物透明化、過程潔淨化、濃度科學化、零耗材低能耗
- 三個長期實證案例：桃園機場、馬偕醫院、國泰長照
- 技術規格和選擇PICT的理由

## 技術實現

### HTML
- 使用語義化HTML5標籤
- 清晰的頁面結構
- 響應式設計支持

### CSS
- 使用CSS3特性實現視覺效果
- Flexbox和Grid布局
- 完整的響應式設計（支持桌面、平板、手機）
- 動畫效果：淡入淡出、視差滾動、懸停效果

### JavaScript
- 純JavaScript實現，無前端框架
- 導航功能：活動鏈接高亮、漢堡菜單
- 視差滾動效果
- 回到頂部按鈕
- 頁面加載動畫
- Intersection Observer API用於元素動畫

## 設計系統

### 色彩方案
- 主色：深藍色 (#0f766e)、亮藍色 (#2563eb)
- 輔助色：青色、綠色、紅色
- 背景：白色、淺灰色
- 文字：深灰色、黑色

### 排版
- 字體：Noto Sans TC (中文)、Sans-serif (英文)
- 標題：大字體、粗體、深色
- 副標題：中等字體、灰色
- 正文：標準字體、深灰色

### 響應式斷點
- 桌面：1200px+
- 平板：768px-1199px
- 手機：480px-767px
- 小手機：<480px

## 圖像文件

網站需要以下圖像文件（放在 `images/` 文件夾中）：

| 文件名 | 用途 | 建議尺寸 |
|--------|------|---------|
| space-capsule.jpg | Hero背景 | 1920x1080px |
| modern-building.jpg | 新型建築區域 | 800x600px |
| scientist-lab.jpg | 科學家實驗室 | 800x600px |
| space-station.jpg | 太空站 | 800x600px |
| market-growth.jpg | 市場增長 | 800x600px |
| pict-birth.jpg | PICT誕生 | 800x600px |
| covid-test.jpg | 新冠疫情 | 800x600px |
| new-building.jpg | 新型建築 | 800x600px |
| airport.jpg | 桃園機場 | 600x400px |
| hospital.jpg | 馬偕醫院 | 600x400px |
| care-center.jpg | 長照中心 | 600x400px |

## 部署方式

### 本地測試
1. 在本地開發環境中打開 `index.html`
2. 或使用簡單的HTTP服務器：
   ```bash
   # Python 3
   python3 -m http.server 8000
   
   # Node.js
   npx http-server
   ```

### 生產部署
1. 將所有文件上傳到Web服務器
2. 確保所有圖像文件都已上傳到 `images/` 文件夾
3. 設置服務器支持HTML5路由（如需要）

## 瀏覽器支持

- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+
- 移動瀏覽器（iOS Safari、Chrome Mobile）

## 性能優化

- 使用CSS3實現動畫而非JavaScript
- 使用Intersection Observer API進行高效的元素觀察
- 響應式圖像支持
- 最小化CSS和JavaScript文件
- 使用視差滾動效果優化視覺體驗

## 自定義指南

### 修改顏色
編輯 `css/styles.css` 中的CSS變數：
```css
:root {
    --primary-color: #0f766e;
    --secondary-color: #2563eb;
    /* ... 其他顏色 */
}
```

### 修改字體
在HTML文件的 `<head>` 中修改Google Fonts連結，或在CSS中更改 `font-family`

### 添加新頁面
1. 在 `pages/` 文件夾中創建新的HTML文件
2. 複製現有頁面的結構
3. 在導航欄中添加新鏈接
4. 創建相應的CSS文件

## 許可證

© 2024 PICT 技術故事. All rights reserved.

## 聯絡方式

如有任何問題或建議，請聯絡我們。

---

**最後更新**: 2024年12月
**版本**: 1.0
