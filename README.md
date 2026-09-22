# LEARNWITHANOO  

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Learn With Anoo - Bihar Board and NCERT aligned learning platform for Class 11 and 12 students.">
  <title>Learn With Anoo | Learn Smart. Score Better.</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header class="navbar">
    <a class="brand" href="#home" aria-label="Learn With Anoo home">
      <span class="brand-icon">📚</span>
      <span>LEARN WITH <b>ANOO</b></span>
    </a>

    <button class="menu-toggle" id="menuToggle" aria-label="Open navigation" aria-expanded="false">☰</button>

    <nav id="mainNav">
      <a href="#home">Home</a>
      <a href="#classes">Classes</a>
      <a href="#subjects">Subjects</a>
      <a href="#planner">Planner</a>
      <a href="#practice">Practice</a>
      <a href="#progress">Progress</a>
      <a href="#about">About</a>
    </nav>
  </header>

  <main>
    <section id="home" class="hero">
      <div class="hero-content">
        <span class="eyebrow">📖 YOUR LEARNING COMPANION</span>
        <h1>Learn Smart.<br><span>Understand Deep.</span><br>Score Better.</h1>
        <p>Your Class 11 & 12 learning and exam preparation companion for Bihar Board students, with NCERT-aligned concepts.</p>

        <div class="hero-actions">
          <button class="btn primary" data-target="classes">Start Learning →</button>
          <button class="btn secondary" data-target="classes">Explore Classes</button>
        </div>

        <div class="hero-stats">
          <div><strong>11 & 12</strong><small>Classes</small></div>
          <div><strong>3</strong><small>Streams</small></div>
          <div><strong>Daily</strong><small>Practice</small></div>
        </div>
      </div>

      <div class="hero-visual">
        <div class="floating-card card-one">🧠 Understand concepts</div>
        <div class="book-illustration">
          <div class="book-cover">📚<strong>ANOO</strong><small>LEARN EVERY DAY</small></div>
        </div>
        <div class="floating-card card-two">🎯 Track your progress</div>
      </div>
    </section>

    <section class="section journey">
      <div class="section-heading">
        <span class="eyebrow">YOUR LEARNING JOURNEY</span>
        <h2>From learning to improvement</h2>
      </div>
      <div class="journey-grid">
        <div>01 <strong>Choose Class</strong></div>
        <div>02 <strong>Choose Stream</strong></div>
        <div>03 <strong>Learn Concepts</strong></div>
        <div>04 <strong>Practice</strong></div>
        <div>05 <strong>Take Tests</strong></div>
        <div>06 <strong>Revise & Improve</strong></div>
      </div>
    </section>

    <section id="classes" class="section">
      <div class="section-heading">
        <span class="eyebrow">START HERE</span>
        <h2>Choose your class</h2>
        <p>Select a class to explore available streams and subjects.</p>
      </div>

      <div class="class-grid">
        <button class="class-card" data-class="11">
          <span class="class-number">11</span>
          <div><h3>Class 11</h3><p>Build strong fundamentals.</p></div>
          <span class="arrow">↗</span>
        </button>
        <button class="class-card" data-class="12">
          <span class="class-number">12</span>
          <div><h3>Class 12</h3><p>Prepare for board examinations.</p></div>
          <span class="arrow">↗</span>
        </button>
      </div>

      <div id="streamArea" class="selection-area hidden">
        <h3 id="selectedClassTitle">Choose Your Stream</h3>
        <div class="stream-grid">
          <button class="stream-card" data-stream="Commerce">💼 <strong>Commerce</strong><small>Accounts, Economics & Business</small></button>
          <button class="stream-card" data-stream="Science">🔬 <strong>Science</strong><small>Physics, Chemistry & Biology</small></button>
          <button class="stream-card" data-stream="Arts">🎨 <strong>Arts</strong><small>History, Geography & more</small></button>
        </div>
      </div>

      <div id="subjectArea" class="selection-area hidden">
        <h3 id="selectedStreamTitle">Subjects</h3>
        <div id="subjectGrid" class="subject-grid"></div>
      </div>
    </section>

    <section id="subjects" class="section soft-section">
      <div class="section-heading">
        <span class="eyebrow">SUBJECT EXPLORER</span>
        <h2>Explore your subjects</h2>
        <p>Choose a subject to view its learning modules.</p>
      </div>
      <div id="allSubjects" class="subject-grid"></div>
    </section>

    <section id="chapter" class="section hidden">
      <div class="section-heading">
        <span class="eyebrow">LEARNING MODULE</span>
        <h2 id="chapterTitle">Subject Overview</h2>
        <p id="chapterDescription"></p>
      </div>
      <div class="learning-grid">
        <article class="learning-card">
          <span>📘</span><h3>Concept Notes</h3>
          <p>Understand concepts in easy, standard and deeper explanations.</p>
          <button class="text-btn" data-target="practice">Explore practice →</button>
        </article>
        <article class="learning-card">
          <span>📝</span><h3>Practice Questions</h3>
          <p>Practice questions with explanations. Sample content only.</p>
          <button class="text-btn" data-target="practice">Practice now →</button>
        </article>
        <article class="learning-card">
          <span>🔁</span><h3>Quick Revision</h3>
          <p>Review definitions, important points and your own notes.</p>
          <button class="text-btn" data-target="planner">Plan revision →</button>
        </article>
      </div>
      <div class="notice">Content status: This demo contains sample learning modules. Official syllabus and verified PYQs will be added only after reliable verification.</div>
    </section>

    <section id="practice" class="section">
      <div class="section-heading">
        <span class="eyebrow">OBJECTIVE CORNER</span>
        <h2>Practice a question</h2>
        <p>Try a sample question and check your answer.</p>
      </div>
      <div class="quiz-card">
        <div class="quiz-top"><span id="quizTopic">Sample Practice</span><span id="quizCount">Question 1</span></div>
        <h3 id="questionText">What is the purpose of studying a concept deeply?</h3>
        <div id="quizOptions" class="quiz-options"></div>
        <p id="quizFeedback" class="quiz-feedback" aria-live="polite"></p>
        <div class="quiz-actions">
          <button class="btn primary" id="nextQuestion">Next Question →</button>
          <button class="btn secondary" id="resetQuiz">Restart</button>
        </div>
      </div>
    </section>

    <section id="planner" class="section soft-section">
      <div class="section-heading">
        <span class="eyebrow">STUDY PLANNER</span>
        <h2>What should I study today?</h2>
        <p>Create a simple daily study target. You can change the plan anytime.</p>
      </div>
      <div class="planner-card">
        <div class="planner-form">
          <label for="studySubject">Subject</label>
          <select id="studySubject">
            <option>Accountancy</option>
            <option>Economics</option>
            <option>Business Studies</option>
            <option>Mathematics</option>
            <option>English</option>
            <option>Hindi</option>
          </select>
          <label for="studyMinutes">Study duration: <span id="minutesLabel">45</span> minutes</label>
          <input id="studyMinutes" type="range" min="15" max="120" value="45" step="15">
          <button class="btn primary" id="addPlan">Add to today's plan</button>
        </div>
        <div class="today-plan">
          <h3>Today's Target</h3>
          <div id="planList"><p class="empty">No tasks yet. Add your first study task.</p></div>
          <div class="plan-total">Total planned: <strong id="totalMinutes">0</strong> minutes</div>
        </div>
      </div>
    </section>

    <section id="progress" class="section">
      <div class="section-heading">
        <span class="eyebrow">MY PROGRESS</span>
        <h2>Small progress every day</h2>
        <p>Your demo progress is stored in this browser.</p>
      </div>
      <div class="progress-grid">
        <div class="progress-card"><span>📚</span><strong id="completedCount">0</strong><small>Tasks completed</small></div>
        <div class="progress-card"><span>⏱️</span><strong id="plannedCount">0</strong><small>Minutes planned</small></div>
        <div class="progress-card"><span>🎯</span><strong id="quizScore">0%</strong><small>Quiz accuracy</small></div>
      </div>
      <div class="progress-track"><div id="progressBar" class="progress-fill"></div></div>
      <p id="progressText">Start a task to begin tracking your progress.</p>
      <button class="btn secondary" id="resetProgress">Reset demo progress</button>
    </section>

    <section id="about" class="section about-section">
      <div class="about-content">
        <span class="eyebrow">ABOUT THE PLATFORM</span>
        <h2>Learn With Anoo</h2>
        <p>A student-focused learning platform for Class 11 and 12. Learn concepts, practice questions, revise regularly and improve step by step.</p>
        <p class="founder">Founded & Created by <strong>Anuj Yadavanshi</strong></p>
      </div>
      <div class="about-box">
        <h3>Our learning philosophy</h3>
        <p>Learn → Understand → Practice → Test → Analyze → Revise → Improve</p>
      </div>
    </section>
  </main>

  <footer>
    <div class="footer-brand">📚 LEARN WITH ANOO</div>
    <p>Learn Smart. Understand Deep. Practice Daily. Score Better.</p>
    <p class="disclaimer">Educational demo. Check official Bihar Board notifications for official syllabus and examination information.</p>
    <p>© <span id="year"></span> LearnWithAnoo. All rights reserved.</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>
