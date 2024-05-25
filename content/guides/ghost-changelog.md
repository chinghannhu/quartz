---
title: Ghost 架站日誌
draft: false
tags:
  - seeds
  - technical
date: 2021/11/22
description: 在 2021 年的秋天，我的 Ghost(Pro) 架站旅程正式啟航。
---
## [1.6.7] - 2023-10-16

### modified

- kobo、讀冊、台北圖書館超連結加入 icon，移除超連結結尾箭頭符號

```
a[href^="https://book.tpml.edu.tw/"], a[href^="https://book.tpml.edu.tw/"] {
  background: transparent url(https://www.chinghannhu.com/content/images/2023/08/tplib.svg) no-repeat center right;
  padding-right: 26px;
}
```

```
  a[href^="https://book.tpml.edu.tw"]::after {
  display: none;
  }
```

---

## [1.6.6] - 2023-10-15

### modified

- [ HTML/CSS ] 超連結結尾加入箭頭符號

```
a::after {
  content: " ↗";
  font-size: 0.8em;
    }
```

### reference

- [html - Line-break in inline-links with icon in the end (css) - Stack Overflow](https://stackoverflow.com/questions/71124706/line-break-in-inline-links-with-icon-in-the-end-css)

---

## [1.6.5] - 2023-09-18

### checked

- 更換網域到 Cloudflare
- ghost support: When using Cloudflare, you need to make sure to set the Proxy status to ****"DNS only"**** as with the "Proxied" status it won't allow our system to look up the records and make the connection.

### reference

- [Google Domains 網域搬家到 Cloudflare 教學 » 科技人](https://techtarian.com/others/guide/google-domains-transfer-to-cloudflare/)

---

## [1.6.5] - 2023-08-03

### modified

- [ HTML/CSS ] 更動導覽列英文大小寫

```
nav.gh-head-menu {
  text-transform:capitalize;
}
```

### reference

- [控制字母的大小寫──CSS的text-transform](https://www.webdesigns.com.tw/css_text-transform.asp)

---

## [1.6.4] - 2023-03-01

### modified

- [ HTML/CSS ] 圖片新增陰影

```
box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
```

- [ HTML/CSS ] 更改反白顏色

```
::selection {
  background: #fac7ae;
}
```

### reference

- [CSS Box Shadow](https://www.w3schools.com/css/css3_shadows_box.asp)
- [CSS ::selection Selector](https://www.w3schools.com/cssref/sel_selection.php)

---

## [1.6.3] - 2023-02-17

### modified

- 新增 Open Graph

### reference

- [OpenGraph - Preview Social Media Share and Generate Metatags](https://www.opengraph.xyz/)

---

## [1.6.2] - 2023-02-16

### modified

- [ HTML/CSS ] 超連結的底線向下移動 2px

```
text-underline-offset: 2px;
```

- 置入 kobo Logo 在樂分紅連結最後

```
/* Rakuten icon for affiliate geni.us links */

a[href^="https://r10.to/"], a[href^="https://r10.to/"] {
background: transparent url(https://www.huchinghann.com/content/images/2023/02/rakutenLogo15px.svg) no-repeat center right;
padding-right: 18px;
}
```

---

## [1.6.1] - 2022-11-25

### modified

- [ HTML/CSS ] 改變滑鼠游標的形狀 / 關掉圖片 Lightbox 效果

```
/* disable hover */

body#collection-5ed02ebed97d7907c6917792 .slides .slide {
    pointer-events: none;
}

.kg-gallery-image, .kg-image[width][height] {
    cursor: default;
}
```

```
/* disable lightbox */
.kg-gallery-image, .kg-image[width][height] {
    cursor: default;
}
```

### reference

- [How to Disable Lightbox mode on a Gallery Page (not gallery block)](https://forum.squarespace.com/topic/163487-how-to-disable-lightbox-mode-on-a-gallery-page-not-gallery-block/)
- [CSS 語法「cursor 屬性」改變滑鼠游標的形狀](http://www.flycan.com/article/css/css-cursor-209.html)

---

## [1.6.0] - 2022-11-15

### checked

- 新增[留言區](https://ghost.org/changelog/native-comments/)

---

## [1.5.1] - 2022-08-06

### modified

- 微調 code 區塊

### reference

- [A complete guide to code snippets](https://ghost.org/tutorials/code-snippets-in-ghost/)

---

## [1.5.0] - 2022-07-25

### checked

- 新增[站內搜尋](https://ghost.org/changelog/search/)

---

## [1.4.2] - 2022-03-29

### modified

- [ HTML/CSS ] div 不換行

### reference

- [div 並排不換行顯示](https://www.html8.com.cn/css/875.html)

---

## [1.4.1] - 2022-02-23

### modified

- [ HTML/CSS ] 更改手機網址進度條顏色 / 螢光筆、背景顏色透明度

### reference

- [How to change the color of header bar and address bar in newest Chrome version on Lollipop? - Stack Overflow](https://stackoverflow.com/questions/26960703/how-to-change-the-color-of-header-bar-and-address-bar-in-newest-chrome-version-o)
- [CSS Highlight，用 CSS 為文字畫上底線 - 工作玩樂實驗室](https://cola.workxplay.net/css-highlight-text/)
- [HTML mark Tag](https://www.w3schools.com/tags/tag_mark.asp)
- [html - Transparent CSS background color - Stack Overflow](https://stackoverflow.com/questions/11184117/transparent-css-background-color)
- [CSS Colors](https://www.w3schools.com/css/css3_colors.asp)

---

## [1.4.0] - 2022-02-19

### checked

- [Convertkit](https://app.convertkit.com/users/login) 設定電子報、[YAML] 隱藏 Tag 文章

```
collections:
/:
permalink: /{slug}/
template: index
filter: tag:-tagiwanttofilter+tag:-hash-tagiwanttofilter2
```

### reference

- [Hide specific articles tagged with a specific tag - Developer help / Routing - Ghost Forum](https://forum.ghost.org/t/hide-specific-articles-tagged-with-a-specific-tag/21524/4)
- [Tutorial: Building content collections with Ghost](https://ghost.org/docs/tutorials/creating-content-collections/)
- [Ghost Themes - Dynamic URLs & Routing](https://ghost.org/docs/themes/routing/)

---

## [1.3.0] - 2022-02-16

### checked

- 安裝 [hotjar](https://www.hotjar.com/)

---

## [1.2.0] - 2022-01-02

### checked

- 增加 subdomain

### reference

- [Subdomain－子網域、次網域 | dcplus 數位行銷實戰家](https://blog.dcplus.com.tw/marketing-knowledge/trend/26399)

---

## [1.1.2] - 2021-12-26

### modified

- [ HTML/CSS ] 點擊連結另開視窗

### reference

- [Make (All) External Links Open in a New Tab](https://ghost-o-matic.com/make-links-open-in-a-new-tab/)
- [Ghost Blog external links to open in a new tab - Rey Reece](https://www.reyreece.com/posts/ghost-blog-external-links-to-open-in-a-new-tab/)

---

## [1.1.1] - 2021-12-25

### modified

- 換主題 [Edition](https://ghost.org/themes/edition/)

---

## [1.1.0] - 2021-10-25

### checked

- 連接 Google Analytics

### reference

- [GHOST BLOG 加入 GA 分析和 FB 留言](https://yuwenit.ghost.io/ghost-ga-fbcomment/)

---

## [1.0.2] - 2021-10-24

### modified

- 設定主題 Dawn 淺色/深色模式

### reference

- [How I Moved To Ghost 3 (And Made Ghost Dawn Dark-Mode Only)](https://blog.neigor.me/migration-to-ghost-3/#tweaking-ghost-dawn-theme)

---

## [1.0.1] - 2021-10-18

### modified

- [ HTML/CSS ] 時間軸、Youtube 播放介面

### reference

- [Create page template with timeline - Developer help - Ghost Forum](https://forum.ghost.org/t/create-page-template-with-timeline/13172)
- [Lite YouTube Embeds - A Better Method for Embedding YouTube Videos on your Website - Digital Inspiration](https://www.labnol.org/internet/light-youtube-embeds/27941/#embed-youtube-videos-responsively---tutorial)

---

## [1.0.0] - 2021-10-17

### checked

- 購買網域，Google Domains 網域年費為 12 鎂，最低購買 1 年起，最高可以購買 9 年，年數越高並不會降低費用

### reference

- [在 Google Domains 註冊購買網域名稱教學](https://free.com.tw/google-domains/)
- [Google Domains 台灣可以使用了﹍購買 + 轉移網域(Godaddy) + DNS 設定心得＠WFU BLOG](https://www.wfublog.com/2019/04/google-domains-tw-purchase-transfer-godaddy-dns.html)

---

## [0.0.0] - 2021-10-12

### checked

- 註冊 Ghost (Pro)