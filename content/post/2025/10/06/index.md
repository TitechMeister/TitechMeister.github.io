---
title: 
date: 2025-10-06T15:00:15+09:00
archives:
    - 2025-10
    - 2025
tags:
    - 26代
    - 全体
categories: []
draft: false
---
<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>特設ページ</title>
  <style>
    /* ページの基本設定 */
    html, body {
      margin: 0;
      padding: 0;
      height: 100%;
      overflow: hidden; /* スクロールバーを隠す */
    }

    /* 背景GIFの設定 */
    body {
      background-image: url('XFbw.gif');
      background-size: cover;
      background-position: center;
      background-repeat: no-repeat;
      
      /* 中央配置のための設定 (Flexbox) */
      display: flex;
      /* ▼▼▼ 変更点1: 要素を縦に並べるように変更 ▼▼▼ */
      flex-direction: column;
      justify-content: center;
      align-items: center;
    }

    /* 上部に追加する一文のスタイル */
    .top-message {
      /* ▼▼▼ 変更点2: position:absoluteを削除し、marginを追加 ▼▼▼ */
      text-align: center;
      color: white;
      font-size: 24px;
      text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.7);
      margin-bottom: 20px; /*下のボックスとの間に余白を追加*/
    }

    /* 中央のコンテンツエリアの設定 */
    .content-box {
      background-color: rgba(255, 255, 255, 0.8);
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
      text-align: center;
      max-width: 80%;
    }

    /* イラスト画像の設定 */
    .main-illustration {
      max-width: 100%;
      height: 400px;
      margin-bottom: 20px;
    }

    /* テキストのスタイル */
    h1 {
      margin: 0;
      color: #333;
    }
  </style>
</head>
<body>

  <div class="top-message">
    GIVINGCAMNPAIGN特設サイトです。<br>
    票数に応じて飛行距離が伸びるよ！
  </div>

  <div class="content-box">
    <img src="photo-output.jpg" alt="メインイラスト" class="main-illustration">
    
    <h1>現在の飛行距離</h1>
    <p>0m</p>
  </div>

</body>
</html>
