# Skirt_Bone_Generation_Tool
# 裙子骨骼生成工具 | Skirt_Bone_Generation_Tool

用於產生裙子骨骼的 Blender 插件  
*A Blender add-on for generating bones for skirt rigs.*

---

**📥 請前往右側的 [Releases] 區下載你想要的版本**  
**📥 Please download from the [Releases] section on the right**

---

## 👋 關於作者 | About Me

嗨，大家好！我是 **沙士小弟**。  
最近我開發了一款 Blender 插件，名稱是：

> 🎀 **裙子骨骼生成工具**

之所以要研發這款插件，是因為我前陣子在研究，blender的裙子的物理要怎麼處理
我找到一位日本大佬的教學，雖然效果很好，但操作實在太麻煩了！  
假如我有很多角色需要穿裙子，那我先搞到崩潰。

所以我有了個想法：  
我雖然沒寫過 Blender 插件，但稍微接觸過一點 C 跟 Python，  
而且現在 AI 這麼厲害，那我是不是可以靠 AI 幫我做出一個插件？

於是我從2025年5月5日開始，開發到2025年5月16日 完成了這個插件的 beta 測試版

---

## 🛠 插件使用方法

安裝插件後，打開 Blender 的 N 面板，你會看到：

- `裙子骨骼生成工具`
  - `裙子基礎骨骼生成`
  - `骨骼轉換`

### ➤ 1. 基礎骨骼生成

1. 調整你需要的參數。
   - `骨骼練數量`
   - `連接數量`
2. 按下【生成】，此時就會生成一個基礎骨骼。

### ➤ 2. 骨骼轉換

1. 在【骨骼轉換】面板選擇模式。
2. 指定剛剛建立的基礎骨骼。
3. 點擊【啟動】，骨骼就完成了！

---

## 🔧 【骨骼轉換】面板模式說明 | Available Modes

目前共有 **五種模式**：

### 1. 💠 純 FK 模式
- 單純的骨骼鏈，只包含根骨，適用於手動控制。

### 2. 🎯 FK + 追蹤模式
- 多一個 **追蹤網格**，骨骼會朝向網格的頂點。
- 適合綁定在大腿上，讓裙子跟隨腿部動作。
- 保有 FK 控制骨骼。

### 3. 🌬 純物理模式
- 骨骼會根據布料模擬自動飄動。
- ⚠ 綁定時請將【物理控制】骨骼的「型變」關掉，避免權重問題。

### 4. 🌀 FK + 物理模式
- 同時保有布料模擬 + FK 控制。
- ⚠ 一樣建議關閉【物理控制】骨骼的型變。

### 5. 🔁 FK + 物理 + 追蹤模式
- 三種模式綜合：FK 控制 + 布料飄動 + 指向追蹤頂點。
- 適合需要完整裙子控制效果的場景。

---

🧪 **這是 Beta 測試版本，歡迎大家試用並提供意見！**


