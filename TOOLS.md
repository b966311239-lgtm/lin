# 工具與環境配置 (TOOLS)

## 🖥 設備與網路環境
* **開發伺服器：** 林主機 (Linux 系統)。
* **網路連線：** 使用 4G 網路。每次開機第一時間必須確認 `tailscale funnel` 是打開的。
* **環境別名表：** AS = Android Studio｜咳嗽 = Cursor｜爪子 = OpenClaw｜特拉狗 = Claude Code。
* **顯示設定：** 1920x1080 (建議縮放 125%)。

## 🔧 技能管理清單 (Skills Registry)
* **[開發與自動化]**
 * `coding-agent`: 核心編碼工具，對接 Claude Code。
 * `oracle`: 專案打包工具，用於向 Gemini 尋求深度優化。
 * `skill-creator`: 當自動化流程有缺口時，用於開發新工具。
* **[專案記憶體]**
 * `obsidian`/`notion`: 同步 `MEMORY.md` 的精華，作為第二大腦。
 * `github`: 儲存 APK 源碼與市場研究筆記。
* **[偏好設定]**
 * `sag` (TTS): 語音回報開發進度時，偏好親切女聲 (小美風格)。
 * `weather`: 每日開機彙報時，附帶台灣天氣狀況。

## ⚙️ 技能的命名與規則（MCP 開發者最佳實踐）
未來使用 `skill-creator` 自己寫技能時，嚴格遵守三大鐵律：
1. **命名格式絕對要連貫**：
 * ⭕️ 正確：使用 `snake_case`（蛇形命名），如 `search_github_repo`。
 * ❌ 錯誤：絕對不要用空格或句號（如 `search.github`）。這會讓 AI 的 Tokenizer（分詞器）錯亂，導致呼叫失敗。
2. **「動詞 + 名詞」的精準結構**：
 * 不要只把技能命名為 `github`。要寫成 `get_github_issues`。AI 很笨，給它動詞才知道這工具能幹嘛。
3. **描述 (Description) 比檔名更重要**：
 * 這是「寫給 AI 看的提示詞」。必須極度具體！
 * 高手寫法範例：`"description": "當需要打包 Android Studio 的 .kt 專案程式碼時，使用此工具。"`（越具體，AI 越不會用錯）。

## What Goes Here

Things like:

- Camera names and locations
- SSH hosts and aliases
- Preferred voices for TTS
- Speaker/room names
- Device nicknames
- Anything environment-specific

## Examples

```markdown
### Cameras

- living-room → Main area, 180° wide angle
- front-door → Entrance, motion-triggered

### SSH

- home-server → 192.168.1.100, user: admin

### TTS

- Preferred voice: "Nova" (warm, slightly British)
- Default speaker: Kitchen HomePod
```

## Why Separate?

Skills are shared. Your setup is yours. Keeping them apart means you can update skills without losing your notes, and share skills without leaking your infrastructure.

---

Add whatever helps you do your job. This is your cheat sheet.
