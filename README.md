# HP_build

<html>
<head>

<meta charset="UTF-8">
<meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
<meta http-equiv="X-UA-Compatible" content="IE=EmulateIE10" />
<meta http-equiv="X-UA-Compatible" content="IE=edge">

<!--ここから上はお決まりの定型文です-->


<!--ここからが表現の書式などを決めるcssという部分-->

<style type="text/css">
 p {
color: #ffffff;
font-size: 1.5em;
 }
 

 .red {color:#ff0000;}
 .grey {color:#ffffff; background:#999999;}
 .snow {color:#fffafa;}
 .yellow {color:#ff0000; background:#ffff00;}
 .blue {color:#0000ff;}
 .white {color:#ffffff; blinking;}
 .waku {border:2px dotted #99cc66;
　　　　　　line-height: 200%;
　　　　　　padding: 10px;}

 
 main {
background-color: rgba(255, 255, 255, 0.5);
}

section {
background-color: rgba(0, 225, 0, 0.3);
}
 

/* 点滅 */
.blinking{
	-webkit-animation:blink 1.5s ease-in-out infinite alternate;
    -moz-animation:blink 1.5s ease-in-out infinite alternate;
    animation:blink 1.5s ease-in-out infinite alternate;
}
@-webkit-keyframes blink{
    0% {opacity:0;}
    100% {opacity:1;}
}
@-moz-keyframes blink{
    0% {opacity:0;}
    100% {opacity:1;}
}
@keyframes blink{
    0% {opacity:0;}
    100% {opacity:1;}
}

#wrap {background:none} /*PC用の背景はオフ 背景を指定する部分*/
body::before {
  content:"";
  display:block;
  position:fixed;
  top:0;
  left:0;
  z-index:-1;
  width:100%;
  height:100vh;
  background:url(https://torokoid.github.io/20210704_Utsunomiya_swim/20210704_001.JPG) center/cover no-repeat; /*fixedをトル！*/
  -webkit-background-size:cover;/*Android4*/
  }
  
a.p:hover {
    position: relative;
    text-decoration: none;
}
a.p span {
    display: none;
    position: relative;
    top: -0.5em;
    left: 2em;
}
a.p:hover span {
    border: none;
    display: block;
    width: 800px;
}   
 

@media	screen and (min-width: 540px),
	screen and (orientation: landscape) {
   p.note { display: none; }
}

</style>

<link href="https://cdnjs.cloudflare.com/ajax/libs/lightbox2/2.7.1/css/lightbox.css" rel="stylesheet">

</head>

<body>


<p class="note">
  モバイル端末をお使いの場合は、画面を横向きにすると
  より見やすくご覧頂けます。
</p>
    
<!-- ここから上は定型文としてそのままコピペして再利用します —->

<!—- リンクの作り方、例 -->
<!--
<a href="ここにリンク先のURLを入れる" target="_blank" rel="noopener noreferrer">新規タブで開く</a>
-->
<!-- ぱんくずリストの表示例 -->

<p><a href="https://dorikawa.github.io/20210704_Utsunomiya_swim/">2021年宇都宮市民大会</a>>IT関連情報</p>


<!-- 表題の表示、背景黄色、流れ文字の例 -->
<h1><span class="yellow"><marquee>!!! QRコードの作り方、他にも色々な方法がありますが、一例です。 !!!</marquee></span></h1>

<!--
<div style="background-color:rgb(255,255,255,0.3);”>

<!-- QRコードの表示例 -->
<p align="left"> <img src="qr.png" alt="アクセス用QRコード" width="100">アクセス用QRコード</p>


 <p><h2>① QRコードを作成したいページのURLをコピーします。<br>
② 以下のリンク先に飛んで、所定の場所にURLをペースト、できた画像をダウンロードして使用します。</h2></p>
							       
<p><a href="https://qr.quel.jp/url.php">QRコード作成リンクhttps://qr.quel.jp/url.php</a></p>	
	<br><br>
	
<p><h2>以上、簡単ですが上部のQRコードも同じ方法でできています。<br>リンク先にはURL以外のものもQRコード化する方法が提供されています。</h2></p>


<br><br><br><br><br><br><br><br><br>	
<h1><span class="yellow"><marquee direction="right">!!! 以下、HPの作り方解説 !!!</marquee></span></h1>
 <p><h2>HPの作り方は色々ありますが、ここで説明するのはGithubを使ったHPの作り方の例です。<br><br>
Githubとはネットワーク技術者たちが共同作業をするためのしくみで、2008年に発足、<br>
2018年にはマイクロソフトに吸収合併されました。2021年時点で無料開放されいてます。<br>
今回はそのしくみのごく一部の機能を使います。<br><br>
まず初めに、Githubのアカウントを作ります。<br>
以下のリンク先に飛んで、ユーザーネーム、パスワード、メールアドレスなどを入力してアカウントを作成します。</h2></p>
<p><a href="https://github.com/">Githubリンクhttps://github.com/</a><br>すでにアカウントをお持ちの場合は、ご自分のアカウントに飛ぶようです。</p>

<br>
<a href="20210709_001.png" data-lightbox="abc"><img src="20210709_001.png" alt="サンプル画像" width="900" /></a>
<br>
<p><h2>サインアップを使うのは最初の一回だけ、二回目以降はサインインを使います。<br>
アカウントは一度作ってしまえば、以降はユーザーネームとパスワードの入力でサインインできますので、この二つは忘れないようにしましょう。<br>
ちなみにこのページのアカウント:dorikawa、パスワード:doridori2021　ですのでご自由にお使い下さい。使う際には既にあるリポジトリは温存願います。<br>
以下は新しいリポジトリ(≒ HP)の作り方です。皆さんが独自のアカウントを立ち上げても同じ作業でHPが作れます。<br>
参考までに、このページのリポジトリ名は、HP_buildです。URLの中に見えますね。</h2></p>

<p><h2>では、新しいリポジトリを作ってみましょう。<br>
以下のようにクリックして、</h2></p>
<a href="20210709_006.png" data-lightbox="abc"><img src="20210709_006.png" alt="サンプル画像" width="900" /></a>
<p><h2>リポジトリの名前を適当に決めて入力、<br>
下の二箇所にチェックを入れます。最後に一番下の緑のボタンを押して作成完了です。</h2></p>
<a href="20210709_002.png" data-lightbox="abc"><img src="20210709_002.png" alt="サンプル画像" width="900" /></a>
<p><h2>ここからが本番で、README.fileにソースコードを書き込んでいきます。<br>
ただし、初めてでは難易度が高いので、以下のコードをコピペして使います。</h2></p>
<p><a href="https://docs.google.com/spreadsheets/d/1wnsQSTP2Vv3ncIYPWtxRlBZRESRBkq_FD-y8f3Vbwpk/edit#gid=0" target="_blank" rel="noopener noreferrer">サンプルコードへのリンク、別のタブで開きます。</a></p>

<p><h2>作成段階でREADME.fileだったものは、README.meになっていますが、これの鉛筆マーククリックでソースコードをペーストします。<br>
この段階で市民大会の動画配信したページと同じものができています。</h2></p>

<a href="20210709_007.png" data-lightbox="abc"><img src="20210709_007.png" alt="サンプル画像" width="900" /></a>
<p><h2>では、肝心のYoutube動画のリンク方法です。<br>
Youtubeにアップされている動画の閲覧画面下、共有ボタンを押します。</h2></p>
<a href="20210709_010.jpg" data-lightbox="abc"><img src="20210709_010.jpg" alt="サンプル画像" width="900" /></a>
<p><h2>ダイアログの中、埋め込むを選びます。</h2></p>
<a href="20210709_011.png" data-lightbox="abc"><img src="20210709_011.png" alt="サンプル画像" width="900" /></a>
<p><h2>
埋め込むで出てきたコードをコピーしてそのまま使います。<br>
専門用語で、iframeと呼ばれている仕組みです。<br>
そのままソースコードの中にペーストするとリンクします。</h2></p>
<a href="20210709_012.png" data-lightbox="abc"><img src="20210709_012.png" alt="サンプル画像" width="900" /></a>

<p><h2>最初にコピペしたHPのソースコード中段に並んでいるものがこれです。</h2></p>
<a href="20210709_013.png" data-lightbox="abc"><img src="20210709_013.png" alt="サンプル画像" width="900" /></a>


<p><h2>動画に対応していないGithubでの動画共有はYoutube頼みになります。<br><br>
ここからは、このHPでも多用した静止画像の配置方法です。背景画像もこれに含まれます。<br>
最初にPC内に作った静止画像をリポジトリにアップします。</h2></p>
<a href="20210709_008.png" data-lightbox="abc"><img src="20210709_008.png" alt="サンプル画像" width="900" /></a>
<p><h2>アップロード動作が終わったら、緑のボタンを押して静止画の追加完了。</h2></p>
<a href="20210709_009.png" data-lightbox="abc"><img src="20210709_009.png" alt="サンプル画像" width="900" /></a>
<p><h2>Codeボタンを押した時に見える**.pngや**jpgが静止画像のファイルです。</h2></p>
<a href="20210709_014.png" data-lightbox="abc"><img src="20210709_014.png" alt="サンプル画像" width="900" /></a>
<p><h2>リポジトリ内の画像を表示するソースコードは、以下になります。</h2></p>
<a href="20210709_015.png" data-lightbox="abc"><img src="20210709_015.png" alt="サンプル画像" width="900" /></a>
<p><a href="https://docs.google.com/spreadsheets/d/1wnsQSTP2Vv3ncIYPWtxRlBZRESRBkq_FD-y8f3Vbwpk/edit#gid=1880997290" target="_blank" rel="noopener noreferrer">ソースコードへのリンク、別のタブで開きます。</a></p>

<p><h2>リンク先のページでは、黄色いセルだけ更新すれば、青い列のコードに全て反映されますので、それをコピペするだけで使えます。</h2></p>
<a href="20210709_018.png" data-lightbox="abc"><img src="20210709_018.png" alt="サンプル画像" width="900" /></a>

<br><br>
<p><h2>では、何か変更したら、最下段の緑のボタンを押すのを忘れずに！</h2></p>

<p><h2>最後にリポジトリに記載したHTMLソースコードをHPとして公開する方法の説明です。<br>
以下の操作で、一般的なURLの表示までたどり着きます。<br>
最初に上段右端のSettingを押します。</h2></p>
<a href="20210709_003.png" data-lightbox="abc"><img src="20210709_003.png" alt="サンプル画像" width="900" /></a>
<p><h2>下の方にスクロールして出てくる、Check it out here!を押します。</h2></p>
<a href="20210709_004.png" data-lightbox="abc"><img src="20210709_004.png" alt="サンプル画像" width="900" /></a>
<p><h2>以下の三つのボタンを順番に押します。</h2></p>
<a href="20210709_005.png" data-lightbox="abc"><img src="20210709_005.png" alt="サンプル画像" width="900" /></a>
<p><h2>変更が更新されるまでしばらく待つと緑色になるので、そこにあるのがHPとして公開するURLです。<br>
URLのクリックでHPとして開きます。</h2></p>
<a href="20210709_016.png" data-lightbox="abc"><img src="20210709_016.png" alt="サンプル画像" width="900" /></a>
<br><br>
<p><h2>以上、ちょっと長くなりましたがここまでの作業を順番にこなすと、無料の広告なしHPが作れます。<br>
ここまで読んでいただきありがとうございました！</h2></p>

<p><h2><span class="snow"><marquee scrollamount="16">〜〜〜〜〜〜〜〜ご質問等ありましたら、なんなりとどうぞ！以下のQRコードをスマホで読みこむとブラウザが立ち上がって、メール作成リンクをクリックすると、torokoid@gmail.com(羽田)宛のメール作成動作に入ります。〜〜〜〜〜〜〜〜</marquee></span></h2></p>
<p align="left"> <img src="qr_mail.png" alt="質問メール作成用QRコード" width="100">質問メール作成用QRコード</p>

<br><br><br><br>
<p><h2>最後にそこかしこに出てくるネコですが、<br>
Githubのメインキャラ「オクトキャット」(タコ・ねこ)です。<br>
このHPのQRコード真ん中にも配置してあります。<br>
Net技術者の間ではすでに当たり前のキャラで、グッズも販売されています。<br>
気になる方は、以下のリンクから購入できますので、よろしければどうぞ！</h2></p>
<p><a href="https://thegithubshop.com/">Githubのグッズ販売へのリンク</a></p>
<p><h2>こんなのが売られています。</h2></p>
<a href="20210709_017.png" data-lightbox="abc"><img src="20210709_017.png" alt="サンプル画像" width="900" /></a>

<br><br>

<!--
<p><h2><span class="snow"><marquee scrollamount="16">〜〜〜〜〜〜〜〜作成中〜〜〜〜〜〜〜〜</marquee></span></h2></p>
-->
<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>

<h6>
<p align="right"> <span class="snow">背景奥の白い家は、ユナちゃんの家、場所は秘密です！</span></p>
</h6>
<!-- フッタ -->
 <footer>
 <span class="snow">Copyright 2021/07/08 S.Hada</span>
 </footer>

<!--HPにさまざまなJavaScriptを呼び込むための書式-->
<script src="https://code.jquery.com/jquery-1.12.4.min.js" type="text/javascript"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/lightbox2/2.7.1/js/lightbox.min.js" type="text/javascript"></script>

<script type='text/javascript' src='https://torokoid.github.io/shiba/jquery.js?ver=1.12.4'></script>
<script src="https://torokoid.github.io/shiba/jquery.goup.min.js"></script>
<script src="https://torokoid.github.io/shiba/my.js"></script>


</body>

</html>
