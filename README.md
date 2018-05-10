# 水

用地圖查詢得知某地址或現在位置的供水淨水廠、水來源河川，及水庫水質狀態。以視覺地圖資訊方式呈現水質狀況情報。

[投影片](https://docs.google.com/presentation/d/1XDSWULSKJjudGcbf2JlQGJ6JXryI8gyk69IWpmX278Y/edit#slide=id.p) [hackpad](https://hackpad.tw/--jBgwNkPTdiW)

## 緣由

沒有人參加[第 30 次的 g0v 黑客松](https://beta.hackfoldr.org/g0v-hackath30n)所看到這個題目後，想跳進來看看能不能做點什麼事情。

## 資料來源

1. [ ] [台灣自來水公司供水轄區資訊](https://data.gov.tw/dataset/36602)

## Project Initial Steps

Create PWA tempalte:

``` bash
$ vue init nuxt-community/pwa-template water.g0v.tw

? Project name water.g0v.tw
? Project description Taiwan Water
? Author Yi-Hua Liang <yihua1218@gmail.com>

   vue-cli · Generated "water.g0v.tw".

   To get started:

     cd water.g0v.tw
     npm install # Or yarn
     npm run dev
```

Set development web server port number, edit package.json

``` json
  ...
  ...
  ...
  "config": {
    "nuxt": {
      "port": "3008"
    }
  }
  ...
  ...
  ...
```

Start local development static web server:

``` bash
$ yarn dev
```

Install nuxt-google-maps-module, edit nuxt.config.js

```
$ yarn add vue2-google-maps
```

``` javascript
  ...
  ...
  ...

  ...
  ...
  ...
```

### Google Cloud Platform

1. Create Project
2. Enable Maps JavaScript API
