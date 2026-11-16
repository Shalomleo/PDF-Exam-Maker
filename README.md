# PDF Exam Maker

Turn your lecture notes into a timed, scored practice exam. Upload a PDF (or paste text), choose how many objective and theory questions you want, set a time limit, and sit the exam right in your browser.

It is a single HTML file with no build step, no account and no backend.

## Features

- Upload one or more text-based PDFs or .txt files, or paste notes
- Objective (multiple-choice) questions, marked instantly: 1 mark each
- Theory questions, graded by AI against a model answer with feedback: 5 marks each
- Countdown timer that submits automatically when time is up
- Score and a full review with explanations and model answers
- Set either question type to 0 for a theory-only or objective-only exam (up to 40 objective and 10 theory)
- Retake the same exam or start a new one
- Works on desktop and phone browsers

## How to use it

1. Get a free Gemini API key at https://aistudio.google.com/apikey
2. Open the app (see "Run it" below) and paste your key
3. Upload your notes, choose your question counts and time, and click **Generate exam**

The log under the button shows each step, so you can see what is happening and what went wrong if something fails.

## Run it

- **Locally:** download `index.html` and open it in Chrome, Edge or Firefox
- **Online, free:** host it on GitHub Pages (Settings > Pages > deploy from the main branch) or Netlify Drop, then share the link

## Privacy

- Your API key is stored only in your own browser and is sent only to Google
- The text of your notes is sent to Google's Gemini API to write and grade questions. Don't upload anything confidential. Check Google's current terms for how free-tier data is handled
- Nothing is sent to any server run by this project

## Limits and tips

- Scanned PDFs (photos of pages) have no readable text. Paste the text instead
- Only the first 40,000 characters of your material are used. For a long book, upload one chapter at a time
- AI-written questions and grades can be wrong. Check them against your notes
- If Gemini says a model is busy, the app retries and switches to another model automatically
- Free-tier usage limits are set by Google and can change

## Ideas for contributors

- An optional in-browser model (for example WebLLM) so people can use it with no key
- Shuffled questions and negative marking
- Saving past scores
- Other AI providers

## License

MIT. See the LICENSE file.
