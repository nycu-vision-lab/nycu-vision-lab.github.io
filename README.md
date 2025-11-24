# **NYCU IEE Vision Lab**

## **# Folder structure**
```
nycu-vision-lab.github.io/
├─ assets/
│  ├─ css/
│  │   └─ styles.css
│  ├─ js/
│  │   └─ main.js
│  └─ img/
│      ├─ advisor/…     ← 教授照片
│      ├─ index/…       ← 主頁圖片
│      ├─ members/…     ← 成員頭像
│      └─ research/…    ← 研究圖、示意圖
├─ data/
│  └─ research/
│      ├─ index.json    ← 各 Projects 的資訊 (給 JS 讀的)
│      └─ xxx.md        ← Project 文章
├─ index.html           ← Home (Vision Lab)
├─ advisor.html         ← Advisor
├─ members.html         ← Member
├─ research.html        ← Research
└─ courses.html         ← Course
```

</br>

## **# Tutorial**
- **本地修改網頁:**
    1. 先安裝好 VSCode 以及 Github Desktop (並登入 nycu-vision-lab)。
    2. 用 Github Desktop 把 nycu-vision-lab.github.io 的 Repository 給 Clone 下來。
    3. 在 VSCode 開啟那個 Clone 下來的資料夾，並使用 Live Server (Go Live) 的功能在本地開啟假網頁。
    4. 更新好的時候去 Githun Desktop 把它 Push 上去。
    5. _(以上步驟有困難都屬於不熟悉使用 VSCode 或 Github，上網查或問 GPT 絕對能解決！)_

- **更新圖片:**
    1. 把新圖片放到 `assets/img/...` 中。
    2. 到要更新的頁面 (`xxx.html`) 找到描述要更新的圖片的地方。
    3. 把對應的圖片相對路徑位置更新上去。

- **更新 Member:**
    1. 到 `members.html` 找到想更新的位置。
    2. 依照以下結構為一屆，新增到 `<h2>Master Students</h2>` 的下方裡面：
        ```html
        <!-- Grade -->
        <h3 class="member-year">123</h3>
        <div class="member-grid">
          <!-- Member 1 -->
          <article class="member-card"> 
            <img src="assets/img/members/member_photo.jpg" />
            <div class="member-info">
              <h3>學生A</h3>
              <p class="member-role">Master Student</p>
            </div>
          </article>

          <!-- Member 2 -->
          <article class="member-card">
            <!-- 沒有圖片的話就不用放 -->
            <div class="member-info">
              <h3>學生B</h3>
              <p class="member-role">Master Student</p>
            </div>
          </article>
        </div>
        ```

- **更新 Research Project:**
    1. 新增文章 `.md` 檔案 (就是 Markdown 文字檔) 到 `data/research/` 資料夾中。
    2. 放置圖片到 `assets/img/research/` 資料夾中。
    3. 仿照其他篇的格式，更改 `data/research/index.json` 檔案中的資訊。
        ```
        {
            "group": "recent",  ← (或者是 "previous")
            "file": "my_research.md",  ← (放置在 `data/research/` 資料夾中的 `.md` 檔案名稱)
            "images": [
              {
                "src": "assets/img/research/my_research.png",
                "alt": "This is my research",  ← (這邊填什麼其實不太重要)
                "caption": "Fig. MY RESEARCH"  ← (如果想加圖片標題的話，沒有標題就不用這項)
              }
            ],
            "videos": [
              {
                "label": "Video 1",  ← (想顯示的影片名稱)
                "url": "https://www.youtube.com/XXX"  ← (影片連結)
              }, {
                "label": "Video 2",
                "url": "https://www.youtube.com/XXX"  ← (第二個影片連結)
              }
            ]
        }
        ```

- **更新 Others:**
    1. 想要更改更多東西的話，就得靠直接改寫 html 來改動內文了！
    2. 如果是想改模板樣式 (也就是 CSS)，都放在 `assets/css` 裡面！

- **Notice:**
    - 絕對不要更動 `index.html`, `advisor.html`, `members.html`, ... 的檔案名稱。</br>
      (會讓網頁連結壞掉，除非確定所有寫到網頁連結的地方都一併修改好。)
    - 請務必在本地端開假網頁測試過沒問題再 Push 上去。

</br>

## **# Contributors**
- **BSChen**
    - Create the website
    - 2025 / 11 ~ Now

</br>

---
_Have a good day :D  -- BSChen_
