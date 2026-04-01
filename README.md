<html>
<head>
  <title>AutoGov Assistant</title>
</head>
<body>

<h2>Auto-Governance 🇮🇳</h2>

<label>Enter Your Age:</label>
<input type="number" id="age">
<button onclick="check()">Check</button>

<p id="result"></p>

<script>
function check() {
  let age = document.getElementById("age").value;
  let result = "";

  if (age >= 18) {
    result = "You are eligible for:\n- PAN Card\n- Voter ID\n- Bank Account";
  } else if (age >= 16) {
    result = "You can apply for:\n- Learning Driving License";
  } else {
    result = "Currently no major documents required.";
  }

  document.getElementById("result").innerText = result;
}
</script>

</body>
</html>
