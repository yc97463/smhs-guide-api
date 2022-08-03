# 如何嵌入公告小工具？

## 取得公告模組編號

首先，打開校網首頁（或放置公告模組之頁面），接著點選指定公告模組的「更多」。

> <img width="50%" alt="image" src="https://user-images.githubusercontent.com/53697217/182557322-9c1f4106-808e-41b1-abad-620e2ac4e98d.png">

抄寫網址中的模組編號（如圖）。

> <img width="50%" alt="image" src="https://user-images.githubusercontent.com/53697217/182557340-abee0086-36d2-44ce-8e9d-fbfe0a1eb54b.png">

## 嵌入網站

### Google 協作平台

打開 Google 協作平台編輯頁面。

> <img width="50%" alt="image" src="https://user-images.githubusercontent.com/53697217/182557919-8220de70-1ca4-466f-83f4-8ea73623e34a.png">

接著選擇右側選單的「內嵌」功能。

> <img width="50%" alt="image" src="https://user-images.githubusercontent.com/53697217/182559092-0cfdd0af-3a90-4af1-b83b-2e207c072d55.png">



接著貼上 `https://smhsguide-api.dstw.dev/pages/school-announcement?rcg=<模組編號>`，`<模組編號>` 請替換成上方抄寫的資訊。

> <img width="50%" alt="image" src="https://user-images.githubusercontent.com/53697217/182557731-01210e22-0515-4fcf-85f1-278596e1d23c.png">

拉伸區塊高度即完成嵌入公告。

> <img width="50%" alt="image" src="https://user-images.githubusercontent.com/53697217/182557794-0aedde71-d7b6-43c6-b249-47912c84d6e1.png">

### iframe 小工具

請在您的網站中，貼上以下程式碼。`<模組編號>` 請替換成上方抄寫的資訊。

```html
<iframe src="https://smhsguide-api.dstw.dev/pages/school-announcement?rcg=<模組編號>" width="125px" height="150px"></iframe>
```

## 特別感謝

@liaojason2 協助修正 Cloudflare Workers 存取 CORS。