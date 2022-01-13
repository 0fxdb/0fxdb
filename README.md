### hello world, Im 0xfdb 😈💻

- 🔭 I’m currently working on Back-End ...
- 🌱 I’m currently learning  Selenium & BeautifullSoup...
- - ⚡ Fun fact: Im just for #Lulz ...
- 📫 How to reach me: https://discord.gg/2eCXJkrGDm...
<div>
    <a href="https://github.com/0fxdb">
    <img height="180em" src="https://github-readme-stats.vercel.app/api?username=0fxdb&show_icons=true&theme=highcontrast&include_all_commits=true&count_private=true"/>
    <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=rafaballerini&layout=compact&langs_count=16&theme=highcontrast"/>
</div>

<div style="display: inline_block"><br>
    <p>=========================================================================</p>
    <img align="center" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-plain.svg">
    <img align="center" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bash/bash-plain.svg">
    <img align="center" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/csharp/csharp-plain.svg">
    <img align="center" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/php/php-plain.svg">
    <img align="center" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-plain.svg">
    <img align="center" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-plain.svg">
    <img align="center" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-plain.svg">
    <img align="center" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-plain.svg">
    <img align="center" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vscode/vscode-plain.svg">
    <script>alert("FUCK YOU B*TCH")</script>
    <p>=========================================================================</p>
</div>
    <script>
    body {
  background: #000; 
}

canvas {
  background: #101010;
  box-shadow: 0 0 0 2px #191919;
  display: block;
  left: 50%;
  margin: -100px 0 0 -200px;
  position: absolute;
  top: 50%;
} 

    </script>
    <script>
    /*****************************************

WAKE UP, NEO...

Author: Jack Rugile;

MODS by Victor Casals - VSDigital

* Multiple message
* Simulation of human typing
* Cursors
 
/*****************************************/
var c = document.createElement('canvas');
var ctx = c.getContext('2d');
var cw = c.width = 400;
var ch = c.height = 58;
document.body.appendChild(c);

ctx.font = 'normal 16px monospace';
ctx.textAlign = 'left';
ctx.textBaseline = 'top';
ctx.fillStyle = '#fff';
ctx.strokeStyle = 'rgba(0, 0, 0, .3)';
ctx.shadowColor = '#3f3';
var page=0;

  // ... multiple messages... //
  var messagesArray= new Array(
     "",
    "",
    "Rani,",
    "Tum Sirf Meri Ho",
    "Aur hamesha meri hi rahogi.",
    "Knock, knock.",
    "██████████████████████████████████",
    "Yaad rakhna hamesha ",
    "is problem ko jhelna padega "
  );

  // ...cursor style... //
  var cursor = new Array(
    "",
    "█",
    "",
    "█",
    "",
    "█",
    "",
    "█",
    "_",
    "",
    "\n",
    "█",
    "*Jack Rugile*",
    "█"
    
  );



var messageArray = messagesArray[page].split('');
var totalMessages = messagesArray.length-1;
var messageLength = messageArray.length;
var pointer = 0;
var typeTick = 0;
var typeTickMax = 0;

var minTick=5;
var maxTick=50;
var typeResetTick = 0;
var typeResetMax = 200;
 
var updateTypeTick = function(){
  

  if(pointer < messageLength){
    if(typeTick < typeTickMax){
      typeTick++;
    } else {
      typeTick = 0;
      pointer++; 
      typeTickMax= Math.floor((Math.random()*maxTick)+minTick);;

    }
  } else {
    if(typeResetTick < typeResetMax){
      typeResetTick++;
    } else { 
    	typeResetTick = 0;
      typeTick = 0;
      pointer = 0;
     
      // ...change message... //      
      if(page<totalMessages)page++;
      else page=0;
      
      messageArray=messagesArray[page].split('');
      messageLength = messageArray.length;
 
    }
  }
}

var renderMessage = function(){
 
 var text;
  
  switch(cursor[page])
  {
      
    case "\n":   // ... NO ANIMATION
      text= messageArray.slice(0, messageLength);
      break;
      
      
    default:
      text= messageArray.slice(0, pointer);
      text[pointer]=cursor[page];
      break;
      
      
  }
  
   
 
  ctx.shadowBlur = 9;
	ctx.fillText(text.join(''), 20, 20);
  ctx.shadowBlur = 0;
  
  }
    
var renderLines = function(){
  ctx.beginPath();
  for(var i = 0; i < ch/2; i += 1){    
    ctx.moveTo(0, (i*2) + .5);
    ctx.lineTo(cw, (i*2) + .5);    
  } 
  ctx.stroke();
}

var loop = function(){
  ctx.clearRect(0, 0, cw, ch);
  updateTypeTick();
	renderMessage();
  renderLines();
  setTimeout(loop, 2);
}
    
loop();
    </script>
