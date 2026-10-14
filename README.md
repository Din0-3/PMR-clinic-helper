# 復健科看診幫手 / PMR Clinic Helper

門診時用的小工具，單一 HTML 檔，不需安裝、不需網路後端，打開就能用。
A tiny single-file web tool for outpatient clinic work.

**線上使用：** 直接打開網址就可以使用了 [https://din0-3.github.io/PMR-clinic-helper/](https://din0-3.github.io/PMR-clinic-helper/)

## 功能

**ICD Code**
點人體圖上的部位，列出常用 ICD-10 碼；點一下即複製。

**PE 模版**
點部位後，ICD 碼下方會出現該部位的理學檢查（PE）模版：點內文或 Copy 即複製，按「✎ 編輯」修改（自動儲存），「+ 新增模版」可為同一部位加多個模版。每個部位預設附一份範例，可直接改成自己的版本。模版存在瀏覽器裡，可用「PE 模版備份：匯出／匯入」備份或分享給同事（匯入為合併，不會覆蓋現有模版）。

**日期格式**
輸入多組治療日期，一鍵複製成 `3月5日、3月12日` 或 `2026/03/05、2026/03/12` 格式。最後一格按 Tab 會自動新增一列。

**待辦清單**
簡單的待辦／已完成清單，重新整理後仍會保留。資料只存在你自己的瀏覽器（localStorage），不會上傳到任何地方；可用「匯出／匯入」備份或搬到別台電腦。

## 使用方式

- 線上：開 GitHub Pages 網址即可
- 離線：下載 `index.html`，用 Chrome 或 Safari 直接開啟

> 待辦與 PE 模版是「每個瀏覽器各自一份」。無痕模式下可以暫存，但關閉所有無痕視窗後資料就會清除；推薦定期「匯出」備份比較不會被其他人誤刪喔。

## 自訂 ICD 清單

用文字編輯器打開 `index.html`，搜尋 `const icdCodes`，照格式增刪即可：

```js
knee: [
  'M17.0 - knee OA',
  'S83.2 - Tear of meniscus',
],
```

## 免責聲明

ICD 碼清單為個人臨床常用整理，僅供參考，請以健保署公告之 ICD-10-CM 為準。本工具不提供任何醫療建議。

## 致謝

人體剪影：["Man and woman silhouettes 2"](https://openclipart.org/detail/345637/man-and-woman-silhouettes-2) by DG-RA，取自 Openclipart（Public Domain）。

## License

[MIT](LICENSE)
