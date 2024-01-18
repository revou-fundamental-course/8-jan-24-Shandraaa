**<!DOCTYPE html>
<html>
<head>
	<title>Program Hitung Luas Persegi</title>
</head>
<body>
  
  <div class="home">
    <h1>Luas Persegi</h1>
    <img src="persegi.jpg" alt="persegi.jpg"><br><br><br>
    <p>K = s × s</p>
    <br><br>
    <p class="note">Note : </p>
    <p class="note">s = sisi</p>
    <br><br><br>
    <hr>
    <div class="hasil">
      <p><strong>Hitung Keliling Persegi</strong></p>
    </div>
	<form>
		<input type="number" placeholder="Panjang Sisi" id="sisi"><br>
		<button type="button" onclick="hitung()">Hitung</button>
		<button type="button" onclick="reset()">Reset</button>
		<p id="outputText">Hasil: 0</p>
		<button href="kal.html">Kal</button>
	</form>
  </div>

	<script>
		function hitung() {
			let sisi = parseInt(document.getElementById("sisi").value);
			let luas = sisi * sisi;
			let hasilElem = document.getElementById("hasil");
			document.getElementById("outputText").innerHTML = "Hasil: " + luas;
		}
		function reset() {
		  var displayTextElement = document.getElementById("outputText");
		  displayTextElement.innerHTML = "Hasil: 0";
		}
	</script>
</body>
</html>
<style>
*{
  margin:0;
  padding:0;
}
  .home h1{
    background-color: rgb(225, 130, 211);
    text-align: center;
    height: 55px;
    padding-top: 20px;
  }
  .home {
    text-align: center;
  }
  .home img {
    padding-top: 30px;
    height: 100px;
  }
  .note{
    padding-left: 20px;
    padding-top: 5px;
    text-align: left;
  }
  .hasil p{
    font-size: 20px;
    padding-top:10px;
  }
  .home input {
    margin-top: 10px;
    width: 400px;
    height: 20px;
  }
  .home button{
    margin-top: 10px;
    height: 35px;
    width: 50px;
    background-color: rgb(197, 120, 174);
    transition: 0.75s;
  }
  .home button:hover {
    background-color: red;
    transition: 0.75s;
  }
  #outputText{
    padding-top: 10px;
    margin-top: 10px;
    background-color: rgb(224, 97, 178);
    height: 30px;
  }
</style>**
