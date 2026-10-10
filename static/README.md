# TRUSTLENS AI
### Think Before You Trust

TRUSTLENS AI is an AI-assisted digital safety application that analyzes messages, internship offers, job offers, and website URLs to identify potential warning signs and recommend safer next steps.

## Features

- **Message Analyzer:** Checks messages for suspicious wording, threats, payment requests, and sensitive-information requests.
- **Internship Offer Analyzer:** Identifies warning signs in internship offers and training opportunities.
- **Job Offer Analyzer:** Flags potential recruitment scams, unusual fees, and unrealistic job claims.
- **URL Analyzer:** Checks links for selected suspicious URL patterns.
- **Rule-Based Risk Scoring:** Calculates a heuristic score from detected warning signals.
- **Gemini AI Explanations:** Provides plain-English assessments and verification suggestions.
- **Analyzer Selection Interface:** Lets users choose one analyzer at a time.

## Technologies Used

- Python
- Flask
- Google Gemini API
- HTML5
- CSS3
- Regular Expressions
- Python URL Parsing

## How It Works

1. Select an analyzer.
2. Enter a message, offer, or website URL.
3. The rule-based engine checks for configured warning patterns.
4. A heuristic risk score and warning list are generated.
5. Gemini AI provides an additional explanation when available.
6. TRUSTLENS AI presents recommended verification steps and safe actions.

## Project Structure

```text
trustlens-ai/
├── app.py
├── templates/
│   └── index.html
├── static/
│   └── style.css
└── README.md
```

## Installation and Setup

### 1. Install Python dependencies

Open a terminal in the project folder and run:

```bash
python -m pip install flask google-genai
```

### 2. Configure the Gemini API key

Set your API key as an environment variable. Never publish the key in your code or GitHub repository.

**Windows PowerShell:**

```powershell
$env:GEMINI_API_KEY="YOUR_API_KEY"
```

Replace `YOUR_API_KEY` locally with your own key. Do not share it.

### 3. Start the application

```bash
python app.py
```

### 4. Open in your browser

Visit:

http://127.0.0.1:5000

## Limitations

- Risk scores are heuristic indicators, not verified probabilities.
- The application does not independently confirm whether an organization or message is genuine.
- URL checks use selected patterns and do not guarantee that a website is safe or malicious.
- Gemini explanations depend on API availability, access, and quota.
- False positives and false negatives are possible.

## Future Enhancements

- Screenshot text extraction using OCR
- Analysis history with user-controlled deletion
- More comprehensive URL reputation checks
- Automated testing and improved risk calibration
- Deployment with secure API-key management

## Disclaimer

TRUSTLENS AI is an educational prototype intended to support digital safety awareness. It does not replace independent verification or professional security tools.

**Think Before You Trust.**