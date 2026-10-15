慈濟大學經營管理學系｜粉色系簡約風系網頁

檔案結構：
- index.html：系所簡介首頁
- studentworks.html：學生作品展示頁
- graph/：網頁使用的所有本地圖片素材（SVG）

本網站設計方向：日本設計科系常見的留白、編輯式排版、低飽和粉色與簡潔圖形；以繁體中文呈現，並支援手機與桌面瀏覽。

如何預覽：
1. 解壓縮後，直接以瀏覽器開啟 index.html。
2. 點選首頁導覽列的「學生作品」測試兩頁互相切換。

上傳 GitHub Pages：
1. 建立 Public repository。
2. 將 index.html、studentworks.html、graph 資料夾及 README.txt 一併上傳到 repository 根目錄。
3. 到 Settings → Pages，將 Build and deployment 的 Source 選為 Deploy from a branch，Branch 選 main，資料夾選 /(root)，再按 Save。
4. 等待 Pages 建置完成後，使用 GitHub Pages 顯示的網址。

修改圖片：
所有圖片都位於 graph 資料夾，HTML 使用相對路徑，例如 src="graph/hero-art.svg"。
studentworks.html 的專案圖目前是「版面示意圖」，正式繳交前可將自己的照片或作品圖放進 graph，再修改 img 的 src、標題與描述。

加入影片的方式：
將影片檔案放在 graph 資料夾，之後可把影片展示區的圖片替換為：
<video controls poster="graph/video-cover.jpg" width="100%">
  <source src="graph/your-video.mp4" type="video/mp4">
  您的瀏覽器不支援 HTML video。
</video>
注意：請將 your-video.mp4 與 video-cover.jpg 換成實際檔名。

內容與資訊來源：
系所官方網站：https://mdm.tcu.edu.tw/p/412-1021-2.php
首頁系所介紹、課程面向與學生作品說明為此網站的設計提案。正式上線前，請依系上最新公告核對需公開的課程與系所資訊。

重要：若要上傳 GitHub Pages，請將 index.html、studentworks.html、README.txt 與 graph 資料夾「裡面的內容」直接放在 Repository 的根目錄，不要再放進額外的子資料夾。首頁與學生作品頁使用 ./studentworks.html、./index.html 相對連結，兩個 HTML 檔必須放在同一層。
