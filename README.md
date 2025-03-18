# Empower Her - An AI Interview Coach and Confidence builder
Hackthon Submission: **Google's Women Techmakers presents She Builds AI** built by **Ashley Sally and Vino Gupta**

Use our AI Interview Coach, build your confidence, and reach new heights in your career.

**Watch the video:** https://devpost.com/software/empower-her-qgesk9

**Try out the app:** https://duncan-prep.streamlit.app/


### App Features:
- **AI Interview Coach:** Practice interviewing with real-time feedback and ace your next interview.
- **Confidence Quiz:** Assess your confidence level and get tips to improve.
- **Resources:** Access a library of resources to support your career growth.
- **Statistics:** Learn about the Gender Pay Gap Statistics & Insights based on your state.
- **Motivation:** Get daily inspirational quotes, read succes stories and motivational tips to keep pushing forward.
- **Progress Tracker:** Monitor your goals, milestones, and achievements as you grow.


## Local Setup Instructions

### Prerequisites

- Python 3.8 or higher
- Git
- Google (Gemini) API key from [Google AI Studio](https://makersuite.google.com/app/apikey)

### Installation Steps

1. Clone the repository

```bash
git clone https://github.com/ashleysally00/interview-prep-app.git
cd interview-prep-app
```

2. Create and activate virtual environment

```bash
# Windows
python -m venv venv
venv\Scripts\activate

# MacOS/Linux
python -m venv venv
source venv/bin/activate
```

3. Install required packages

First, install Streamlit and Google Generative AI dependencies directly

```bash
pip install streamlit
pip install google-generativeai
```

Next install all the other requirements from the txt file

```bash
pip install -r requirements.txt
```

4. Set up your API keys:

Create `.streamlit/secrets.toml`:

```toml
GOOGLE_API_KEY = "your-api-key-here"
```

Create `.env` in root directory:

```
GOOGLE_API_KEY=your-api-key-here
```

5. Run the application

```bash
streamlit run app.py
```

The application should open in your default web browser at `http://localhost:8501`

### Features

- **Confidence Assessment Quiz**: Evaluates your workplace confidence and provides personalized feedback
- **AI Interview Practice**: Interactive interview simulation powered by Google's Gemini AI
- **Split-Screen Interface**: Take the quiz and practice interviewing side by side
- **Instant Feedback**: Get real-time feedback on your interview responses
- **Personalized Recommendations**: Receive tailored advice based on your confidence assessment

### Project Structure

```
interview-prep-app/
├── .streamlit/
│   └── secrets.toml
├── src/
│   ├── confidence_quiz.py
│   ├── gemini_interviewer.py
│   └── utils.py
├── app.py
├── requirements.txt
└── .env
```

### Note

Make sure to never commit your API keys or secrets file to GitHub. The `.gitignore` file is configured to prevent this, but always double-check before committing changes.
