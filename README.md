# 看診幫手 Clinic Helper

門診時用的小工具，單一 HTML 檔，不需安裝、不需網路後端，打開就能用。
A tiny single-file web tool for outpatient clinic work.

**線上使用：** 直接打開網址就可以使用了 [https://din0-3.github.io/PMR-clinic-helper/](https://din0-3.github.io/PMR-clinic-helper/)

## 功能

**ICD Code**
點人體圖上的部位，列出常用 ICD-10 碼；點一下即複製。

**日期格式**
輸入多組治療日期，一鍵複製成 `3月5日、3月12日` 或 `2026/03/05、2026/03/12` 格式。最後一格按 Tab 會自動新增一列。

**待辦清單**
簡單的待辦／已完成清單，重新整理後仍會保留。資料只存在你自己的瀏覽器（localStorage），不會上傳到任何地方；可用「匯出／匯入」備份或搬到別台電腦。

## 使用方式

- 線上：開 GitHub Pages 網址即可
- 離線：下載 `index.html`，用 Chrome 或 Safari 直接開啟

> 待辦資料是「每個瀏覽器各自一份」。無痕模式或某些預覽視窗無法保存資料，頁面會顯示提醒。

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
