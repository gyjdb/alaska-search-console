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

- 默认只添加一张直飞票，填一次整张票含税总价即可。
- 联程点击「添加中转 / 航段」；一张票可含多个实际航段，无需拆分每段费用。
- 分开买的票点击「添加另一张票」，归入同一方案；酒店、地面交通等额外费用在方案层只计一次。
- 每个航段分别记录机场、当地出发日期、候选 / 已购 / 已飞状态与资格核对。
- 中转机场在相邻航段之间自动同步；改变机场后需重新核对对应航段资格。
- 分别展示票价 / 实际段、全成本 / 实际段和全成本 / 已核对合资格段。未填票价是「待补」，不当作零元。
- 只有已飞且确认资格的航段计入完成进度；已购待飞只计预计进度。目标可选 4 / 8 / 20 段或自定义。
- 支持筛选、排序、编辑、删除、JSON 完整备份 / 合并导入、旧版 CSV 导入和上一次修改前恢复。
- 新版 CSV 每行一个实际航段：整张票价只在该票首段出现，方案额外成本只在方案首行出现，避免重复求和。
- 「两程凑 4 段」仍可作为两张票的快捷模板，实际中转机场需自行填写。

#### 旧记录升级与备份

在原来使用的同一浏览器、同一网站打开新版，旧记录会自动迁移为两张票的方案。原始 v1 数据保持不动，v2 使用独立存储键。旧版只记段数、没有记录中转机场，所以这些机场显示为 `?`，不会猜测；价格、航段数、备注和原状态均保留，请核对逐段机场、日期与资格。

如果旧记录为了绕过表单限制填了虚拟第二张票，可在编辑中移除该票；若旧记录实际是一张联程票，请核对后改成单张票的真实航段结构和整张票总价。系统不会自行推断这类修改。

升级前建议从旧页面导出 CSV。更换浏览器或从本地 HTML 转到在线页面时，使用旧版 CSV 导入或新版 JSON 备份迁移；仅复制 HTML 文件不会复制浏览器记录。导入重复记录会跳过，同 ID 冲突保留本机版本并提示，不会悄悄覆盖。新版 CSV 用于分析，不支持完整恢复，请以 JSON 为备份格式。

每次成功修改前自动保留一个上一版本，可用「恢复上次修改前」撤销最近的改动。若数据损坏或浏览器存储失败，会明确提示并停止写入，不会把空列表当作成功恢复。

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

- Start with one nonstop ticket and enter its whole-ticket, tax-inclusive price once.
- Use “Add connection / flight” for connecting itineraries. A ticket can contain multiple actual flight segments without splitting its fare.
- Use “Add another ticket” for separately purchased tickets in the same plan. Plan-level hotel / ground-transport extras are counted once.
- Record airports, local departure dates, Candidate / Booked / Flown status, and eligibility separately for each flight.
- Connection airports synchronize between adjacent flights. Changing an airport requires rechecking eligibility for the affected flights.
- Compare airfare per actual segment, all-in cost per actual segment, and all-in cost per verified eligible segment. Missing fares remain pending, never zero.
- Only verified Flown segments count as completed. Eligible Booked segments count toward projected progress only. Choose 4 / 8 / 20 segments or a custom goal.
- Filter, sort, edit, delete, export / merge-import full JSON backups, import legacy CSV files, and restore the previous revision.
- New CSV exports have one row per flight: the whole-ticket fare appears only on its first flight, and plan extras only on the plan's first row, preventing double counting.
- The two-ticket planner remains a shortcut template; fill in the actual connection airports before saving.

#### Migration and backups

Open the new version in the same browser and on the same site to migrate old records automatically into two-ticket plans. Original v1 data remains untouched; v2 uses a separate storage key. Old records saved segment counts, not connection airports, so unknown airports appear as `?` rather than guessed values. Fares, counts, notes, and original statuses are preserved; review individual airports, dates, and eligibility.

If an old record included a dummy second ticket to work around the form, remove that ticket in the editor. If the old record actually describes one connecting ticket, review and change it to the real flight structure and whole-ticket total. These corrections are never inferred automatically.

Export CSV from the old page before upgrading. When changing browsers or moving from a local HTML file to the hosted page, import legacy CSV or a new JSON backup; copying the HTML file alone does not copy browser records. Duplicate imports are skipped. Conflicting IDs keep the local version with a notice rather than silently overwriting it. New CSV is for analysis, not full recovery; use JSON for backups.

Each successful edit retains one previous revision for undo. Corrupt data or unavailable browser storage produces an explicit warning; the app does not silently replace unreadable records with an empty list.

### Award search

- Custom award calendars plus Asia / China and Europe route presets.
- Leaving-US and returning-US directions.
- Cabin and traveler controls.
- Partner labels, adjacent-month comparisons, recent routes, and booking notes.

### Local data and disclaimer

Preferences, opened-route markers, and price-tracker records stay only in the browser's `localStorage`. The tool does not upload or collect them and contains no credentials. Export important price records before changing browsers or clearing site data.

This tool only constructs Alaska search URLs. Alaska's live results and the current promotion terms remain the final source of truth for fares, routing, operating carriers, cabins, and segment eligibility.

The legacy `alaska_award_launcher.html` entry is kept in sync with `index.html` so older direct links continue to work.
