securenumbermask
================

securenumbermask jquery plugin

A simple plugin to hide password,credit card numbers & mask other security fields


Easy to use   

Example code : 
<html>
 <head>
    
<title>Test raaccordion</title>
 <script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/1.8.2/jquery.js"></script>
     <script type="text/javascript" src="js/securenumbermask.js"></script>
     <link href="style.css" rel="stylesheet" type="text/css" />
    </head>
    
    <body>
    <input TYPE="text" id="inputtext" name="test1" value="123"/>
      <input TYPE="text" id="inputtext2"   name="test2" value="1234"/>
        <input TYPE="text" id="inputtext3"  name="test3" value="12345"/>
          <input TYPE="text" id="inputtext4"  name="test4" value="123456"/>
    </body>
    <script>
   $(document).ready(function(){
       $('#inputtext').securenumbermask({mask:'*',maxlength:2});
        $('#inputtext2').securenumbermask({mask:'&',maxlength:15});
         $('#inputtext3').securenumbermask();
          $('#inputtext4').securenumbermask();
       }); 
    </script>
</html>