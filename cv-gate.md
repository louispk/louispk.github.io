---
layout: page
title: CV Access
---

<h2>What is the best mode of transportation?</h2>

<form id="riddle-form">
  <input type="text" id="riddle-answer" placeholder="Your answer">
  <button type="submit">Submit</button>
</form>

<p id="error-message" style="color: red; display: none;">Sorry, that's not the right answer. Please try again.</p>

<script>
  document.getElementById('riddle-form').addEventListener('submit', function(event) {
    event.preventDefault();
    var answer = document.getElementById('riddle-answer').value.toLowerCase();
    var correctAnswers = ['bicycle', 'bike'];
    if (correctAnswers.includes(answer)) {
      window.location.href = '/assets/CV_Louis_Kiesewetter.pdf';
    } else {
      document.getElementById('error-message').style.display = 'block';
    }
  });
</script>
