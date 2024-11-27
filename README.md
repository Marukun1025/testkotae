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
			border:1px;
		}
		button{
		height:80px;
			width:200px;
			border-radius:4px;
		}
		
		
	</style>
	
	<div class="content">
	<h1>比例、反比例のテスト</h1>
	<p>みんな、自分の能力をテストしてみよう！ちなみにこの背景色は志歩ちゃんのイメージカラーに最も近かったものだよ！</p>
		<h3>
			1.志歩ちゃんは、秒速10mで走っています。スタートを0m地点とする場合、志歩ちゃんがスタートしてから18秒後には、何m地点にいますか？</h3>
	<p>もしあなたの答えが50m地点だった場合、ここには50と入力してね。</p>
	<input type="number" name="dai1" id="dai1_1"/>
	<div class="dai2">
	
	<h3>
		2.志歩ちゃんは、成城学園前からドルトンまでの2000mを歩きます。
		志歩ちゃんが歩く速度が2倍、3倍...となると、かかる時間はどのように変化しますか？</h3>
		<p>分数をイメージして答えてね。</p>
	<input name="dai2no2"type="number" id="dai2_2"/><span>　　</span><input name="dai2no4" id="dai2_4" type="number"/>
		<br>
	<input name="dai2no1" type="number" id="dai2_1"/><span>倍、</span><input name="dai2no3" id="dai2_3" type="number"/><span>倍...</span>
		

	</div>
	<div class="dai3">
		<h3>3.次の文のうち、比例する物には〇を、反比例するものには×を、どちらにも当てはまらないものには△を選択してください。</h3>
		<div class="3_1">
		<fieldset>
		<legend>志歩ちゃんの身長が159cmの場合の志歩ちゃんの体重</legend>
		<input type="radio" id="hirei1" name="3_1" value="1"/>〇<br>
			<input type="radio" id="hanpirei1" name="3_1" value="2"/>×<br>
			<input type="radio" id="nashi1" name="3_1" value="3"/>△
		</fieldset>
		</div>
		<div class="3_2">
		<fieldset>
		<legend>志歩ちゃんが42.195kmを秒速xmで走るときのかかる時間</legend>
		<input type="radio" id="hirei2" name="3_2" value="1"/>〇<br>
			<input type="radio" id="hanpirei2" name="3_2" value="2"/>×<br>
			<input type="radio" id="nashi2" name="3_2" value="3"/>△
		</fieldset>
		</div>
		<div class="3_3">
		<fieldset>
		<legend>志歩ちゃんのライブの観客数と売上(チケットはすべて同じ値段とする)</legend>
		<input type="radio" id="hirei3" name="3_3" value="1"/>〇<br>
			<input type="radio" id="hanpirei3" name="3_3" value="2"/>×<br>
			<input type="radio" id="nashi3" name="3_3" value="3"/>△
		</fieldset>
		</div>
	</div>
	<div class="dai4">
	<h3>4.次のグラフの比例定数を答えなさい。</h3>
	
		
		<img class="gurafu1" src="https://i.imgur.com/lJYDGP7.png" alt="ごめん！画像が表示されないから、飛ばしてね☆"/>
		<br>
		<span>比例定数(α):</span><input type="number" name="dai4no1" id="dai4">
	
	</div>
	<div class="dai5">
	<h3>5.yはxに反比例し、xが5の時、yは225です。比例定数(α)を答えなさい。</h3>
	<input type="text" name="dai5" id="dai5"/>
	</div>
		<button id="submitBtn">答えを送信</button>
		<h3>最後に...このページを通してどのようなことを感じたか教えてください。特になければ、志歩ちゃんかわいいでもなんでもいいです。</h3>
		<form action="https://formspree.io/f/xnnqbwbw" method="POST">
			<label for="shimei">お名前</label>
			<br>
		<input type="text" name="shimei" id="shimei" placeholder="氏名" required/>
			<br>
			<label for="kansou" >感想くれ</label>
			<br>
			<textarea id="kansou" name="kansou" required></textarea>
			<br>
			<button type="submit">送信</button>
		
		
		
		</form>
	</div>
	<script>
		
    function test(){
	let score=0;
        let answer1=document.getElementById("dai1_1").value;
		if(parseInt(answer1)===180){
			score++;
		}
		let answer2_1=document.getElementById("dai2_1").value;
		let answer2_2=document.getElementById("dai2_2").value;
		let answer2_3=document.getElementById("dai2_3").value;
		let answer2_4=document.getElementById("dai2_4").value;

		if(parseInt(answer2_1)===2){
			score++;
		}
		if(parseInt(answer2_2)===1){
			score++;
		}
		if(parseInt(answer2_3)===3){
			score++;
		}
		if(parseInt(answer2_4)===1){
			score++;
		}
		
		let answer3_1 = document.querySelector('input[name="3_1"]:checked');
		let answer3_2 = document.querySelector('input[name="3_2"]:checked');
		let answer3_3 = document.querySelector('input[name="3_3"]:checked');
		let answer3_4 = document.querySelector('input[name="3_4"]:checked');
		if(answer3_1 && answer3_1.value==="3"){
			score++;
		}
		if(answer3_2 && answer3_2.value==="2"){
			score++;
		}
		if(answer3_3 && answer3_3.value==="1"){
			score++;
		}
		
		let answer4 = document.getElementById("dai4").value;
		
		if(parseInt(answer4)===8){
			score++;
		}
		let answer5 = document.getElementById("dai5").value;
		if(parseInt(answer5)===225){
			score++
		}
		
if(score<=9){
	alert("あなたの点数は"+score+"/10点です");
}else{
	alert("凄い！満点おめでとう！")
}
		
		
	}
		document.getElementById("submitBtn").addEventListener("click",function(){
				test();
			});
	</script>

</body>
</html>
