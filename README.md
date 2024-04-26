<!DOCTYPE html>
<html>
  <head>
    <title>smart_add_calc.demo</title>
    <style>
      footer {
        position: fixed;
        bottom: 0;
        width: 100%;
        background-color: #333; /* Dark gray background */
        padding: 10px 0;
        color: white; /* White text */
        font-size: 12px;
      }
    </style>
  </head>
  <body>
    <form>
      <h3>Number 1:</h3>
      <label for="a">Number 1:</label>
      <input id="a" placeholder="Write a number..">
      <br>
      <h3>Number 2:</h3>
      <label for="b">Number 2:</label>
      <input id="b" placeholder="Write another number..">
      <br>
      <br>
      <button type="reset">Reset</button><button type="button" onclick="calculateSum()">Submit</button>
      <br>
      <p style="text-align: center" id="c"><b>Input</b></p>
    </form>

    <footer>
      <code>Literal Website, Made by a beginner. ©</code>
    </footer>

    <script>
      function calculateSum() {
        var num1 = parseFloat(document.getElementById('a').value);
        var num2 = parseFloat(document.getElementById('b').value);
        var sum = num1 + num2;
        document.getElementById('c').innerHTML = "<b>Sum:</b> " + sum;
      }
    </script>
  </body>
</html>
