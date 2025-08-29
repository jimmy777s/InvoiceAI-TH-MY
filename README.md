# 📌 InvoicAI-TH-MY 使用指南

**自动化发票信息提取工具**  
（支持泰国 & 马来西亚发票PDF处理）

---

## 🚀 快速开始
### 方式一：从 SharePoint 上传
1. **访问路径**  
   `SalesandCash-Vistra/NDF2/Tax invoice`
2. **选择类别** → 输入月份文件夹名  
   - 常规格式：`MM Mon`（以sharepoint具体创建的文件夹名决定）  
   - Robinhood 特殊格式：`06 Jun 25/M184519`

### 方式二：本地上传
1. **先选择类别**  
2. **上传文件夹**（自动读取所有PDF文件）  
   ⚠️ 仅支持PDF格式
   
### 方式三：邮箱上传
1.**Outlook文件夹名称**
 - 文件夹名称示例：GZASC-THFIN\Inbox
 - 目前仅支持下载pdf，如果附件里面有无用的pdf，需要去缓存区手动剔除。
 - 缓存区地址：C:\Users\用户名\AppData\Local\Temp\3. Thailand
   
2.**附件关键词**
  - 支持自设

3.**日期**
  - 日期设置在需要提取的邮件发送时间之前
  - 格式：23/7/2025 (週三) 13:42 或者 Wednesday, July 30, 2025 02:48 PM 
---

## 📂 文件结构规范
### 输出路径示例
```plaintext
Thailand & Maylaysia - Extract invoice information/
└── 3. Thailand/
    └── 6. SBUX/
        └── NDF2/
            └── 4. Invoices/
                ├── Jul/
                │   ├── BBL_Starbucks/  [PDF存放处]
                │   └── SBUX_NDF2_Jul_results.xlsx    [输出文件]
                └── processing_log.xlsx   [全局日志]
```

---

## 🔄 数据恢复
### 如需修复历史数据
- 访问备份路径 \\10.86.2.112\SEA AR - Extract invoice information
- 按时间戳查找最近的文件

---
# Tips
- 如果文件之前识别过，希望再识别一次，在processing_log里面将文件的状态改为失败，就可以让程序重新识别。
- 打开缓存区按键弹窗显示缓存区不存在，运行一次程序后会新建缓存区。


