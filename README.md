<!doctype html>

<html>
<head>
<meta charset="utf-8">
<title>hanpireitest</title>
</head>

<body>
	<style>
		.content{
			background-color:#f9f9f9;
		}
		body{
			background-color:#ccff00;
		}
	
	
		.dai2 input{
			width:30px;
		}
		.gurafu1{
			width:400px;
			height:auto;
		}
		.dai4 input{
			width:50px;
		}
		input{
			border-radius:4px;
			border:1.5px solid #000000;
		}
		input:focus{
			background-color:#C4E2FF
		}
		button{
		height:80px;
			width:200px;
			border-radius:4px;
			border:1.5px solid #000000;
			transition:background-color 0.3s ease;
		}
		button:hover{
			background-color:#A4A4A4;
			 box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2); 
		}
		.btntxt{
			font-size:25px;
		}
		.btntxt:hover{
			color:#FFFFFF;
		}
		
	</style>
	
	<div class="content">
	<h1>比例、反比例のテスト</h1>
	<p>みんな、自分の能力をテストしてみよう！ちなみにこの背景色は志歩ちゃんのイメージカラーに最も近かったものだよ！</p>
		<h3>
			1.志歩ちゃんは、秒速10mで走っています。スタートを0m地点とする場合、志歩ちゃんがスタートしてから18秒後には、何m地点にいますか？</h3>
	<p>秒速10mで18秒間走るということは、10×18=180</p>
	
	<div class="dai2">
	
	<h3>
		2.志歩ちゃんは、成城学園前からドルトンまでの2000mを歩きます。
		志歩ちゃんが歩く速度が2倍、3倍...となると、かかる時間はどのように変化しますか？</h3>
		<p>分数をイメージして答えてね。</p>
  <p>距離が一定の場合、歩く速度とかかる時間は反比例の関係にある。</p>
	<span>1</span><span>　　</span><span>1</span>
		<br>
	<span>2</span><span>倍、</span><span>3</span><span>倍...</span>
		

	</div>
	<div class="dai3">
		<h3>3.次の文のうち、比例する物には〇を、反比例するものには×を、どちらにも当てはまらないものには△を選択してください。</h3>
		<div class="3_1">
		<fieldset>
		<legend>志歩ちゃんの身長が159cmの場合の志歩ちゃんの体重</legend>
		
		<legend>志歩ちゃんが42.195kmを秒速xmで走るときのかかる時間</legend>
		
		</div>
		<div class="3_3">
		<fieldset>
		<legend>志歩ちゃんのライブの観客数と売上(チケットはすべて同じ値段とする)</legend>
		
		</div>
	</div>
	<div class="dai4">
	<h3>4.次のグラフの比例定数を答えなさい。</h3>
	
		
		<img class="gurafu1" src="https://i.imgur.com/lJYDGP7.png" alt="ごめん！画像が表示されないから、飛ばしてね☆"/>
		<br>
		<p>比例定数(α):このグラフは反比例のグラフで、4,2と2,4を通っている。ということは、α÷2=4,α÷4=2ということになり、α=8だとわかる。</p>
	
	</div>
	<div class="dai5">
	<h3>5.yはxに反比例し、xが5の時、yは9です。比例定数(α)を答えなさい。</h3>
 <p>言い方を変えればy=α÷x。xが5、yは9の場合、5が分母、分子はαの分数の答えが9ということになるので、5×9=45</p>
	<input type="text" name="dai5" id="dai5"/>
	</div>
 <form action="https://formspree.io/f/xnnqbwbw" method="POST">
		<h3>最後に...このページを通してどのようなことを感じたか教えてください。特になければ、志歩ちゃんかわいいでもなんでもいいです。</h3>
	 <h4>模範解答</h4>
			<label for="shimei">お名前</label>
			<br>
		<input type="text" name="shimei" id="shimei" placeholder="日野森志歩" required/>
			<br>
			<label for="kansou" >感想くれ</label>
			<br>
			<textarea id="kansou" name="kansou" required placeholder="志歩ちゃんがかわいかった"></textarea>
			<br>
			<button type="submit"><div class="btntxt">送信</div></button>
		</form>
  <h3>以上でサイトは終わりです！ちょっと不慮のけがで作業効率が激下がりしてしまったけど、何とかやりました。ほんとはもうちょっと問題数を多くしたかったけど、そこは仕方ないので許してクレメンス</h3>
  <img src="https://imgur.com/zmiC36X" alt="けがの写真">
	</div>
	

</body>
</html>
