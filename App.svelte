<script>
  let currentNum=1;
  let num1 = "";
  let num2 = "";
  let awnser = "";
  let operator = "";
  function one(){
    if(currentNum==1){
      num1 += "1";
      erase();
    }
    if(currentNum==2){
      num2 += "1";
    }
  }
  function two(){
    if(currentNum==1){
      num1 += "2";
      erase();
    }
    if(currentNum==2){
      num2 += "2";
    }
  }
  function three(){
    if(currentNum==1){
      num1 += "3";
      erase();
    }
    if(currentNum==2){
      num2 += "3";
    }
  }
  function four(){
    if(currentNum==1){
      num1 += "4";
      erase();
    }
    if(currentNum==2){
      num2 += "4";
    }
  }
  function five(){
    if(currentNum==1){
      num1 += "5";
      erase();
    }
    if(currentNum==2){
      num2 += "5";
    }
  }
  function six(){
    if(currentNum==1){
      num1 += "6";
      erase();
    }
    if(currentNum==2){
      num2 += "6";
    }
  }
  function seven(){
    if(currentNum==1){
      num1 += "7";
      erase();
    }
    if(currentNum==2){
      num2 += "7";
    }
  }
  function eight(){
    if(currentNum==1){
      num1 += "8";
      erase();
    }
    if(currentNum==2){
      num2 += "8";
    }
  }
  function nine(){
    if(currentNum==1){
      num1 += "9";
      erase();
    }
    if(currentNum==2){
      num2 += "9";
    }
  }
  function zero(){
    if(currentNum==1){
      num1 += "0";
      erase();
    }
    if(currentNum==2){
      num2 += "0";
    }
  }
  function period(){
    // num1 += ".";
  }
  function plus(){
    currentNum = 2;
    operator = "+";
  }
  function multi(){
    currentNum = 2;
    operator = "*";
  }
  function sub(){
    currentNum = 2;
    operator = "-";
  }
  function div(){
    currentNum = 2;
    operator = "/";
  }
  function equals(){
    if(operator == "+"){
      awnser = parseInt(num1) + parseInt(num2);
    }
    if(operator == "-"){
      awnser = parseInt(num1) - parseInt(num2);
    }
    if(operator == "*"){
      awnser = parseInt(num1) * parseInt(num2);
    }
    if(operator == "/"){
      awnser = parseInt(num1) / parseInt(num2);
    }
    num1 = "";
    num2 = "";
    operator = "";
    currentNum = 1;
  }
  function erase(){
    if(awnser != ""){
      awnser = "";
    }
  }
  function clr(){
    num1 = "";
    num2 = "";
    operator = "";
    currentNum = 1;
    awnser = "";
  }
</script>
<style>
  .grid-container {
    display: grid;
    grid-template-columns: auto auto auto auto;
    padding: 10px;
  }
  .grid-item {
    background-color: rgba(255, 255, 255, 0.8);
    border: 1px solid rgba(0, 0, 0, 0.8);
    padding: 20px;
    font-size: 30px;
    text-align: center;
  }
	.widdth{
		width: 300px;
	}
</style>
<main class="widdth"> 
  <h1>{num1} {operator} {num2}</h1>
  <h1>{awnser}</h1>
  <div class="grid-container">
    <button class="grid-item" on:click={one}>1</button>
    <button class="grid-item" on:click={two}>2</button>
    <button class="grid-item" on:click={three}>3</button>
    <button class="grid-item" on:click={plus}>+</button>
    <button class="grid-item" on:click={four}>4</button>
    <button class="grid-item" on:click={five}>5</button>
    <button class="grid-item" on:click={six}>6</button>
    <button class="grid-item" on:click={sub}>-</button>
    <button class="grid-item" on:click={seven}>7</button>
    <button class="grid-item" on:click={eight}>8</button>
    <button class="grid-item" on:click={nine}>9</button>
    <button class="grid-item" on:click={multi}>*</button>
    <button class="grid-item" on:click={zero}>0</button>
    <button class="grid-item" on:click={div}>/</button>
    <button class="grid-item" on:click={clr}>c</button>
    <button class="grid-item" on:click={equals}>=</button>
  </div>
</main>
