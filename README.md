
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Free Word Counter Online | Count Words & Characters</title>
  <meta name="description" content="Count words, characters, sentences and paragraphs instantly with our free online Word Counter. Check reading time and copy your text easily.">
  <meta name="theme-color" content="#f7f9ff">

  <style>
    :root {
      --blue: #3459e6;
      --blue-dark: #2445c5;
      --ink: #17213b;
      --muted: #66718a;
      --border: #e3e8f3;
      --bg: #f7f9ff;
      --white: #ffffff;
    }

    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: Inter, "Segoe UI", Arial, sans-serif;
      background: var(--bg);
      color: var(--ink);
      line-height: 1.65;
    }

    a {
      color: var(--blue);
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline;
    }

    .container {
      width: min(1000px, 92%);
      margin-inline: auto;
    }

    header {
      background: rgba(255, 255, 255, 0.95);
      border-bottom: 1px solid var(--border);
    }

    .nav {
      min-height: 76px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 20px;
    }

    .brand {
      display: flex;
      align-items: center;
      gap: 11px;
      font-weight: 800;
      font-size: 20px;
      color: var(--ink);
    }

    .brand-icon {
      width: 42px;
      height: 42px;
      display: grid;
      place-items: center;
      color: white;
      background: linear-gradient(135deg, #5378ff, #3450d5);
      border-radius: 13px;
      font-size: 22px;
    }

    .nav-link {
      font-size: 14px;
      font-weight: 650;
    }

    .hero {
      text-align: center;
      padding: 56px 0 32px;
    }

    .eyebrow {
      display: inline-block;
      color: var(--blue);
      background: #e9eeff;
      border-radius: 30px;
      padding: 6px 13px;
      font-size: 12px;
      font-weight: 800;
      letter-spacing: 0.5px;
      text-transform: uppercase;
    }

    h1 {
      font-size: clamp(32px, 5vw, 48px);
      line-height: 1.15;
      letter-spacing: -1.5px;
      margin: 18px 0 12px;
    }

    .hero p {
      max-width: 590px;
      margin: 0 auto;
      color: var(--muted);
      font-size: 17px;
    }

    .tool-card,
    .info-card {
      background: var(--white);
      border: 1px solid var(--border);
      border-radius: 20px;
      box-shadow: 0 12px 40px rgba(38, 59, 115, 0.06);
    }

    .tool-card {
      padding: clamp(18px, 4vw, 32px);
    }

    .editor-top {
      display: flex;
      align-items: center;
      justify-content: space-between;
      flex-wrap: wrap;
      gap: 8px;
      margin-bottom: 12px;
    }

    label {
      font-size: 15px;
      font-weight: 750;
    }

    .privacy {
      color: #168354;
      font-size: 12px;
      font-weight: 700;
    }

    textarea {
      display: block;
      width: 100%;
      min-height: 230px;
      padding: 18px;
      border: 1px solid #d6deed;
      border-radius: 13px;
      resize: vertical;
      font: inherit;
      font-size: 16px;
      color: var(--ink);
      background: #fcfdff;
      outline: none;
      transition: border-color 0.2s, box-shadow 0.2s;
    }

    textarea:focus {
      border-color: var(--blue);
      box-shadow: 0 0 0 4px rgba(52, 89, 230, 0.1);
    }

    .stats {
      display: grid;
      grid-template-columns: repeat(4, minmax(0, 1fr));
      gap: 12px;
      margin: 20px 0;
    }

    .stat {
      padding: 17px 8px;
      text-align: center;
      background: #f5f7ff;
      border: 1px solid #e9edfc;
      border-radius: 14px;
    }

    .stat strong {
      display: block;
      color: var(--blue);
      font-size: clamp(23px, 4vw, 30px);
      line-height: 1.3;
      overflow-wrap: anywhere;
    }

    .stat span {
      color: var(--muted);
      font-size: 12px;
      font-weight: 650;
    }

    .actions {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
    }

    button {
      border: 0;
      border-radius: 10px;
      padding: 12px 18px;
      font: inherit;
      font-size: 14px;
      font-weight: 750;
      cursor: pointer;
      transition: transform 0.15s, background 0.15s;
    }

    button:hover {
      transform: translateY(-1px);
    }

    .primary {
      color: white;
      background: var(--blue);
    }

    .primary:hover {
      background: var(--blue-dark);
    }

    .secondary {
      color: var(--ink);
      background: #edf0f7;
    }

    .secondary:hover {
      background: #e0e6f2;
    }

    .status {
      min-height: 24px;
      margin: 12px 0 0;
      color: var(--muted);
      font-size: 13px;
    }

    .below {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 18px;
      margin: 24px 0 60px;
    }

    .info-card {
      padding: 24px;
      box-shadow: none;
    }

    h2 {
      margin: 0 0 12px;
      font-size: 21px;
      letter-spacing: -0.4px;
    }

    .info-card p,
    .info-card li {
      color: var(--muted);
      font-size: 14px;
    }

    .info-card ol {
      padding-left: 21px;
      margin-bottom: 0;
    }

    .faq {
      margin-top: 20px;
    }

    details {
      border-top: 1px solid var(--border);
      padding: 13px 0;
    }

    summary {
      cursor: pointer;
      font-weight: 700;
      font-size: 14px;
    }

    details p {
      margin-bottom: 0;
    }

    footer {
      padding: 25px 0;
      text-align: center;
      border-top: 1px solid var(--border);
      color: var(--muted);
      font-size: 13px;
    }

    @media (max-width: 650px) {
      .nav {
        min-height: 66px;
      }

      .brand {
        font-size: 17px;
      }

      .hero {
        padding-top: 40px;
      }

      .stats {
        grid-template-columns: repeat(2, minmax(0, 1fr));
      }

      .below {
        grid-template-columns: 1fr;
      }

      .actions button {
        flex: 1;
      }
    }
  </style>
</head>

<body>
  <header>
    <div class="container nav">
      <a class="brand" href="#home" aria-label="Free Tools home">
        <span class="brand-icon" aria-hidden="true">W</span>
        <span>Free Tools</span>
      </a>
      <a class="nav-link" href="#how-to-use">How it works</a>
    </div>
  </header>

  <main id="home" class="container">
    <section class="hero">
      <span class="eyebrow">Simple · Free · Instant</span>
      <h1>Free Online Word Counter</h1>
      <p>
        Count words, characters, sentences and paragraphs in seconds.
        A simple writing tool for students, writers and everyday work.
      </p>
    </section>

    <section class="tool-card" aria-label="Word Counter tool">
      <div class="editor-top">
        <label for="textInput">Your text</label>
        <span class="privacy">✓ Your text stays in this browser</span>
      </div>

      <textarea
        id="textInput"
        placeholder="Start typing or paste your text here..."
        spellcheck="false"
      ></textarea>

      <div class="stats" aria-live="polite">
        <div class="stat">
          <strong id="words">0</strong>
          <span>Words</span>
        </div>
        <div class="stat">
          <strong id="characters">0</strong>
          <span>Characters</span>
        </div>
        <div class="stat">
          <strong id="sentences">0</strong>
          <span>Sentences</span>
        </div>
        <div class="stat">
          <strong id="paragraphs">0</strong>
          <span>Paragraphs</span>
        </div>
      </div>

      <div class="stats">
        <div class="stat">
          <strong id="readingTime">0 min</strong>
          <span>Estimated reading time</span>
        </div>
        <div class="stat">
          <strong id="charactersNoSpaces">0</strong>
          <span>Characters without spaces</span>
        </div>
      </div>

      <div class="actions">
        <button class="primary" id="copyBtn" type="button">Copy text</button>
        <button class="secondary" id="downloadBtn" type="button">Download .txt</button>
        <button class="secondary" id="clearBtn" type="button">Clear text</button>
      </div>

      <p class="status" id="status" role="status" aria-live="polite"></p>
    </section>

    <div class="below">
      <section class="info-card" id="how-to-use">
        <h2>How to use the Word Counter</h2>
        <ol>
          <li>Type or paste your text into the box.</li>
          <li>See the word and character counts update instantly.</li>
          <li>Check your estimated reading time.</li>
          <li>Copy your text or download it as a text file.</li>
        </ol>
      </section>

      <section class="info-card">
        <h2>Why use this tool?</h2>
        <p>
          This free Word Counter helps you check writing length for
          essays, assignments, articles, emails and social posts.
          No account or payment is required.
        </p>
        <p>
          Your text is processed in your browser by this page.
          It is not sent to a server by the counting tool.
        </p>
      </section>
    </div>

    <section class="info-card faq">
      <h2>Frequently asked questions</h2>

      <details>
        <summary>How are words counted?</summary>
        <p>
          Words are separated by whitespace. Punctuation attached to a
          word does not count as a separate word.
        </p>
      </details>

      <details>
        <summary>How is reading time estimated?</summary>
        <p>
          Reading time is estimated using 200 words per minute.
          Actual reading speed can vary from person to person.
        </p>
      </details>

      <details>
        <summary>Is this Word Counter free?</summary>
        <p>
          Yes. You can use this tool without signing up or paying.
        </p>
      </details>
    </section>
  </main>

  <footer>
    <div class="container">
      <p>Free Tools — simple tools for everyday work.</p>
      <p>© <span id="year"></span> Free Tools</p>
    </div>
  </footer>

  <script>
    const textInput = document.getElementById("textInput");
    const statusEl = document.getElementById("status");

    function countText() {
      const text = textInput.value;
      const trimmed = text.trim();

      const words = trimmed ? trimmed.split(/\s+/u).length : 0;

      const sentences = trimmed
        ? (trimmed.match(/[^.!?]+[.!?]+|[^.!?]+$/gu) || [])
            .filter(sentence => sentence.trim()).length
        : 0;

      const paragraphs = trimmed
        ? trimmed.split(/\n\s*\n/u)
            .filter(paragraph => paragraph.trim()).length
        : 0;

      document.getElementById("words").textContent = words;
      document.getElementById("characters").textContent = text.length;
      document.getElementById("charactersNoSpaces").textContent =
        text.replace(/\s/gu, "").length;
      document.getElementById("sentences").textContent = sentences;
      document.getElementById("paragraphs").textContent = paragraphs;

      const minutes = words === 0 ? 0 : Math.ceil(words / 200);
      document.getElementById("readingTime").textContent =
        minutes + (minutes === 1 ? " min" : " min");

      statusEl.textContent = "";
    }

    textInput.addEventListener("input", countText);

    document.getElementById("clearBtn").addEventListener("click", () => {
      textInput.value = "";
      countText();
      statusEl.textContent = "Text cleared.";
      textInput.focus();
    });

    document.getElementById("copyBtn").addEventListener("click", async () => {
      if (!textInput.value) {
        statusEl.textContent = "Pehle kuch text likho.";
        return;
      }

      try {
        await navigator.clipboard.writeText(textInput.value);
        statusEl.textContent = "Text copied successfully!";
      } catch (error) {
        textInput.focus();
        textInput.select();
        statusEl.textContent =
          "Automatic copy unavailable. Press Ctrl+C to copy the selected text.";
      }
    });

    document.getElementById("downloadBtn").addEventListener("click", () => {
      const blob = new Blob([textInput.value], {
        type: "text/plain;charset=utf-8"
      });

      const url = URL.createObjectURL(blob);
      const link = document.createElement("a");
      link.href = url;
      link.download = "my-text.txt";
      link.click();
      URL.revokeObjectURL(url);

      statusEl.textContent = "Text file download started.";
    });

    document.getElementById("year").textContent = new Date().getFullYear();

    countText();
  </script>
</body>
</html>
