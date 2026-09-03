# Atmos Search Console

[中文](#中文) · [English](#english)

在线使用 / Live page: **https://gyjdb.github.io/alaska-search-console/**

## 中文

一个单文件、无依赖的浏览器搜索台，整合两类 Alaska / Atmos 行程：

1. 用现金购买 **Main Cabin**，横向比较低价并规划 qualifying segments；
2. 搜索美国、中国与欧洲之间的 **Atmos Rewards 伙伴奖励票月历**。

页面右上角可以随时切换中文 / English，语言、主题和搜索参数都会保存在当前浏览器。无需安装、构建、登录或后端服务；下载 `index.html` 后也可以直接打开使用。

### 现金 Main 搜索

- Flexible dates 整月日历与 Exact date 指定日期两种链接。
- 自定义机场、机场名称提示与最近搜索。
- 两张单程票的 **2 + 2 = 4 段**规划器。
- 东部 / 中部 → 西部比价矩阵。
- 西部短途与夏威夷岛内预设路线。
- 所有现金搜索链接固定为单程、现金票、Main Cabin。
- 已看标记、逐条打开、整组复制以及浅色 / 深色主题。

### 价格记录器

- 保存两张单程票的路线、日期、含税票价、实际航段、额外成本、状态与备注。
- 自动计算纯票价 / 段与全成本 / 段。
- 支持候选、已购、已飞三种状态。
- 只有「已购 / 已飞」且手动确认资格的航段才计入 8 段目标。
- 支持筛选、排序、编辑、删除与双语 CSV 导出。
- 可从“两程凑 4 段”一键带入路线。

### 里程票搜索

- 自定义奖励票月历，以及亚洲 / 中国和欧洲预设路线。
- 离美 / 回美方向切换。
- 舱位与人数控制。
- 伙伴标签、相邻月份比较、最近路线与订票提示。

### 本地数据与说明

偏好、已看标记和价格记录只保存在浏览器的 `localStorage`，不会上传，也不包含任何账号凭据。更换浏览器或清理网站数据前，请先导出重要价格记录。

本工具只负责生成 Alaska 搜索链接。票价、路线、执飞航司、舱位以及航段是否符合资格，均以 Alaska 实时结果和当期活动条款为准。

---

## English

A self-contained, dependency-free browser console for two Alaska / Atmos workflows:

1. finding low cash fares in **Main Cabin** while planning qualifying flight segments; and
2. launching **Atmos Rewards partner-award calendar** searches between the US, China, and Europe.

Switch between 中文 and English at any time from the top-right control. Language, theme, and search preferences persist in the current browser. There is no build step, server, account login, or external dependency; you can also download and open `index.html` directly.

### Cash Main search

- Flexible-date monthly calendars and exact-date result links.
- Custom airport search, airport-name suggestions, and recent routes.
- A two-ticket planner for building **2 + 2 = 4 segments**.
- An East / Central → West fare-comparison matrix.
- Western short-haul and Hawaii inter-island presets.
- Every cash-search URL is fixed to one-way, cash, Main Cabin.
- Opened-route markers, open-next controls, group copying, and light / dark themes.

### Price tracker

- Save each two-ticket plan with route, dates, tax-inclusive fares, actual segments, extra costs, status, and notes.
- Calculate airfare per segment and all-in cost per segment automatically.
- Track Candidate, Booked, and Flown states.
- Count only Booked / Flown segments whose eligibility was manually verified toward the 8-segment goal.
- Filter, sort, edit, delete, and export records to a language-aware CSV.
- Send a route directly from the two-ticket planner into the tracker.

### Award search

- Custom award calendars plus Asia / China and Europe route presets.
- Leaving-US and returning-US directions.
- Cabin and traveler controls.
- Partner labels, adjacent-month comparisons, recent routes, and booking notes.

### Local data and disclaimer

Preferences, opened-route markers, and price-tracker records stay only in the browser's `localStorage`. The tool does not upload or collect them and contains no credentials. Export important price records before changing browsers or clearing site data.

This tool only constructs Alaska search URLs. Alaska's live results and the current promotion terms remain the final source of truth for fares, routing, operating carriers, cabins, and segment eligibility.

The legacy `alaska_award_launcher.html` entry is kept in sync with `index.html` so older direct links continue to work.
