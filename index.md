<!DOCTYPE html>
<html lang="en">
<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>Document</title>
 <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
 <style type="text/css">
  p{
   color:red;
   margin:5px;
   cursor:pointer;
  }
  p:hover{
   background:yellow;
  }
  .zenbo{
   position: fixed;
   top: 0;
   left: 0;
   width: 100%;
   height: 100%;
   z-index: 0;
   background: rgba(0,0,0,0.5);
   display: flex;
   justify-content: center;
   align-items: center;
  }
  .X{
   position: fixed;
   top:0;
   right: 0;
   z-index: 10;
   background:  rgba(0,0,0,0.5);
   display: flex;
   
  }


 </style>
</head>
<body>
 <p>產品介紹</p>
 <h1>嚕嚕米</h1>
 <div class="zenbo">
  <img src="https://www.moomin.tw/wp-content/uploads/2020/09/%E5%9A%95%E5%9A%95%E5%92%AA54.jpg">
 <div class="X" >
  <img src="X.png" width="100" height="100">
 </div>

 <script type="text/javascript">
  $('p').click(function(){
   $('.zenbo').slideToggle();
  });
  $('p').click(function(){
   $('.X').slideToggle();
  });
  $('.X').click(function(){
   $('.zenbo').slideToggle();
  });
  $('.X').click(function(){
   $('.X').slideToggle();
  });
 </script>

</body>
</html>
