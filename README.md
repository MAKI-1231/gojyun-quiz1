<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>期末考査対策 英語クイズ｜さぼてん英会話</title>
<style>
:root {
  --green:#9fd8b6;
  --deep:#2f6f4f;
  --soft:#f4fff8;
  --pink:#ffdbe7;
  --yellow:#fff2a8;
  --blue:#e8f5ff;
  --ink:#243229;
  --muted:#68776d;
  --line:#d8eadf;
  --danger:#b84a62;
  --ok:#2f7d5c;
}
* { box-sizing:border-box; }
body {
  margin:0;
  font-family:"Hiragino Kaku Gothic ProN","Yu Gothic","Meiryo",system-ui,sans-serif;
  background:
    radial-gradient(circle at 9% 8%, rgba(255,219,231,.78) 0 8rem, transparent 8rem),
    radial-gradient(circle at 88% 16%, rgba(255,242,168,.76) 0 8rem, transparent 8rem),
    radial-gradient(circle at 50% 100%, rgba(159,216,182,.35) 0 14rem, transparent 14rem),
    linear-gradient(160deg,#f8fff9 0%,#fff8fb 58%,#fff9d7 100%);
  color:var(--ink);
  min-height:100vh;
}
.wrap { max-width:1040px; margin:0 auto; padding:22px 16px 34px; }
header {
  background:rgba(255,255,255,.95);
  border:2px solid var(--line);
  border-radius:30px;
  padding:24px 20px;
  box-shadow:0 10px 30px rgba(57,106,78,.12);
  text-align:center;
  position:relative;
  overflow:hidden;
}
header::before { content:"📚"; position:absolute; left:18px; top:18px; font-size:2.5rem; opacity:.20; }
header::after { content:"✏️"; position:absolute; right:18px; bottom:18px; font-size:2.5rem; opacity:.20; }
h1 { margin:0 0 8px; font-size:clamp(2rem,5vw,3.35rem); color:var(--deep); letter-spacing:.04em; font-weight:950; }
.subtitle { font-size:clamp(1.05rem,2.4vw,1.35rem); font-weight:900; color:#4e6658; line-height:1.65; }
.note { margin-top:10px; color:var(--muted); font-size:1rem; line-height:1.7; font-weight:800; }
.heroArt { display:flex; justify-content:center; gap:8px; flex-wrap:wrap; margin:10px 0 0; }
.sticker {
  min-width:130px;
  background:linear-gradient(180deg,#fff 0%,#f6fff9 100%);
  border:2px solid var(--line);
  border-radius:24px;
  padding:11px 13px;
  box-shadow:0 6px 16px rgba(57,106,78,.08);
}
.sticker .emoji { display:block; font-size:1.55rem; line-height:1; margin-bottom:4px; }
.sticker .label { font-size:.95rem; font-weight:950; color:var(--deep); }
.panel {
  margin-top:18px;
  background:rgba(255,255,255,.95);
  border:2px solid var(--line);
  border-radius:28px;
  padding:20px;
  box-shadow:0 8px 24px rgba(57,106,78,.10);
}
.section-title { font-size:1.35rem; font-weight:950; color:var(--deep); margin:0 0 12px; }
.grid { display:grid; grid-template-columns:repeat(auto-fit,minmax(220px,1fr)); gap:12px; }
button,input { font:inherit; }
.modeBtn,.choiceBtn,.startBtn,.subBtn,.tokenBtn,.selectedToken,.smallBtn {
  border:2px solid var(--line);
  background:#fff;
  border-radius:22px;
  padding:16px 14px;
  cursor:pointer;
  font-weight:950;
  color:var(--ink);
  transition:.15s transform,.15s box-shadow,.15s background,.15s border-color;
}
.modeBtn { min-height:92px; font-size:1.12rem; line-height:1.45; }
.modeIcon { display:block; font-size:1.75rem; line-height:1; margin-bottom:6px; }
.choiceBtn {
  min-height:78px;
  font-size:clamp(1.3rem,3.7vw,1.9rem);
  text-align:left;
  line-height:1.35;
}
.choiceBtn b,.question b { font-weight:950; }
.modeBtn:hover,.choiceBtn:hover,.startBtn:hover,.subBtn:hover,.tokenBtn:hover,.smallBtn:hover {
  transform:translateY(-1px);
  box-shadow:0 8px 18px rgba(47,111,79,.16);
}
.selected { background:var(--soft); border-color:var(--green); color:var(--deep); }
.startBtn {
  display:block; width:100%; margin-top:18px;
  background:var(--deep); color:#fff; border-color:var(--deep);
  font-size:1.35rem; padding:18px;
}
.subBtn { background:var(--yellow); border-color:#eed66d; font-size:1.15rem; }
.topline { display:flex; gap:10px; flex-wrap:wrap; align-items:center; justify-content:space-between; margin-bottom:14px; }
.badge {
  display:inline-flex; align-items:center; gap:6px;
  background:var(--soft); border:2px solid var(--line); color:var(--deep);
  border-radius:999px; padding:9px 13px; font-weight:950; font-size:1rem;
}
.questionBox {
  border-radius:26px;
  border:2px solid var(--line);
  padding:26px 18px;
  background:#fff;
  text-align:center;
  position:relative;
  overflow:hidden;
}
.questionBox::before,.questionBox::after { position:absolute; font-size:2rem; opacity:.16; }
.questionBox::before { content:"🔎"; top:10px; left:14px; }
.questionBox::after { content:"🌵"; right:14px; bottom:10px; }
.qLabel { color:var(--muted); font-weight:900; font-size:1.08rem; margin-bottom:10px; }
.question {
  font-size:clamp(1.85rem,6.2vw,3.55rem);
  line-height:1.25;
  font-weight:950;
  color:var(--deep);
  word-break:keep-all;
}
.question.ja { font-size:clamp(1.55rem,5.6vw,3rem); color:#37463d; }
.options { display:grid; gap:12px; margin-top:16px; }
.tokenArea {
  display:flex;
  gap:10px;
  flex-wrap:wrap;
  padding:14px;
  border:2px dashed var(--line);
  border-radius:22px;
  background:#fbfffc;
  min-height:76px;
  margin-top:14px;
}
.answerArea {
  background:var(--blue);
  border-color:#cfe6f6;
}
.tokenBtn,.selectedToken {
  padding:12px 14px;
  font-size:clamp(1.05rem,3.2vw,1.45rem);
  border-radius:18px;
}
.selectedToken { background:#fff; border-color:#b9dceb; }
.smallRow { display:flex; gap:10px; flex-wrap:wrap; margin-top:12px; }
.smallBtn { padding:12px 16px; background:#fff; font-size:1.05rem; }
.inputRow { display:flex; gap:10px; margin-top:18px; flex-wrap:wrap; }
.spellInput {
  flex:1 1 320px;
  border:3px solid var(--line);
  border-radius:22px;
  padding:16px 18px;
  font-size:clamp(1.45rem,4vw,2.25rem);
  font-weight:950;
  background:#fff;
}
.checkBtn {
  flex:0 0 auto;
  border:0;
  background:var(--deep);
  color:#fff;
  border-radius:22px;
  padding:16px 24px;
  font-size:1.25rem;
  font-weight:950;
  cursor:pointer;
}
.feedback {
  min-height:50px;
  margin-top:14px;
  padding:12px 14px;
  border-radius:20px;
  font-size:1.15rem;
  font-weight:950;
  line-height:1.5;
}
.ok { background:#e8fff1; color:var(--ok); border:2px solid #b9e7ca; }
.ng { background:#fff0f4; color:var(--danger); border:2px solid #ffd1dc; }
.result { text-align:center; padding:28px 14px; }
.score { font-size:clamp(2.2rem,8vw,4.5rem); color:var(--deep); font-weight:950; margin:10px 0; }
.message {
  font-size:clamp(1.32rem,4vw,2rem);
  font-weight:950;
  line-height:1.6;
  background:var(--soft);
  border:2px solid var(--line);
  padding:18px;
  border-radius:24px;
  margin:16px 0;
}
.review { text-align:left; margin-top:16px; display:grid; gap:8px; }
.reviewItem { background:#fff; border:1px solid var(--line); border-radius:18px; padding:10px 12px; font-size:1rem; line-height:1.5; }
.hidden { display:none !important; }
.nextBtn {
  display:block;
  width:100%;
  margin-top:10px;
  border:0;
  background:var(--deep);
  color:#fff;
  border-radius:20px;
  padding:15px 18px;
  font-size:1.25rem;
  font-weight:950;
  cursor:pointer;
}
footer { text-align:center; color:#6b7b70; margin-top:20px; font-weight:900; font-size:.95rem; }
@media (min-width:760px) { .options { grid-template-columns:1fr 1fr; } }
@media (max-width:520px) {
  .wrap { padding:8px 8px 18px; }
  header { border-radius:18px; padding:12px 10px; }
  header::before, header::after { display:none; }
  h1 { font-size:1.55rem; line-height:1.25; margin-bottom:4px; }
  .subtitle { font-size:.95rem; line-height:1.4; }
  .heroArt { display:none; }
  .panel { border-radius:18px; padding:12px; margin-top:10px; }
  .section-title { font-size:1.08rem; margin-bottom:8px; }
  .grid { gap:8px; }
  .modeBtn { min-height:64px; padding:10px 8px; font-size:.98rem; border-radius:16px; }
  .modeIcon { display:inline; font-size:1.05rem; margin-right:4px; }
  .topline { gap:6px; margin-bottom:8px; }
  .badge { padding:6px 9px; font-size:.86rem; }
  .questionBox { padding:16px 12px; border-radius:18px; }
  .questionBox::before, .questionBox::after { display:none; }
  .qLabel { font-size:.92rem; margin-bottom:6px; }
  .question { font-size:1.55rem; line-height:1.3; }
  .question.ja { font-size:1.35rem; line-height:1.35; }
  .options { gap:8px; margin-top:10px; }
  .choiceBtn { min-height:56px; padding:11px 12px; font-size:1.08rem; border-radius:16px; }
  .tokenArea { gap:7px; padding:9px; min-height:50px; margin-top:8px; border-radius:16px; }
  .tokenBtn, .selectedToken { padding:9px 10px; font-size:1rem; border-radius:14px; }
  .smallRow { gap:8px; margin-top:8px; }
  .smallBtn { padding:10px 12px; font-size:.95rem; border-radius:14px; }
  .checkBtn { width:100%; padding:12px 16px; border-radius:16px; font-size:1.05rem; }
  .feedback { min-height:auto; margin-top:8px; padding:9px 10px; border-radius:14px; font-size:1rem; }
  .nextBtn { margin-top:8px; padding:12px 16px; border-radius:16px; font-size:1.08rem; }
  .score { font-size:2.3rem; margin:6px 0; }
  .message { font-size:1.08rem; padding:12px; border-radius:16px; margin:10px 0; }
  .reviewItem { font-size:.92rem; padding:8px 10px; }
}
</style>
</head>
<body>
<div class="wrap">
  <header>
    <h1>期末考査対策<br>英語クイズ</h1>
    <div class="subtitle">単語・熟語・重要文を10問ずつ練習</div>
    <div class="heroArt">
      <div class="sticker"><span class="emoji">📘</span><span class="label">単語・熟語</span></div>
      <div class="sticker"><span class="emoji">🧩</span><span class="label">並べ替え</span></div>
      <div class="sticker"><span class="emoji">✏️</span><span class="label">穴埋め</span></div>
    </div>
    
  </header>

  <main>
    <section id="setup" class="panel">
      <p class="section-title">練習メニューを選んでください</p>
      <div class="grid" id="modeGrid">
        <button class="modeBtn selected" data-mode="all"><span class="modeIcon">🎲</span>ぜんぶランダム<br><small>3種類から出題</small></button>
        <button class="modeBtn" data-mode="vocab"><span class="modeIcon">📘</span>単語・熟語<br><small>英語⇄日本語 4択</small></button>
        <button class="modeBtn" data-mode="reorder"><span class="modeIcon">🧩</span>重要文ならべ替え<br><small>語順を作る</small></button>
        <button class="modeBtn" data-mode="cloze"><span class="modeIcon">✏️</span>穴埋め<br><small>重要ポイント</small></button>
      </div>
      <button class="startBtn" id="startBtn">10問スタート</button>
    </section>

    <section id="quiz" class="panel hidden">
      <div class="topline">
        <span class="badge" id="progressBadge">1 / 10</span>
        <span class="badge" id="modeBadge">ぜんぶランダム</span>
        <span class="badge" id="scoreBadge">正解 0</span>
      </div>
      <div class="questionBox">
        <div class="qLabel" id="qLabel">意味を選びましょう</div>
        <div class="question" id="questionText">because</div>
      </div>

      <div id="options" class="options"></div>

      <div id="reorderArea" class="hidden">
        <p class="qLabel" style="margin-top:16px;">答え</p>
        <div id="answerArea" class="tokenArea answerArea"></div>
        <p class="qLabel" style="margin-top:14px;">語句カード</p>
        <div id="wordBank" class="tokenArea"></div>
        <div class="smallRow">
          <button class="smallBtn" id="undoBtn">1つ戻す</button>
          <button class="smallBtn" id="clearBtn">やり直す</button>
          <button class="checkBtn" id="checkOrderBtn">答える</button>
        </div>
      </div>

      <div id="feedback" class="feedback hidden"></div>
      <button class="nextBtn hidden" id="nextBtn">次へ</button>
    </section>

    <section id="result" class="panel hidden">
      <div class="result">
        <p class="section-title">おつかれさまでした！</p>
        <div class="score" id="finalScore">8 / 10</div>
        <div class="message" id="resultMessage">すばらしい集中力です。</div>
        <button class="startBtn" id="againBtn">もう一度10問</button>
        <button class="subBtn" id="backBtn" style="margin-top:12px; width:100%;">メニューを選び直す</button>
        <div class="review" id="review"></div>
      </div>
    </section>
  </main>
  <footer>© 2026 さぼてん英会話</footer>
</div>

<script>
const DATA = {"vocab": [{"en": "through", "ja": "〜を通して", "kind": "単語", "type": "vocab", "id": "V001"}, {"en": "event", "ja": "行事／イベント", "kind": "単語", "type": "vocab", "id": "V002"}, {"en": "expo", "ja": "博覧会", "kind": "単語", "type": "vocab", "id": "V003"}, {"en": "introduce", "ja": "〜を紹介する", "kind": "単語", "type": "vocab", "id": "V004"}, {"en": "aspect", "ja": "側面", "kind": "単語", "type": "vocab", "id": "V005"}, {"en": "fashion", "ja": "ファッション", "kind": "単語", "type": "vocab", "id": "V006"}, {"en": "traditional", "ja": "伝統的な", "kind": "単語", "type": "vocab", "id": "V007"}, {"en": "foreign", "ja": "外国の", "kind": "単語", "type": "vocab", "id": "V008"}, {"en": "native", "ja": "出生地の／在来の", "kind": "単語", "type": "vocab", "id": "V009"}, {"en": "project", "ja": "企画／プロジェクト", "kind": "単語", "type": "vocab", "id": "V010"}, {"en": "present", "ja": "〜を発表する／提供する", "kind": "単語", "type": "vocab", "id": "V011"}, {"en": "excellent", "ja": "優れた", "kind": "単語", "type": "vocab", "id": "V012"}, {"en": "topic", "ja": "話題／主題", "kind": "単語", "type": "vocab", "id": "V013"}, {"en": "information", "ja": "情報", "kind": "単語", "type": "vocab", "id": "V014"}, {"en": "classmate", "ja": "同級生", "kind": "単語", "type": "vocab", "id": "V015"}, {"en": "culture", "ja": "文化", "kind": "単語", "type": "vocab", "id": "V016"}, {"en": "difference", "ja": "違い", "kind": "単語", "type": "vocab", "id": "V017"}, {"en": "uniform", "ja": "制服", "kind": "単語", "type": "vocab", "id": "V018"}, {"en": "hairstyle", "ja": "髪型", "kind": "単語", "type": "vocab", "id": "V019"}, {"en": "charm", "ja": "お守り", "kind": "単語", "type": "vocab", "id": "V020"}, {"en": "magazine", "ja": "雑誌", "kind": "単語", "type": "vocab", "id": "V021"}, {"en": "temple", "ja": "寺", "kind": "単語", "type": "vocab", "id": "V022"}, {"en": "smartphone", "ja": "スマートフォン", "kind": "単語", "type": "vocab", "id": "V023"}, {"en": "although", "ja": "〜だけれども", "kind": "単語", "type": "vocab", "id": "V024"}, {"en": "though", "ja": "〜だけれども", "kind": "単語", "type": "vocab", "id": "V025"}, {"en": "if", "ja": "もし〜なら", "kind": "単語", "type": "vocab", "id": "V026"}, {"en": "because", "ja": "〜だから", "kind": "単語", "type": "vocab", "id": "V027"}, {"en": "that", "ja": "〜ということ", "kind": "単語", "type": "vocab", "id": "V028"}, {"en": "chance", "ja": "機会", "kind": "単語", "type": "vocab", "id": "V029"}, {"en": "step", "ja": "一歩／段階", "kind": "単語", "type": "vocab", "id": "V030"}, {"en": "experience", "ja": "経験", "kind": "単語", "type": "vocab", "id": "V031"}, {"en": "worried", "ja": "心配して", "kind": "単語", "type": "vocab", "id": "V032"}, {"en": "alone", "ja": "ひとりで", "kind": "単語", "type": "vocab", "id": "V033"}, {"en": "agree", "ja": "賛成する／一致する", "kind": "単語", "type": "vocab", "id": "V034"}, {"en": "mix", "ja": "〜を混ぜる", "kind": "単語", "type": "vocab", "id": "V035"}, {"en": "examination", "ja": "試験", "kind": "単語", "type": "vocab", "id": "V036"}, {"en": "non-native", "ja": "外来の", "kind": "単語", "type": "vocab", "id": "V037"}, {"en": "species", "ja": "種／生物の種類", "kind": "単語", "type": "vocab", "id": "V038"}, {"en": "create", "ja": "〜を作り出す／引き起こす", "kind": "単語", "type": "vocab", "id": "V039"}, {"en": "harmful", "ja": "有害な", "kind": "単語", "type": "vocab", "id": "V040"}, {"en": "activity", "ja": "活動", "kind": "単語", "type": "vocab", "id": "V041"}, {"en": "accident", "ja": "偶然の出来事", "kind": "単語", "type": "vocab", "id": "V042"}, {"en": "purpose", "ja": "目的", "kind": "単語", "type": "vocab", "id": "V043"}, {"en": "original", "ja": "本来の／元の", "kind": "単語", "type": "vocab", "id": "V044"}, {"en": "European", "ja": "ヨーロッパの", "kind": "単語", "type": "vocab", "id": "V045"}, {"en": "rabbit", "ja": "ウサギ", "kind": "単語", "type": "vocab", "id": "V046"}, {"en": "settler", "ja": "入植者", "kind": "単語", "type": "vocab", "id": "V047"}, {"en": "wild", "ja": "野生の", "kind": "単語", "type": "vocab", "id": "V048"}, {"en": "hunt", "ja": "狩る", "kind": "単語", "type": "vocab", "id": "V049"}, {"en": "survive", "ja": "生き残る", "kind": "単語", "type": "vocab", "id": "V050"}, {"en": "crop", "ja": "作物", "kind": "単語", "type": "vocab", "id": "V051"}, {"en": "million", "ja": "百万", "kind": "単語", "type": "vocab", "id": "V052"}, {"en": "island", "ja": "島", "kind": "単語", "type": "vocab", "id": "V053"}, {"en": "forest", "ja": "森／森林", "kind": "単語", "type": "vocab", "id": "V054"}, {"en": "disappear", "ja": "姿を消す", "kind": "単語", "type": "vocab", "id": "V055"}, {"en": "completely", "ja": "完全に", "kind": "単語", "type": "vocab", "id": "V056"}, {"en": "scientist", "ja": "科学者", "kind": "単語", "type": "vocab", "id": "V057"}, {"en": "government", "ja": "政府", "kind": "単語", "type": "vocab", "id": "V058"}, {"en": "reduce", "ja": "〜を減らす", "kind": "単語", "type": "vocab", "id": "V059"}, {"en": "environment", "ja": "環境", "kind": "単語", "type": "vocab", "id": "V060"}, {"en": "choice", "ja": "選択", "kind": "単語", "type": "vocab", "id": "V061"}, {"en": "future", "ja": "未来／将来", "kind": "単語", "type": "vocab", "id": "V062"}, {"en": "impact", "ja": "影響", "kind": "単語", "type": "vocab", "id": "V063"}, {"en": "miso soup", "ja": "みそ汁", "kind": "単語", "type": "vocab", "id": "V064"}, {"en": "rice ball", "ja": "おにぎり", "kind": "単語", "type": "vocab", "id": "V065"}, {"en": "tofu", "ja": "豆腐", "kind": "単語", "type": "vocab", "id": "V066"}, {"en": "salmon", "ja": "サーモン", "kind": "単語", "type": "vocab", "id": "V067"}, {"en": "bagel", "ja": "ベーグル", "kind": "単語", "type": "vocab", "id": "V068"}, {"en": "flight", "ja": "飛行機の便／フライト", "kind": "単語", "type": "vocab", "id": "V069"}, {"en": "nervous", "ja": "緊張した／不安な", "kind": "単語", "type": "vocab", "id": "V070"}, {"en": "excited", "ja": "わくわくしている", "kind": "単語", "type": "vocab", "id": "V071"}, {"en": "advice", "ja": "助言", "kind": "単語", "type": "vocab", "id": "V072"}, {"en": "useful", "ja": "役に立つ", "kind": "単語", "type": "vocab", "id": "V073"}, {"en": "smile", "ja": "笑顔／ほほえむ", "kind": "単語", "type": "vocab", "id": "V074"}, {"en": "favorite", "ja": "お気に入りの", "kind": "単語", "type": "vocab", "id": "V075"}, {"en": "sleepy", "ja": "眠い", "kind": "単語", "type": "vocab", "id": "V076"}, {"en": "flute", "ja": "フルート", "kind": "単語", "type": "vocab", "id": "V077"}, {"en": "tomato", "ja": "トマト", "kind": "単語", "type": "vocab", "id": "V078"}, {"en": "yummy", "ja": "おいしい", "kind": "単語", "type": "vocab", "id": "V079"}, {"en": "uncle", "ja": "おじ", "kind": "単語", "type": "vocab", "id": "V080"}, {"en": "aunt", "ja": "おば", "kind": "単語", "type": "vocab", "id": "V081"}, {"en": "adventure", "ja": "冒険", "kind": "単語", "type": "vocab", "id": "V082"}, {"en": "author", "ja": "作家", "kind": "単語", "type": "vocab", "id": "V083"}, {"en": "character", "ja": "登場人物／性格", "kind": "単語", "type": "vocab", "id": "V084"}, {"en": "novel", "ja": "小説", "kind": "単語", "type": "vocab", "id": "V085"}, {"en": "imagination", "ja": "想像力", "kind": "単語", "type": "vocab", "id": "V086"}, {"en": "not only A but also B", "ja": "AだけでなくBも", "kind": "熟語・表現", "type": "vocab", "id": "V087"}, {"en": "both A and B", "ja": "AもBも両方とも", "kind": "熟語・表現", "type": "vocab", "id": "V088"}, {"en": "work on", "ja": "〜に取り組む", "kind": "熟語・表現", "type": "vocab", "id": "V089"}, {"en": "look up", "ja": "〜を調べる", "kind": "熟語・表現", "type": "vocab", "id": "V090"}, {"en": "learn about", "ja": "〜について学ぶ", "kind": "熟語・表現", "type": "vocab", "id": "V091"}, {"en": "for example", "ja": "たとえば", "kind": "熟語・表現", "type": "vocab", "id": "V092"}, {"en": "such as", "ja": "〜のような", "kind": "熟語・表現", "type": "vocab", "id": "V093"}, {"en": "be interested in", "ja": "〜に興味がある", "kind": "熟語・表現", "type": "vocab", "id": "V094"}, {"en": "make a video", "ja": "動画を作る", "kind": "熟語・表現", "type": "vocab", "id": "V095"}, {"en": "present it to the class", "ja": "それをクラスで発表する", "kind": "熟語・表現", "type": "vocab", "id": "V096"}, {"en": "school rule", "ja": "校則", "kind": "熟語・表現", "type": "vocab", "id": "V097"}, {"en": "of course", "ja": "もちろん", "kind": "熟語・表現", "type": "vocab", "id": "V098"}, {"en": "in English", "ja": "英語で", "kind": "熟語・表現", "type": "vocab", "id": "V099"}, {"en": "at school", "ja": "学校で", "kind": "熟語・表現", "type": "vocab", "id": "V100"}, {"en": "What a nice day!", "ja": "なんてすてきな日でしょう", "kind": "熟語・表現", "type": "vocab", "id": "V101"}, {"en": "How beautiful!", "ja": "なんて美しいのでしょう", "kind": "熟語・表現", "type": "vocab", "id": "V102"}, {"en": "Shall I ...?", "ja": "私が〜しましょうか", "kind": "熟語・表現", "type": "vocab", "id": "V103"}, {"en": "Shall we ...?", "ja": "一緒に〜しましょうか", "kind": "熟語・表現", "type": "vocab", "id": "V104"}, {"en": "Will you ...?", "ja": "〜してくれますか", "kind": "熟語・表現", "type": "vocab", "id": "V105"}, {"en": "have to", "ja": "〜しなければならない", "kind": "熟語・表現", "type": "vocab", "id": "V106"}, {"en": "don't have to", "ja": "〜する必要はない", "kind": "熟語・表現", "type": "vocab", "id": "V107"}, {"en": "must not", "ja": "〜してはいけない", "kind": "熟語・表現", "type": "vocab", "id": "V108"}, {"en": "need to", "ja": "〜する必要がある", "kind": "熟語・表現", "type": "vocab", "id": "V109"}, {"en": "on time", "ja": "時間通りに", "kind": "熟語・表現", "type": "vocab", "id": "V110"}, {"en": "stop by", "ja": "〜に立ち寄る", "kind": "熟語・表現", "type": "vocab", "id": "V111"}, {"en": "in a hurry", "ja": "急いで", "kind": "熟語・表現", "type": "vocab", "id": "V112"}, {"en": "write out", "ja": "書き出す", "kind": "熟語・表現", "type": "vocab", "id": "V113"}, {"en": "go well", "ja": "うまくいく", "kind": "熟語・表現", "type": "vocab", "id": "V114"}, {"en": "non-native species", "ja": "外来種", "kind": "熟語・表現", "type": "vocab", "id": "V115"}, {"en": "because of", "ja": "〜のために", "kind": "熟語・表現", "type": "vocab", "id": "V116"}, {"en": "by accident", "ja": "偶然に", "kind": "熟語・表現", "type": "vocab", "id": "V117"}, {"en": "on purpose", "ja": "わざと／意図的に", "kind": "熟語・表現", "type": "vocab", "id": "V118"}, {"en": "take the place of", "ja": "〜に取って代わる", "kind": "熟語・表現", "type": "vocab", "id": "V119"}, {"en": "more than", "ja": "〜を超える", "kind": "熟語・表現", "type": "vocab", "id": "V120"}, {"en": "most of", "ja": "〜のほとんど", "kind": "熟語・表現", "type": "vocab", "id": "V121"}, {"en": "the number of", "ja": "〜の数", "kind": "熟語・表現", "type": "vocab", "id": "V122"}, {"en": "die out", "ja": "絶滅する", "kind": "熟語・表現", "type": "vocab", "id": "V123"}, {"en": "play an important role", "ja": "重要な役割を果たす", "kind": "熟語・表現", "type": "vocab", "id": "V124"}, {"en": "in some cases", "ja": "場合によっては", "kind": "熟語・表現", "type": "vocab", "id": "V125"}, {"en": "in danger", "ja": "危険にさらされて", "kind": "熟語・表現", "type": "vocab", "id": "V126"}, {"en": "natural environment", "ja": "自然環境", "kind": "熟語・表現", "type": "vocab", "id": "V127"}, {"en": "as carefully as we can", "ja": "できる限り慎重に", "kind": "熟語・表現", "type": "vocab", "id": "V128"}, {"en": "It smells good.", "ja": "いいにおいがします。", "kind": "熟語・表現", "type": "vocab", "id": "V129"}, {"en": "It sounds yummy.", "ja": "おいしそうです。", "kind": "熟語・表現", "type": "vocab", "id": "V130"}, {"en": "stay with", "ja": "〜の家に泊まる／滞在する", "kind": "熟語・表現", "type": "vocab", "id": "V131"}, {"en": "for breakfast", "ja": "朝食に", "kind": "熟語・表現", "type": "vocab", "id": "V132"}, {"en": "put A in B", "ja": "AをBに入れる", "kind": "熟語・表現", "type": "vocab", "id": "V133"}, {"en": "Here you are.", "ja": "はい、どうぞ。", "kind": "熟語・表現", "type": "vocab", "id": "V134"}, {"en": "Me, too.", "ja": "私もです。", "kind": "熟語・表現", "type": "vocab", "id": "V135"}, {"en": "buy A for B", "ja": "BのためにAを買う", "kind": "熟語・表現", "type": "vocab", "id": "V136"}, {"en": "thanks to", "ja": "〜のおかげで", "kind": "熟語・表現", "type": "vocab", "id": "V137"}, {"en": "make me happy", "ja": "私を幸せにする", "kind": "熟語・表現", "type": "vocab", "id": "V138"}, {"en": "give me advice", "ja": "私に助言をくれる", "kind": "熟語・表現", "type": "vocab", "id": "V139"}, {"en": "send me a message", "ja": "私にメッセージを送る", "kind": "熟語・表現", "type": "vocab", "id": "V140"}, {"en": "show me your notebook", "ja": "私にあなたのノートを見せる", "kind": "熟語・表現", "type": "vocab", "id": "V141"}, {"en": "tell me the truth", "ja": "私に本当のことを話す", "kind": "熟語・表現", "type": "vocab", "id": "V142"}, {"en": "teach me English", "ja": "私に英語を教える", "kind": "熟語・表現", "type": "vocab", "id": "V143"}, {"en": "ask me a question", "ja": "私に質問をする", "kind": "熟語・表現", "type": "vocab", "id": "V144"}, {"en": "buy me a ticket", "ja": "私にチケットを買ってくれる", "kind": "熟語・表現", "type": "vocab", "id": "V145"}, {"en": "make me lunch", "ja": "私に昼食を作ってくれる", "kind": "熟語・表現", "type": "vocab", "id": "V146"}, {"en": "keep the room clean", "ja": "部屋をきれいに保つ", "kind": "熟語・表現", "type": "vocab", "id": "V147"}, {"en": "leave the door open", "ja": "ドアを開けたままにする", "kind": "熟語・表現", "type": "vocab", "id": "V148"}, {"en": "call her Maki", "ja": "彼女をマキと呼ぶ", "kind": "熟語・表現", "type": "vocab", "id": "V149"}, {"en": "paint the wall blue", "ja": "壁を青く塗る", "kind": "熟語・表現", "type": "vocab", "id": "V150"}, {"en": "find English useful", "ja": "英語が役に立つとわかる", "kind": "熟語・表現", "type": "vocab", "id": "V151"}], "reorder": [{"type": "reorder", "ja": "私は外国の文化に興味があります。", "answer": "I am interested in foreign cultures.", "tokens": ["I", "am", "interested", "in", "foreign", "cultures."], "group": "接続詞・基本表現", "id": "R001"}, {"type": "reorder", "ja": "私たちは授業でそのトピックについて学びました。", "answer": "We learned about the topic in class.", "tokens": ["We", "learned", "about", "the", "topic", "in", "class."], "group": "接続詞・基本表現", "id": "R002"}, {"type": "reorder", "ja": "彼女はプロジェクトに一生懸命取り組みました。", "answer": "She worked hard on the project.", "tokens": ["She", "worked", "hard", "on", "the", "project."], "group": "接続詞・基本表現", "id": "R003"}, {"type": "reorder", "ja": "時間があれば、私を手伝ってください。", "answer": "If you have time, please help me.", "tokens": ["If", "you", "have", "time,", "please", "help", "me."], "group": "接続詞", "id": "R004"}, {"type": "reorder", "ja": "明日雨が降ったら、私たちは教室で練習します。", "answer": "If it rains tomorrow, we will practice in the classroom.", "tokens": ["If", "it", "rains", "tomorrow,", "we", "will", "practice", "in", "the", "classroom."], "group": "接続詞", "id": "R005"}, {"type": "reorder", "ja": "私は疲れていたので、早く寝ました。", "answer": "I went to bed early because I was tired.", "tokens": ["I", "went", "to", "bed", "early", "because", "I", "was", "tired."], "group": "接続詞", "id": "R006"}, {"type": "reorder", "ja": "彼は忙しかったけれども、私にメッセージを送りました。", "answer": "Although he was busy, he sent me a message.", "tokens": ["Although", "he", "was", "busy,", "he", "sent", "me", "a", "message."], "group": "接続詞", "id": "R007"}, {"type": "reorder", "ja": "その話は長かったけれども、とても面白かったです。", "answer": "Though the story was long, it was very interesting.", "tokens": ["Though", "the", "story", "was", "long,", "it", "was", "very", "interesting."], "group": "接続詞", "id": "R008"}, {"type": "reorder", "ja": "私はこのトピックは私たちにとって重要だと思います。", "answer": "I think that this topic is important for us.", "tokens": ["I", "think", "that", "this", "topic", "is", "important", "for", "us."], "group": "接続詞", "id": "R009"}, {"type": "reorder", "ja": "私は試験がうまくいくことを願っています。", "answer": "I hope that the examination will go well.", "tokens": ["I", "hope", "that", "the", "examination", "will", "go", "well."], "group": "接続詞", "id": "R010"}, {"type": "reorder", "ja": "出かける前に、宿題を終えなさい。", "answer": "Finish your homework before you go out.", "tokens": ["Finish", "your", "homework", "before", "you", "go", "out."], "group": "接続詞", "id": "R011"}, {"type": "reorder", "ja": "私が夕食を作っている間、音楽を聞いていました。", "answer": "I listened to music while I was cooking dinner.", "tokens": ["I", "listened", "to", "music", "while", "I", "was", "cooking", "dinner."], "group": "接続詞", "id": "R012"}, {"type": "reorder", "ja": "なんてすばらしい発表でしょう。", "answer": "What an excellent presentation!", "tokens": ["What", "an", "excellent", "presentation!"], "group": "感嘆文", "id": "R013"}, {"type": "reorder", "ja": "なんて面白いトピックでしょう。", "answer": "What an interesting topic!", "tokens": ["What", "an", "interesting", "topic!"], "group": "感嘆文", "id": "R014"}, {"type": "reorder", "ja": "この写真はなんて美しいのでしょう。", "answer": "How beautiful this picture is!", "tokens": ["How", "beautiful", "this", "picture", "is!"], "group": "感嘆文", "id": "R015"}, {"type": "reorder", "ja": "この考えはなんてわくわくするのでしょう。", "answer": "How exciting this idea is!", "tokens": ["How", "exciting", "this", "idea", "is!"], "group": "感嘆文", "id": "R016"}, {"type": "reorder", "ja": "窓を開けましょうか。", "answer": "Shall I open the window?", "tokens": ["Shall", "I", "open", "the", "window?"], "group": "助動詞表現", "id": "R017"}, {"type": "reorder", "ja": "あなたのかばんを運びましょうか。", "answer": "Shall I carry your bag?", "tokens": ["Shall", "I", "carry", "your", "bag?"], "group": "助動詞表現", "id": "R018"}, {"type": "reorder", "ja": "休憩しましょうか。", "answer": "Shall we take a break?", "tokens": ["Shall", "we", "take", "a", "break?"], "group": "助動詞表現", "id": "R019"}, {"type": "reorder", "ja": "一緒に始めましょうか。", "answer": "Shall we start together?", "tokens": ["Shall", "we", "start", "together?"], "group": "助動詞表現", "id": "R020"}, {"type": "reorder", "ja": "ここで待ってくれますか。", "answer": "Will you wait here?", "tokens": ["Will", "you", "wait", "here?"], "group": "助動詞表現", "id": "R021"}, {"type": "reorder", "ja": "あなたのノートを見せてくれますか。", "answer": "Will you show me your notebook?", "tokens": ["Will", "you", "show", "me", "your", "notebook?"], "group": "助動詞表現", "id": "R022"}, {"type": "reorder", "ja": "私は夕食前にレポートを終えなければなりません。", "answer": "I have to finish my report before dinner.", "tokens": ["I", "have", "to", "finish", "my", "report", "before", "dinner."], "group": "助動詞表現", "id": "R023"}, {"type": "reorder", "ja": "あなたは試験を心配する必要はありません。", "answer": "You do not have to worry about the test.", "tokens": ["You", "do", "not", "have", "to", "worry", "about", "the", "test."], "group": "助動詞表現", "id": "R024"}, {"type": "reorder", "ja": "私たちは自然環境について慎重に考えなければなりません。", "answer": "We have to think carefully about the natural environment.", "tokens": ["We", "have", "to", "think", "carefully", "about", "the", "natural", "environment."], "group": "助動詞表現", "id": "R025"}, {"type": "reorder", "ja": "このスープはいいにおいがします。", "answer": "This soup smells good.", "tokens": ["This", "soup", "smells", "good."], "group": "文のしくみ", "id": "R026"}, {"type": "reorder", "ja": "その考えはよさそうに聞こえます。", "answer": "That idea sounds nice.", "tokens": ["That", "idea", "sounds", "nice."], "group": "文のしくみ", "id": "R027"}, {"type": "reorder", "ja": "彼女は少し緊張しているように見えました。", "answer": "She looked a little nervous.", "tokens": ["She", "looked", "a", "little", "nervous."], "group": "文のしくみ", "id": "R028"}, {"type": "reorder", "ja": "そのニュースは私をうれしくしました。", "answer": "The news made me happy.", "tokens": ["The", "news", "made", "me", "happy."], "group": "文のしくみ", "id": "R029"}, {"type": "reorder", "ja": "部屋をきれいにしておきなさい。", "answer": "Keep the room clean.", "tokens": ["Keep", "the", "room", "clean."], "group": "文のしくみ", "id": "R030"}, {"type": "reorder", "ja": "ドアを開けたままにしないで。", "answer": "Do not leave the door open.", "tokens": ["Do", "not", "leave", "the", "door", "open."], "group": "文のしくみ", "id": "R031"}, {"type": "reorder", "ja": "私たちは彼をケンと呼びます。", "answer": "We call him Ken.", "tokens": ["We", "call", "him", "Ken."], "group": "文のしくみ", "id": "R032"}, {"type": "reorder", "ja": "私は英語が役に立つとわかりました。", "answer": "I found English useful.", "tokens": ["I", "found", "English", "useful."], "group": "文のしくみ", "id": "R033"}, {"type": "reorder", "ja": "彼女は私に助言をくれました。", "answer": "She gave me some advice.", "tokens": ["She", "gave", "me", "some", "advice."], "group": "文のしくみ", "id": "R034"}, {"type": "reorder", "ja": "彼は私にメッセージを送りました。", "answer": "He sent me a message.", "tokens": ["He", "sent", "me", "a", "message."], "group": "文のしくみ", "id": "R035"}, {"type": "reorder", "ja": "私の叔母は私に昼食を作ってくれました。", "answer": "My aunt made me lunch.", "tokens": ["My", "aunt", "made", "me", "lunch."], "group": "文のしくみ", "id": "R036"}, {"type": "reorder", "ja": "先生は私たちに新しい単語を教えました。", "answer": "The teacher taught us a new word.", "tokens": ["The", "teacher", "taught", "us", "a", "new", "word."], "group": "文のしくみ", "id": "R037"}, {"type": "reorder", "ja": "彼は私に真実を話しました。", "answer": "He told me the truth.", "tokens": ["He", "told", "me", "the", "truth."], "group": "文のしくみ", "id": "R038"}, {"type": "reorder", "ja": "私は友だちのためにチケットを買いました。", "answer": "I bought a ticket for my friend.", "tokens": ["I", "bought", "a", "ticket", "for", "my", "friend."], "group": "文のしくみ", "id": "R039"}, {"type": "reorder", "ja": "彼女は私にその写真を見せてくれました。", "answer": "She showed me the picture.", "tokens": ["She", "showed", "me", "the", "picture."], "group": "文のしくみ", "id": "R040"}, {"type": "reorder", "ja": "外来種は在来の動植物に害を与えることがあります。", "answer": "Non-native species can be harmful to native animals and plants.", "tokens": ["Non-native", "species", "can", "be", "harmful", "to", "native", "animals", "and", "plants."], "group": "本文重要文風", "id": "R041"}, {"type": "reorder", "ja": "人間の活動が環境に大きな影響を与えることがあります。", "answer": "Human activity can have a big impact on the environment.", "tokens": ["Human", "activity", "can", "have", "a", "big", "impact", "on", "the", "environment."], "group": "本文重要文風", "id": "R042"}, {"type": "reorder", "ja": "科学者たちは動物の数を減らそうとしました。", "answer": "Scientists tried to reduce the number of animals.", "tokens": ["Scientists", "tried", "to", "reduce", "the", "number", "of", "animals."], "group": "本文重要文風", "id": "R043"}, {"type": "reorder", "ja": "いくつかの動物は自然の中で重要な役割を果たします。", "answer": "Some animals play an important role in nature.", "tokens": ["Some", "animals", "play", "an", "important", "role", "in", "nature."], "group": "本文重要文風", "id": "R044"}, {"type": "reorder", "ja": "私たちはできる限り慎重に選択しなければなりません。", "answer": "We have to make choices as carefully as we can.", "tokens": ["We", "have", "to", "make", "choices", "as", "carefully", "as", "we", "can."], "group": "本文重要文風", "id": "R045"}, {"type": "reorder", "ja": "彼女は朝食におにぎりを食べました。", "answer": "She had a rice ball for breakfast.", "tokens": ["She", "had", "a", "rice", "ball", "for", "breakfast."], "group": "Scene", "id": "R046"}, {"type": "reorder", "ja": "このベーグルはサーモンとクリームチーズが入っています。", "answer": "This bagel has salmon and cream cheese in it.", "tokens": ["This", "bagel", "has", "salmon", "and", "cream", "cheese", "in", "it."], "group": "Scene", "id": "R047"}, {"type": "reorder", "ja": "私は飛行機の中で少し緊張しました。", "answer": "I was a little nervous on the plane.", "tokens": ["I", "was", "a", "little", "nervous", "on", "the", "plane."], "group": "Scene", "id": "R048"}, {"type": "reorder", "ja": "彼の笑顔は私を幸せにしました。", "answer": "His smile made me happy.", "tokens": ["His", "smile", "made", "me", "happy."], "group": "Scene", "id": "R049"}, {"type": "reorder", "ja": "この辞書は私にとってとても役に立ちます。", "answer": "This dictionary is very useful for me.", "tokens": ["This", "dictionary", "is", "very", "useful", "for", "me."], "group": "Scene", "id": "R050"}], "cloze": [{"type": "cloze", "ja": "もし時間があれば、電話してください。", "sentence": "___ you have time, please call me.", "answer": "If", "options": ["If", "Because", "Although", "That"], "group": "接続詞", "id": "C001"}, {"type": "cloze", "ja": "雨だったので、私たちは家にいました。", "sentence": "We stayed home ___ it was rainy.", "answer": "because", "options": ["because", "if", "although", "that"], "group": "接続詞", "id": "C002"}, {"type": "cloze", "ja": "寒かったけれども、彼女は外へ行きました。", "sentence": "___ it was cold, she went outside.", "answer": "Although", "options": ["Although", "Because", "If", "When"], "group": "接続詞", "id": "C003"}, {"type": "cloze", "ja": "私は彼が親切だと思います。", "sentence": "I think ___ he is kind.", "answer": "that", "options": ["that", "if", "because", "although"], "group": "接続詞", "id": "C004"}, {"type": "cloze", "ja": "窓を開けましょうか。", "sentence": "___ I open the window?", "answer": "Shall", "options": ["Shall", "Will", "Have", "Does"], "group": "助動詞表現", "id": "C005"}, {"type": "cloze", "ja": "一緒に始めましょうか。", "sentence": "___ we start together?", "answer": "Shall", "options": ["Shall", "Will", "Do", "Are"], "group": "助動詞表現", "id": "C006"}, {"type": "cloze", "ja": "ここで待ってくれますか。", "sentence": "___ you wait here?", "answer": "Will", "options": ["Will", "Shall", "Have", "Did"], "group": "助動詞表現", "id": "C007"}, {"type": "cloze", "ja": "私は今行かなければなりません。", "sentence": "I ___ to go now.", "answer": "have", "options": ["have", "must not", "don't", "shall"], "group": "助動詞表現", "id": "C008"}, {"type": "cloze", "ja": "あなたは急ぐ必要はありません。", "sentence": "You do not ___ to hurry.", "answer": "have", "options": ["have", "must", "shall", "will"], "group": "助動詞表現", "id": "C009"}, {"type": "cloze", "ja": "なんてよい考えでしょう。", "sentence": "___ a good idea!", "answer": "What", "options": ["What", "How", "When", "If"], "group": "感嘆文", "id": "C010"}, {"type": "cloze", "ja": "なんて美しいのでしょう。", "sentence": "___ beautiful!", "answer": "How", "options": ["How", "What", "Because", "That"], "group": "感嘆文", "id": "C011"}, {"type": "cloze", "ja": "このスープはおいしいにおいがします。", "sentence": "This soup ___ good.", "answer": "smells", "options": ["smells", "sounds", "looks", "keeps"], "group": "文のしくみ", "id": "C012"}, {"type": "cloze", "ja": "それはよさそうですね。", "sentence": "That ___ nice.", "answer": "sounds", "options": ["sounds", "smells", "keeps", "gives"], "group": "文のしくみ", "id": "C013"}, {"type": "cloze", "ja": "その知らせは私をうれしくしました。", "sentence": "The news ___ me happy.", "answer": "made", "options": ["made", "gave", "sent", "told"], "group": "文のしくみ", "id": "C014"}, {"type": "cloze", "ja": "部屋をきれいにしておきなさい。", "sentence": "___ the room clean.", "answer": "Keep", "options": ["Keep", "Call", "Give", "Send"], "group": "文のしくみ", "id": "C015"}, {"type": "cloze", "ja": "ドアを開けたままにしないで。", "sentence": "Do not ___ the door open.", "answer": "leave", "options": ["leave", "call", "show", "teach"], "group": "文のしくみ", "id": "C016"}, {"type": "cloze", "ja": "彼女は私に助言をくれました。", "sentence": "She ___ me some advice.", "answer": "gave", "options": ["gave", "made", "called", "kept"], "group": "文のしくみ", "id": "C017"}, {"type": "cloze", "ja": "彼は私にメッセージを送りました。", "sentence": "He ___ me a message.", "answer": "sent", "options": ["sent", "bought", "found", "painted"], "group": "文のしくみ", "id": "C018"}, {"type": "cloze", "ja": "私たちは彼をケンと呼びます。", "sentence": "We ___ him Ken.", "answer": "call", "options": ["call", "give", "send", "show"], "group": "文のしくみ", "id": "C019"}, {"type": "cloze", "ja": "私は英語が役に立つとわかりました。", "sentence": "I found English ___.", "answer": "useful", "options": ["useful", "alone", "wild", "foreign"], "group": "文のしくみ", "id": "C020"}, {"type": "cloze", "ja": "外来種は問題を引き起こすことがあります。", "sentence": "Non-native species can ___ problems.", "answer": "create", "options": ["create", "survive", "disappear", "agree"], "group": "本文重要語句", "id": "C021"}, {"type": "cloze", "ja": "いくつかの動物は重要な役割を果たします。", "sentence": "Some animals ___ an important role.", "answer": "play", "options": ["play", "make", "give", "take"], "group": "本文重要語句", "id": "C022"}, {"type": "cloze", "ja": "科学者たちはその数を減らそうとしました。", "sentence": "Scientists tried to ___ the number.", "answer": "reduce", "options": ["reduce", "introduce", "survive", "present"], "group": "本文重要語句", "id": "C023"}, {"type": "cloze", "ja": "その動物は完全に姿を消しました。", "sentence": "The animal disappeared ___.", "answer": "completely", "options": ["completely", "carefully", "probably", "usually"], "group": "本文重要語句", "id": "C024"}]};
let mode = "all";
let quiz = [];
let index = 0;
let score = 0;
let answered = false;
let mistakes = [];
let currentOrder = [];
let currentTokens = [];

const $ = (id) => document.getElementById(id);
const modeLabels = {
  all:"ぜんぶランダム",
  vocab:"単語・熟語",
  reorder:"重要文ならべ替え",
  cloze:"穴埋め"
};

function scrollToQuestionTop() {
  const quizTop = $("quiz");
  if (quizTop) quizTop.scrollIntoView({ behavior: "smooth", block: "start" });
}
function shuffle(arr) {
  const a = [...arr];
  for (let i = a.length - 1; i > 0; i--) {
    const j = Math.floor(Math.random() * (i + 1));
    [a[i], a[j]] = [a[j], a[i]];
  }
  return a;
}
function escapeHTML(s) {
  return String(s).replace(/[&<>'"]/g, c => ({'&':'&amp;','<':'&lt;','>':'&gt;',"'":'&#39;','"':'&quot;'}[c]));
}
function normalizeSentence(s) {
  return (s || "")
    .replace(/[“”]/g, '"')
    .replace(/[’‘]/g, "'")
    .replace(/\s+([,.!?])/g, "$1")
    .replace(/\s+/g, " ")
    .trim();
}
function buildPool() {
  const vocabQuestions = DATA.vocab.map(x => ({...x, quizType:"vocab", direction: Math.random() < 0.5 ? "en-ja" : "ja-en"}));
  const reorderQuestions = DATA.reorder.map(x => ({...x, quizType:"reorder"}));
  const clozeQuestions = DATA.cloze.map(x => ({...x, quizType:"cloze"}));
  if (mode === "vocab") return vocabQuestions;
  if (mode === "reorder") return reorderQuestions;
  if (mode === "cloze") return clozeQuestions;
  return [...vocabQuestions, ...reorderQuestions, ...clozeQuestions];
}
function startQuiz() {
  quiz = shuffle(buildPool()).slice(0, 10);
  index = 0; score = 0; mistakes = [];
  $("setup").classList.add("hidden");
  $("result").classList.add("hidden");
  $("quiz").classList.remove("hidden");
  showQuestion();
  setTimeout(scrollToQuestionTop, 50);
}
function resetQuestionUI() {
  answered = false;
  $("feedback").className = "feedback hidden";
  $("feedback").textContent = "";
  $("nextBtn").classList.add("hidden");
  $("options").innerHTML = "";
  $("options").classList.add("hidden");
  $("reorderArea").classList.add("hidden");
  $("answerArea").innerHTML = "";
  $("wordBank").innerHTML = "";
  currentOrder = [];
  currentTokens = [];
}
function showQuestion() {
  resetQuestionUI();
  const q = quiz[index];
  $("progressBadge").textContent = `${index + 1} / 10`;
  $("scoreBadge").textContent = `正解 ${score}`;
  $("modeBadge").textContent = modeLabels[mode];

  if (q.quizType === "vocab") showVocab(q);
  if (q.quizType === "reorder") showReorder(q);
  if (q.quizType === "cloze") showCloze(q);
}
function showVocab(q) {
  $("options").classList.remove("hidden");
  const sameKind = DATA.vocab.filter(w => w.kind === q.kind && w.en !== q.en);
  if (q.direction === "en-ja") {
    $("qLabel").textContent = `${q.kind}｜意味を選びましょう`;
    $("questionText").className = "question";
    $("questionText").innerHTML = `<b>${escapeHTML(q.en)}</b>`;
    const wrongs = shuffle(sameKind.filter(w => w.ja !== q.ja)).slice(0,3).map(w => w.ja);
    renderOptions(shuffle([q.ja, ...wrongs]), q.ja, q);
  } else {
    $("qLabel").textContent = `${q.kind}｜英語を選びましょう`;
    $("questionText").className = "question ja";
    $("questionText").innerHTML = `<b>${escapeHTML(q.ja)}</b>`;
    const wrongs = shuffle(sameKind.filter(w => w.en !== q.en)).slice(0,3).map(w => w.en);
    renderOptions(shuffle([q.en, ...wrongs]), q.en, q);
  }
}
function showCloze(q) {
  $("options").classList.remove("hidden");
  $("qLabel").textContent = `穴埋め｜${q.group}`;
  $("questionText").className = "question";
  $("questionText").innerHTML = `<b>${escapeHTML(q.sentence)}</b><div style="font-size:clamp(1rem,3vw,1.25rem); color:#68776d; margin-top:10px;">${escapeHTML(q.ja)}</div>`;
  renderOptions(shuffle(q.options), q.answer, q);
}
function renderOptions(list, correct, q) {
  list.forEach(text => {
    const btn = document.createElement("button");
    btn.className = "choiceBtn";
    btn.innerHTML = `<b>${escapeHTML(text)}</b>`;
    btn.addEventListener("click", () => choose(text, correct, q));
    $("options").appendChild(btn);
  });
}
function choose(answer, correct, q) {
  if (answered) return;
  answered = true;
  const isCorrect = answer === correct;
  if (isCorrect) score++; else mistakes.push(q);
  $("feedback").className = "feedback " + (isCorrect ? "ok" : "ng");
  $("feedback").innerHTML = isCorrect
    ? "正解"
    : `正解：<b>${escapeHTML(correct)}</b>`;
  $("nextBtn").classList.remove("hidden");
}
function showReorder(q) {
  $("qLabel").textContent = `並べ替え｜${q.group}`;
  $("questionText").className = "question ja";
  $("questionText").innerHTML = `<b>${escapeHTML(q.ja)}</b>`;
  $("reorderArea").classList.remove("hidden");
  currentTokens = shuffle(q.tokens.map((text, i) => ({text, id:i})));
  renderWordBank();
  renderAnswerArea();
}
function renderWordBank() {
  const bank = $("wordBank");
  bank.innerHTML = "";
  currentTokens.forEach(tok => {
    const btn = document.createElement("button");
    btn.className = "tokenBtn";
    btn.innerHTML = `<b>${escapeHTML(tok.text)}</b>`;
    btn.addEventListener("click", () => {
      currentOrder.push(tok);
      currentTokens = currentTokens.filter(t => t.id !== tok.id);
      renderWordBank();
      renderAnswerArea();
    });
    bank.appendChild(btn);
  });
}
function renderAnswerArea() {
  const area = $("answerArea");
  area.innerHTML = "";
  if (!currentOrder.length) {
    const hint = document.createElement("div");
    hint.style.color = "#68776d";
    hint.style.fontWeight = "900";
    hint.textContent = "ここに語句を並べます";
    area.appendChild(hint);
    return;
  }
  currentOrder.forEach(tok => {
    const span = document.createElement("button");
    span.className = "selectedToken";
    span.innerHTML = `<b>${escapeHTML(tok.text)}</b>`;
    span.addEventListener("click", () => undoToken(tok.id));
    area.appendChild(span);
  });
}
function undoToken(id) {
  const tok = currentOrder.find(t => t.id === id);
  if (!tok) return;
  currentOrder = currentOrder.filter(t => t.id !== id);
  currentTokens.push(tok);
  renderWordBank();
  renderAnswerArea();
}
function undoLast() {
  const tok = currentOrder.pop();
  if (tok) currentTokens.push(tok);
  renderWordBank();
  renderAnswerArea();
}
function clearOrder() {
  currentTokens = [...currentTokens, ...currentOrder];
  currentOrder = [];
  renderWordBank();
  renderAnswerArea();
}
function checkOrder() {
  if (answered) return;
  const q = quiz[index];
  const answer = normalizeSentence(currentOrder.map(t => t.text).join(" "));
  const correct = normalizeSentence(q.answer);
  const isCorrect = answer === correct;
  answered = true;
  if (isCorrect) score++; else mistakes.push(q);
  $("feedback").className = "feedback " + (isCorrect ? "ok" : "ng");
  $("feedback").innerHTML = isCorrect
    ? "正解"
    : `正解：<br><b>${escapeHTML(q.answer)}</b>`;
  $("nextBtn").classList.remove("hidden");
}
function nextQuestion() {
  index++;
  if (index >= quiz.length) showResult();
  else {
    showQuestion();
    setTimeout(scrollToQuestionTop, 50);
  }
}
function pickMessage(score) {
  const high = [
    "すばらしいです！語句と語順がかなり定着しています。仕上げはまちがえた問題だけでOKです。",
    "とてもよくできました。期末前の確認として、並べ替えをもう一周するとさらに安定します。",
    "安定感があります。接続詞・助動詞表現・文の形がよく見えています。"
  ];
  const mid = [
    "いい感じです。まちがえた問題だけ、声に出してもう一度読むと定着します。",
    "ここまでできれば大丈夫。あと少し、語順と熟語をセットで確認しましょう。",
    "よく集中できました。単語だけでなく文の形もつながってきています。"
  ];
  const low = [
    "ここからで大丈夫。まずは単語・熟語を10問、そのあと並べ替えに進みましょう。",
    "今日は確認の日です。できなかった問題は、次に覚えるチャンスです。",
    "10問やり切れたことが前進です。同じメニューをもう一度やってみましょう。"
  ];
  const arr = score >= 8 ? high : score >= 5 ? mid : low;
  return arr[Math.floor(Math.random() * arr.length)];
}
function describeMistake(q) {
  if (q.quizType === "vocab") return `<b>${escapeHTML(q.en)}</b>：${escapeHTML(q.ja)} <span style="color:#68776d;">（${escapeHTML(q.kind)}）</span>`;
  if (q.quizType === "cloze") return `<b>${escapeHTML(q.sentence.replace("___", q.answer))}</b><br>${escapeHTML(q.ja)}`;
  return `<b>${escapeHTML(q.answer)}</b><br>${escapeHTML(q.ja)}`;
}
function showResult() {
  $("quiz").classList.add("hidden");
  $("result").classList.remove("hidden");
  $("finalScore").textContent = `${score} / 10`;
  $("resultMessage").textContent = pickMessage(score);
  const review = $("review");
  review.innerHTML = "";
  if (mistakes.length) {
    const title = document.createElement("div");
    title.className = "reviewItem";
    title.innerHTML = "<b>復習したい問題</b>";
    review.appendChild(title);
    mistakes.forEach(m => {
      const div = document.createElement("div");
      div.className = "reviewItem";
      div.innerHTML = describeMistake(m);
      review.appendChild(div);
    });
  }
}

$("modeGrid").addEventListener("click", e => {
  const btn = e.target.closest(".modeBtn");
  if (!btn) return;
  document.querySelectorAll(".modeBtn").forEach(b => b.classList.remove("selected"));
  btn.classList.add("selected");
  mode = btn.dataset.mode;
});
$("startBtn").addEventListener("click", startQuiz);
$("againBtn").addEventListener("click", startQuiz);
$("backBtn").addEventListener("click", () => {
  $("result").classList.add("hidden");
  $("setup").classList.remove("hidden");
});
$("undoBtn").addEventListener("click", undoLast);
$("clearBtn").addEventListener("click", clearOrder);
$("checkOrderBtn").addEventListener("click", checkOrder);
$("nextBtn").addEventListener("click", nextQuestion);
</script>
</body>
</html>
