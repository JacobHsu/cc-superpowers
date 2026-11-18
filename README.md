# Superpowers

**繁體中文** | [English](README.en.md)

Superpowers 是一套完整的軟體開發方法論，專為你的程式碼代理（coding agent）設計。它建立在一組可組合的 skills 之上，再加上一些初始指示，確保你的代理真的會使用它們。

## 目錄

- [運作方式](#運作方式)
- [商業服務](#商業服務)
- [開始使用](#安裝)
  - [Claude Code](#claude-code)
  - [Antigravity](#antigravity)
  - [Codex App](#codex-app)
  - [Codex CLI](#codex-cli)
  - [Cursor](#cursor)
  - [Devin CLI](#devin-cli)
  - [Factory Droid](#factory-droid)
  - [Gemini CLI](#gemini-cli)
  - [GitHub Copilot CLI](#github-copilot-cli)
  - [Grok Build CLI](#grok-build-cli)
  - [Kimi Code](#kimi-code)
  - [OpenCode](#opencode)
  - [Pi](#pi)
  - [Qwen Code](#qwen-code)
  - [Hermes Agent](#hermes-agent)
  - [Muse](#muse)
- [基本工作流程](#基本工作流程)
- [出問題時](#出問題時)
- [社群](#社群)
- [內容一覽](#內容一覽)
- [理念](#理念)
- [貢獻](#貢獻)
- [更新](#更新)
- [授權](#授權)
- [視覺輔助工具的遙測](#視覺輔助工具的遙測)

## 運作方式

從你啟動程式碼代理的那一刻就開始了。一旦它發現你要打造某樣東西，它*不會*直接跳進去寫程式，而是先退一步，問你真正想做的是什麼。

等它從對話中整理出規格後，會把規格切成夠短、讀得完也消化得了的段落給你看。

你核可設計之後，代理會擬定一份實作計畫，清楚到連一個熱情但品味差、沒有判斷力、不了解專案背景、又討厭寫測試的初階工程師都能照著做。計畫強調真正的紅燈／綠燈 TDD、YAGNI（You Aren't Gonna Need It，你不會需要它）和 DRY。

接著，只要你說「開始」，它就會啟動 *subagent-driven-development*（子代理驅動開發）流程，讓代理逐一處理每項工程任務，檢查並審查成果，然後繼續往下做。你的代理一次自主工作好幾個小時、而且不偏離你們訂好的計畫，並不少見。

還有很多細節，但這就是整個系統的核心。而且因為 skills 會自動觸發，你不需要做任何特別的事。你的程式碼代理就是擁有了 Superpowers。

## 商業服務

如果你在企業中使用 Superpowers，並且需要商業支援、額外工具或費用管理，歡迎來信 sales@primeradiant.com。

## 安裝

安裝方式依 harness（代理執行環境）而不同。如果你同時使用多個，每個都要分別安裝 Superpowers。

### Claude Code

Superpowers 可以從[官方 Claude plugin marketplace](https://claude.com/plugins/superpowers) 取得。

#### 官方 Marketplace

- 從 Anthropic 官方 marketplace 安裝 plugin：

  ```bash
  /plugin install superpowers@claude-plugins-official
  ```

#### Superpowers Marketplace

Superpowers marketplace 提供 Superpowers 以及其他幾個 Claude Code 相關 plugin。

- 註冊 marketplace：

  ```bash
  /plugin marketplace add obra/superpowers-marketplace
  ```

- 從這個 marketplace 安裝 plugin：

  ```bash
  /plugin install superpowers@superpowers-marketplace
  ```

### Antigravity

從這個 repository 以 plugin 形式安裝 Superpowers：

```bash
agy plugin install https://github.com/obra/superpowers
```

Antigravity 會列出每個已安裝 skill 的描述，而 `using-superpowers` skill 的描述會提示模型在對話一開始就載入它。要更新時，用同一個指令重新安裝即可。

### Codex App

Superpowers 可以從[官方 Codex plugin marketplace](https://github.com/openai/plugins) 取得。

- 在 Codex app 中，點選側邊欄的 Plugins。
- 你應該會在 Coding 區塊看到 `Superpowers`。
- 點 Superpowers 旁邊的 `+`，依照提示操作。

### Codex CLI

Superpowers 可以從[官方 Codex plugin marketplace](https://github.com/openai/plugins) 取得。

- 開啟 plugin 搜尋介面：

  ```bash
  /plugins
  ```

- 搜尋 Superpowers：

  ```bash
  superpowers
  ```

- 選擇 `Install Plugin`。

### Cursor

- 在 Cursor Agent 對話中，從 marketplace 安裝：

  ```text
  /add-plugin superpowers
  ```

- 或在 plugin marketplace 搜尋「superpowers」。

### Devin CLI

- 從這個 repository 安裝 plugin：

  ```bash
  devin plugins install obra/superpowers
  ```

- 更新到最新版本：

  ```bash
  devin plugins update superpowers
  ```

### Factory Droid

- 註冊 marketplace：

  ```bash
  droid plugin marketplace add https://github.com/obra/superpowers
  ```

- 安裝 plugin：

  ```bash
  droid plugin install superpowers@superpowers
  ```

### Gemini CLI

- 安裝 extension：

  ```bash
  gemini extensions install https://github.com/obra/superpowers
  ```

- 之後更新：

  ```bash
  gemini extensions update superpowers
  ```

### GitHub Copilot CLI

- 註冊 marketplace：

  ```bash
  copilot plugin marketplace add obra/superpowers-marketplace
  ```

- 安裝 plugin：

  ```bash
  copilot plugin install superpowers@superpowers-marketplace
  ```

### Grok Build CLI

Superpowers 可以從[官方 Grok plugin marketplace](https://github.com/xai-org/plugin-marketplace) 取得。

- 從 xAI 官方 marketplace 安裝 plugin：

  ```bash
  grok plugin install superpowers@xai-official --trust
  ```

- 或在 TUI 中開啟 marketplace，搜尋 Superpowers 並安裝：

  ```text
  /marketplace
  ```

### Kimi Code

Superpowers 已上架 Kimi Code 的 plugin marketplace。

- 開啟 Kimi Code 的 plugin 管理員：

  ```text
  /plugins
  ```

- 前往 `Marketplace` > `Superpowers` 並安裝。

- 或直接從這個 repository 安裝：

  ```text
  /plugins install https://github.com/obra/superpowers
  ```

- 詳細文件：[docs/README.kimi.md](docs/README.kimi.md)

### OpenCode

OpenCode 有自己的 plugin 安裝方式；即使你已經在其他 harness 用過 Superpowers，也要另外安裝。

- 告訴 OpenCode：

  ```
  Fetch and follow instructions from https://raw.githubusercontent.com/obra/superpowers/refs/heads/main/.opencode/INSTALL.md
  ```

- 詳細文件：[docs/README.opencode.md](docs/README.opencode.md)

### Pi

從這個 repository 以 Pi package 形式安裝 Superpowers：

```bash
pi install git:github.com/obra/superpowers
```

本機開發時，可以讓 Pi 把這份 checkout 當作暫時的 package 載入：

```bash
pi -e /path/to/superpowers
```

這個 Pi package 會載入 Superpowers 的 skills，以及一個小型 extension，在 session 啟動時和壓縮（compaction）之後注入 `using-superpowers` 啟動指示。Pi 本身原生支援 skills，所以不需要相容用的 `Skill` 工具。子代理和任務清單工具則仍是選用的 Pi 輔助 package。

### Qwen Code

Qwen Code 可以直接從 Claude Code marketplace 安裝 plugin。

- 從這個 repository 安裝 plugin，出現提示時選擇 `superpowers`：

  ```bash
  qwen extensions install obra/superpowers
  ```

- 之後更新：

  ```bash
  qwen extensions update superpowers
  ```

### Hermes Agent

從這個 repository 以 Hermes plugin 形式安裝 Superpowers：

```bash
hermes plugins install obra/superpowers --enable
```

安裝後請重新啟動所有進行中的 Hermes session。注意：Hermes 沒有壓縮後（post-compaction）的 hook，所以如果一個很長的 session 在壓縮時蓋掉了第一輪對話，啟動指示就會遺失。如果 skills 不再觸發，請開一個新的 session。

### Muse

Superpowers 提供原生的 Muse plugin：同一個 repo、同一套 skills，所有 harness 通用。`using-superpowers` 啟動指示透過原生的 `SessionStart` hook 注入，和 Claude Code、Codex、Cursor、Gemini、Pi 等其他 harness 一樣，不需要每個 session 手動啟用。

- 從本機 checkout 安裝：

  ```bash
  muse plugins install ./
  muse plugins approve superpowers
  ```

  或先 clone 再安裝：

  ```bash
  git clone https://github.com/obra/superpowers.git
  muse plugins install ./superpowers
  muse plugins approve superpowers
  ```

- 之後更新：

  ```bash
  muse plugins update superpowers
  ```

安裝後請重新啟動所有進行中的 Muse session，`SessionStart` hook 才會生效。Skills 會立即啟用，但 hooks 在第一次安裝時需要核可。要驗證是否安裝成功，請開一個新的 session 並輸入 `Let's make a react todo list`，安裝正確的話，會在寫任何程式之前自動觸發 `brainstorming`。版本記錄在 `.version-bump.json`，由 `scripts/bump-version.sh` 保持同步。

## 基本工作流程

1. **brainstorming**：在打造任何東西之前啟動。透過讓你自己描述的提問，引導出你真正想要什麼、以及為什麼，然後把它的理解複述給你修正。小改動在對話中達成共識即可；專案則會產出一份書面設計文件，讓實作者能據此規劃。

2. **using-git-worktrees**：設計核可後啟動。在新分支上建立隔離的工作區，執行專案設定，並確認測試基準是乾淨的。

3. **writing-plans**：拿到核可的設計後啟動。把工作拆成一口大小的任務（每項 2–5 分鐘）。每項任務都有確切的檔案路徑、完整的程式碼和驗證步驟。

4. **subagent-driven-development** 或 **executing-plans**：拿到計畫後啟動。前者為每項任務派出一個全新的子代理，每項完成後都審查一次（最徹底）；後者在目前的 session 中直接實作所有任務，最後再對整個分支做一次全新的審查（最省）。

5. **test-driven-development**：實作期間啟動。強制執行 RED-GREEN-REFACTOR：先寫會失敗的測試、看它失敗、寫最少的程式碼、看它通過、commit。在測試之前寫的程式碼會被刪掉。

6. **requesting-code-review**：在任務之間啟動。對照計畫進行審查，依嚴重程度回報問題。嚴重問題會擋住進度。

7. **finishing-a-development-branch**：任務完成時啟動。驗證測試，提供選項（merge／PR／保留／捨棄），並清理 worktree。

**代理在執行任何任務之前都會先檢查相關的 skills。** 這些是強制的工作流程，不是建議。

## 出問題時

有時候 session 會出狀況：skill 在不該觸發時觸發、該觸發時卻沒動靜，或是代理忽略計畫、重複做同樣的事、消耗的 token 比預期多。這時請你的程式碼代理「figure out what went wrong with superpowers in this session」，它就會呼叫 **diagnosing-superpowers** skill。要檢查先前的 session，請指名它：「figure out what went wrong with superpowers in session `<id>`」。

這個 skill 會讀取 session 紀錄，附上精確到行的證據回報發生了什麼事；如果你需要，還能打包一份去除敏感資訊的資料，用於回報 bug。

## 社群

Superpowers 由 [Jesse Vincent](https://blog.fsck.com) 和 [Prime Radiant](https://primeradiant.com) 的夥伴們打造。

- **Discord**：[加入我們](https://discord.gg/35wsABTejz)，取得社群支援、提問，以及分享你用 Superpowers 做的東西
- **Issues**：https://github.com/obra/superpowers/issues
- **版本發布通知**：[訂閱](https://primeradiant.com/superpowers/)以在新版本推出時收到通知

## 內容一覽

### Skills 函式庫

**測試**
- **test-driven-development**：RED-GREEN-REFACTOR 循環（含測試反模式參考）

**除錯**
- **systematic-debugging**：四階段根本原因分析流程（含 root-cause-tracing、defense-in-depth、condition-based-waiting 等技巧）
- **verification-before-completion**：確認問題真的修好了
- **diagnosing-superpowers**：找出 session 出了什麼問題並附上證據；匯出去除敏感資訊的資料包或提交 issue

**協作**
- **brainstorming**：在動手之前引導出意圖
- **writing-plans**：詳細的實作計畫
- **executing-plans**：直接執行計畫：單一 context，最後一次審查
- **dispatching-parallel-agents**：並行子代理工作流程
- **requesting-code-review**：審查前檢查清單
- **receiving-code-review**：回應審查意見
- **using-git-worktrees**：平行開發分支
- **finishing-a-development-branch**：merge／PR 決策流程
- **subagent-driven-development**：兩階段審查（先看是否符合規格，再看程式碼品質）的快速迭代

**Meta**
- **writing-skills**：依照最佳實踐建立新的 skills（含測試方法）
- **using-superpowers**：skills 系統簡介

## 理念

- **測試驅動開發**：永遠先寫測試
- **系統化勝過臨場發揮**：重流程，不靠猜
- **降低複雜度**：以簡單為首要目標
- **證據勝過宣稱**：宣告成功前先驗證

閱讀[最初的發布公告](https://blog.fsck.com/2025/10/09/superpowers/)。

## 貢獻

以下是 Superpowers 的一般貢獻流程。請注意，我們通常不接受新 skills 的貢獻，而且任何 skill 的更新都必須在我們支援的所有程式碼代理上都能運作。我們也不接受由代理撰寫、修正他人所提 issue 的 PR，除非是維護者要求的，即使你遇到同樣的問題也一樣；請改在既有的 issue 中補充你的回報。

1. Fork 這個 repository
2. 切換到 `dev` 分支
3. 為你的工作建立一個分支
4. 依照 `writing-skills` skill 來建立及測試新增或修改的 skills
5. 提交 PR，填寫 pull request 範本的每個區塊，包括由人類親自撰寫的摘要。

Skill 行為測試使用 [superpowers-evals](https://github.com/prime-radiant-inc/superpowers-evals/) 的 drill eval harness，clone 到 `evals/` 目錄，設定方式見 `evals/README.md`。Plugin 基礎架構的測試位於 `tests/`，透過對應的 `run-*.sh` 或 `npm test` 執行。

完整指南請見 `skills/writing-skills/SKILL.md`。

## 更新

Superpowers 的更新方式多少取決於程式碼代理，但通常是自動的。

## 授權

MIT 授權，詳見 LICENSE 檔案

## 視覺輔助工具的遙測

因為 skills 和 plugins 不會回傳任何資訊給作者，我們完全不知道有多少人在使用 Superpowers。預設情況下，brainstorming 選用的視覺輔助功能上的 Prime Radiant logo 會從我們的網站載入，請求中會帶上你使用的 Superpowers 版本。它不包含任何關於你的專案、prompt 或程式碼代理的資訊。我們看不到你的點擊，也看不到你在做什麼。這能讓我們大致了解有多少人在使用 Superpowers，以及使用的是哪個版本。這完全是選用的。要停用它，請將環境變數 `SUPERPOWERS_DISABLE_TELEMETRY` 設為任何代表 true 的值。Superpowers 也會遵守 Claude Code 的 `DISABLE_TELEMETRY` 和 `CLAUDE_CODE_DISABLE_NONESSENTIAL_TRAFFIC` 停用設定。
