# question_four
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
  <script language="javascript">
          /*Question 4: Capitalize Words
      Write a program that accepts a string as input, capitalizes the first letter of each word in the 
      string, and then returns the result string.
      Examples: 
      "hi"=> returns "Hi"
      "i love programming"=> returns "I Love Programming*/

      
    function capital(){
      var inputText = document.getElementById("call").value;
      var capitalizedText= inputText.replace(/\b\w/g, function(char){
        return char.toUpperCase();
      });
      document.getElementById("result").innerHTML=capitalizedText;
    }
  </script>
</head>
<body>
  <form name="myform" action="" method="post">
    <input type="text" id="call">
    <br><br>
    <input type="button" onclick="capital()" value="submit">
  </form>
  <div id="result"></div>
</body>
</html>
