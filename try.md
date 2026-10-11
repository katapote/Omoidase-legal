---
title: 保存の練習ページ
---
# このページを保存してみましょう

3回タップするだけです。いま見ているこのページで、そのまま練習できます。

<div class="step"><span class="num">1</span> 画面の右下の <b>「…」</b> をタップ</div>

<img src="./assets/try/step1.png?v=2" alt="Safariの画面右下にある「…」ボタン" class="shot">

<div class="step"><span class="num">2</span> メニューの <b>「共有」</b> をタップ</div>

<img src="./assets/try/step2.png?v=2" alt="メニューのいちばん上にある「共有」" class="shot narrow">

<div class="step"><span class="num">3</span> アイコンの列から <b>「Omoidase」</b> をタップ</div>

<img src="./assets/try/step3.png?v=2" alt="共有メニューのアイコンの列にあるOmoidase" class="shot">

アイコンの列にOmoidaseが見当たらないときは、**列を左へスクロール**して、いちばん右の **「その他」** を押してください。一覧の中にOmoidaseがあります。

<div class="done">✓「保存しました」と出たら完了です。何も押さなくても、自動で閉じます。</div>

## 保存できたら

画面左上の **「◀ Omoidase」** を押して、アプリに戻ってください。ホームに **「〇〇で探す」** というボタンが出ています。

押すと「これですか？」と、いま保存したこのページが出てきます。保存したものを、うろ覚えの言葉で探す。これが Omoidase の使い方のすべてです。

## 次から2タップにする（おすすめ）

手順3のアイコンの列を左へスクロールして **「その他」→ 右上の「編集」** を開き、Omoidase の **「＋」** を押してください。「よく使う項目」に入り、次からは列の先頭に出ます。

## うまくいかないときは

「その他」の一覧にも Omoidase が無いときは、一覧の右上の「編集」から Omoidase をオンにしてください。一度オンにすれば、次からは表示されます。

---

[サポート](./support) ・ [プライバシーポリシー](./privacy-policy) ・ [利用規約](./terms-of-service)

<style>
.step { display:flex; align-items:center; gap:10px; font-size:19px; font-weight:600; margin:28px 0 12px; }
.step .num { flex:none; width:30px; height:30px; border-radius:50%; background:#0969da; color:#fff; display:inline-flex; align-items:center; justify-content:center; font-size:16px; }
img.shot { display:block; width:100%; max-width:440px; border-radius:16px; box-shadow:0 2px 14px rgba(0,0,0,.12); margin:0 0 8px; }
img.shot.narrow { max-width:340px; }
.done { margin:28px 0 8px; padding:14px 16px; border-radius:12px; background:#e7f6ec; color:#1a7f37; font-weight:600; }
</style>
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
<script>
  // Safari folds its toolbar away once the page scrolls, so past the first
  // screen the pointer would aim at nothing and cover the text instead.
  (function () {
    var p = document.querySelector('.omoidase-share-pointer');
    if (!p) return;
    p.style.transition = 'opacity .25s';
    window.addEventListener('scroll', function () {
      p.style.opacity = window.scrollY > 300 ? '0' : '1';
    }, { passive: true });
  })();
</script>
