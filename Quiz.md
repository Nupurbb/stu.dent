# Interactive Quiz

<details>
  <summary>Question 1</summary>
  <p>What is the capital of France?</p>
  <ul>
    <li><a href="javascript:void(0);" onclick="showAnswer(1)">Paris</a></li>
    <li><a href="javascript:void(0);" onclick="showAnswer(0)">London</a></li>
    <li><a href="javascript:void(0);" onclick="showAnswer(0)">Berlin</a></li>
    <li><a href="javascript:void(0);" onclick="showAnswer(0)">Madrid</a></li>
  </ul>
  <p id="answer1" style="display: none;"><strong>Correct Answer:</strong> Paris</p>
</details>

<details>
  <summary>Question 2</summary>
  <p>Which planet is known as the Red Planet?</p>
  <ul>
    <li><a href="javascript:void(0);" onclick="showAnswer(0)">Earth</a></li>
    <li><a href="javascript:void(0);" onclick="showAnswer(1)">Mars</a></li>
    <li><a href="javascript:void(0);" onclick="showAnswer(0)">Venus</a></li>
    <li><a href="javascript:void(0);" onclick="showAnswer(0)">Jupiter</a></li>
  </ul>
  <p id="answer2" style="display: none;"><strong>Correct Answer:</strong> Mars</p>
</details>

<details>
  <summary>Question 3</summary>
  <p>What is the largest mammal in the world?</p>
  <ul>
    <li><a href="javascript:void(0);" onclick="showAnswer(0)">Giraffe</a></li>
    <li><a href="javascript:void(0);" onclick="showAnswer(0)">African Elephant</a></li>
    <li><a href="javascript:void(0);" onclick="showAnswer(1)">Blue Whale</a></li>
    <li><a href="javascript:void(0);" onclick="showAnswer(0)">Lion</a></li>
  </ul>
  <p id="answer3" style="display: none;"><strong>Correct Answer:</strong> Blue Whale</p>
</details>

<details>
  <summary>Question 4</summary>
  <p>What is the largest planet in our solar system?</p>
  <ul>
    <li><a href="javascript:void(0);" onclick="showAnswer(0)">Mars</a></li>
    <li><a href="javascript:void(0);" onclick="showAnswer(0)">Earth</a></li>
    <li><a href="javascript:void(0);" onclick="showAnswer(0)">Venus</a></li>
    <li><a href="javascript:void(0);" onclick="showAnswer(1)">Jupiter</a></li>
  </ul>
  <p id="answer4" style="display: none;"><strong>Correct Answer:</strong> Jupiter</p>
</details>

<script>
  function showAnswer(questionNumber) {
    const answerElement = document.getElementById(`answer${questionNumber + 1}`);
    answerElement.style.display = "block";
  }
</script>
