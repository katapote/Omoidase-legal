---
title: 保存の練習ページ
---
# このページを保存してみましょう

Omoidase への保存を、このページで練習できます。

## 手順

**1. 画面の右下にある「…」をタップ**

点が3つ並んだボタンです。画面の下でゆれている矢印のすぐ下にあります。

**2. メニューの中の「共有」をタップ**

**四角から上向きの矢印が出ているアイコン**です。

**3. 表示された一覧から「Omoidase」を選ぶ**

見つからない場合は、一覧を横にスクロールするか、一番下の「その他」から探してください。

**4. 保存画面が開いたら「保存」をタップ**

これで完了です。AIが自動でこのページを要約し、タグを付けます。

## 保存できたら

Omoidase に戻ると、ホームに **「〇〇で探す」** というボタンが出ます。押してみてください。

「これですか？」と、いま保存したこのページが出てくるはずです。

これが Omoidase の使い方のすべてです。あとは、気になったページを見つけるたびに手順1〜4を繰り返すだけ。覚えておく必要はありません。

## 次から2タップにする（おすすめ）

共有メニューの一覧を左へスクロールして **「その他」→ 右上の「編集」** を開き、Omoidase の **「＋」** を押してください。「よく使う項目」に入り、次からは一覧の先頭に出ます。

## うまくいかないときは

共有メニューに Omoidase が出てこない場合は、一覧の一番右にある「その他」(または「アクションを編集」)をタップし、Omoidase をオンにしてください。一度オンにすれば、次回からは一覧に表示されます。

---

[サポート](./support) ・ [プライバシーポリシー](./privacy-policy) ・ [利用規約](./terms-of-service)

<style>
@keyframes omoidase-point {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(12px); }
}
.omoidase-share-pointer {
  position: fixed;
  right: 10px;
  bottom: 58px;
  z-index: 9999;
  pointer-events: none;
  text-align: right;
  animation: omoidase-point 1.2s ease-in-out infinite;
}
.omoidase-share-pointer .label {
  display: inline-block;
  background: #0969da;
  color: #ffffff;
  font-weight: bold;
  font-size: 15px;
  padding: 8px 14px;
  border-radius: 999px;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.25);
}
.omoidase-share-pointer .arrow {
  font-size: 34px;
  line-height: 1.1;
  padding-right: 16px;
  filter: drop-shadow(0 1px 3px rgba(0, 0, 0, 0.3));
}
</style>
<div class="omoidase-share-pointer">
  <span class="label">この下の「…」をタップ</span>
  <div class="arrow">⬇️</div>
</div>
