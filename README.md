layout:main
<html><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
  
  <script async="" src="https://voidcat.com/void.cat_files/f.txt"></script>
  <script>
    (adsbygoogle = window.adsbygoogle || []).push({
      google_ad_client: "ca-pub-3289062345896209",
      enable_page_level_ads: true
    });
  </script>
  <style>
    html,body { 
      margin: 0; 
      padding: 0; 
      font-family: "Lucida Console", Monaco, monospace; 
      background-color: #101010;
      font-size: 16px;
      color: #eee;
      user-select: none;
      cursor: text;
    }
    div.msg {
      width: 400px;
      margin-left: auto;
      margin-right: auto;
      margin-top: 20%;
    }
    span.host { color: green; }
    span.path { color: blue; }
    div.msg span { float: left; }
    span.hide { opacity: 0; }
    h1{
      display: none;
    }
  </style>
  <title>voidcat</title>
</head>
<body style="">
  <div class="msg">
    <span class="host">root@void</span>
    <span>:</span>
    <span class="path">~</span>
    <span>$&nbsp;</span>
    <span id="content"></span>
    <span id="cursor" class="">█</span>
  </div>
  <ins class="adsbygoogle" style="display:block; margin-left: auto; margin-right: auto;" data-ad-client="ca-pub-3289062345896209" data-ad-slot="9187315106" data-ad-format="auto" data-full-width-responsive="true"></ins>
  <script>
    (adsbygoogle = window.adsbygoogle || []).push({});

    var delayCounter = 0;
    var delayCompleted = 0;
    var msgTyped = 0;
    const typeMsg = "��彩云��易散���琉璃����脆 :)";
    const cursor = document.querySelector("#cursor");
    const msgContent = document.querySelector("#content");
    setInterval(function() {
      cursor.classList.toggle("hide");
    }, 500);
    setInterval(function() {
      // apply delay
      if(delayCompleted < delayCounter){
        delayCompleted++;
        return;
      }

      let newChar = typeMsg[msgTyped];
      if(newChar == "�") {
        delayCounter += 10;
        msgTyped++;
      } else if(newChar == "") {
        msgContent.innerHTML += "</br>";
        msgTyped++;
      }else if(typeMsg.length > msgTyped) {
        msgContent.innerHTML += newChar;
        msgTyped++;
      }
    }, 100);
  </script>


</body></html>