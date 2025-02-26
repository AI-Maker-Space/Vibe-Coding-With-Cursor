<p align = "center" draggable="false" ><img src="https://github.com/AI-Maker-Space/LLM-Dev-101/assets/37101144/d1343317-fa2f-41e1-8af1-1dbb18399719" 
     width="200px"
     height="auto"/>
</p>

# 🐍 Existential Snake Game: Where Snakes Get Hiss-terically Deep! 🧠

Ssssup, fellow existentialists! Welcome to the most mind-bending, scale-raising twist on the classic Snake game ever! This ain't your average reptile simulator - our snake is slithering through a full-blown existential crisis while dropping philosophical quotes that'll make your brain do coils! 🤯 Plus, food gets all nasty and rotten if you wait too long (talk about a sssspoiled meal!), and your snake will totally judge your life choices when you eat the gross stuff - how ssssassy!

> **Want to sink your fangs into the full gameplay deets?** Check out [GAMEPLAY.md](GAMEPLAY.md) for all the juicy features, mechanics, and how to launch the game! 🎮

## 📋 What's Coiled Up Inside This Repo

- [What You Need to Ssslither](#prerequisites) 🛠️
- [Getting This Bad Boy Ssstarted](#installation) 🚀
- [How This Thing's Ssstructured](#project-structure) 🏗️
- [Why UV Is More Venomous Than pip](#why-uv-instead-of-pip) ⚡
- [When Stuff Hisssses and Breaks](#troubleshooting) 🔧
- [Legal Boring Sssstuff](#license) 📜

## 🛠️ What You Need to Ssslither <a name="prerequisites"></a>

Before you dive into the existential abyss, make sure you've ssscaled up with:
- [Node.js](https://nodejs.org/) (v14 or higher) - JavaScript runtime that's actually cool
- [npm](https://www.npmjs.com/) (comes with Node.js) - for all those sweet packages
- [Python](https://www.python.org/) (v3.8 or higher) - because snakes 🐍 and Python, get it?
- [UV](https://github.com/astral-sh/uv) - the lightning-fast package installer that makes pip look like it's molting 🐢
- [Cursor](https://cursor.sh/) - the AI-powered code editor that'll make your coding slither smoothly! 🧠✨

## 🚀 Getting This Bad Boy Ssstarted <a name="installation"></a>

### ⚡ Quick Setup (The Lazy Snake Way - We Approve!)

We've made some awesome scripts that do all the boring stuff for you (because even snakes hate repetitive tasks):

- **Linux/macOS**:
  ```
  chmod +x setup.sh
  ./setup.sh
  ```

- **Windows** (Run in PowerShell):
  ```
  .\setup.ps1
  ```

After running the script, just follow the instructions on screen. It's so easy, even a snake with no limbs could do it! 🐍

### 🔧 Manual Setup (For Control Freaks and Constrictor Types)

#### Installing UV

If you don't have UV yet, get it with these commands (they won't bite!):

- **Windows** (Run in PowerShell):
  ```
  curl -sSf https://astral.sh/uv/install.ps1 | powershell
  ```

- **macOS/Linux**:
  ```
  curl -sSf https://astral.sh/uv/install.sh | sh
  ```

#### Installing Cursor

1. Head over to [cursor.sh](https://cursor.sh/) and download the installer for your OS
2. Run the installer and follow the prompts
3. Launch Cursor and open this project folder
4. Feel the power of AI-assisted coding flow through your fingertips! 🧙‍♂️✨

#### Backend Setup (Where the Snake's Brain Lives)

1. Slither into the backend directory:
   ```
   cd backend
   ```

2. Create a virtual environment using UV (think of it as your snake's terrarium):
   ```
   uv venv
   ```

3. Activate the virtual environment (wake up the snake!):
   - On Windows (Command Prompt):
     ```
     .venv\Scripts\activate
     ```
   - On Windows (PowerShell):
     ```
     .\.venv\Scripts\Activate.ps1
     ```
   - On macOS/Linux:
     ```
     source .venv/bin/activate
     ```

4. Install the required dependencies using UV:
   ```
   uv pip install -r requirements.txt
   ```

5. Start the FastAPI server (release the snake!):
   ```
   uv run main.py
   ```

   The backend server will start running at `http://localhost:8000`. Ssssensational! ✨

#### Frontend Setup (The Snake's Pretty Face)

1. Open a new terminal window and slither to the frontend directory:
   ```
   cd frontend
   ```

2. Install the required dependencies (snake accessories):
   ```
   npm install
   ```

3. Start the React development server (let the snake see the world!):
   ```
   npm start
   ```

   The frontend will fire up at `http://localhost:3000`. Look at you, web dev snake charmer! 🧙‍♂️🐍

## 🏗️ How This Thing's Ssstructured <a name="project-structure"></a>

```
existential-snake-game/
├── backend/                         # Where the snake's brain lives
│   ├── main.py                      # FastAPI server (the snake charmer)
│   ├── requirements.txt             # Python dependencies
│   └── data/                        # Where we store all the deep snake thoughts
├── frontend/                        # The pretty scales of our existential snake
│   ├── public/                      # Static files (boring but necessary)
│   ├── src/                         # Where the React magic happens
│   │   ├── components/              # Building blocks of our snake UI
│   │   │   ├── SnakeGame.js         # The star of the show! 🌟🐍
│   │   │   ├── StartScreen.js       # First impressions matter, even for snakes
│   │   │   └── EndScreen.js         # For when snake existence ends
│   │   ├── App.js                   # The glue holding all snake parts together
│   │   ├── App.css                  # Making things pretty and snake-like
│   │   └── index.js                 # The entry point (snake head, if you will)
│   └── package.json                 # Node.js dependencies (the snake's diet)
├── setup.sh                         # Setup script for Linux/macOS
├── setup.ps1                        # Setup script for Windows
├── README.md                        # You're reading this right now! 👀
└── GAMEPLAY.md                      # All the juicy snake game details
```

## ⚡ Why UV Is More Venomous Than pip <a name="why-uv-instead-of-pip"></a>

UV is the cobra 🐍 of Python package installers:

- **Speed**: UV strikes faster than a rattlesnake, being 10-100x quicker than pip! Zoom zoom! 🏁
- **Reliability**: Dependency resolution that actually works (shocking, we know) - no more tangled nests!
- **Compatibility**: Works with pip's commands, so no new snake tricks to learn
- **Safety**: Written in a safe language, so it's basically wearing snake armor
- **Environment Management**: The `uv run` command makes sure everything runs in the right place, so you can say goodbye to those annoying "module not found" errors that make you want to hiss in frustration 🐍

## 🔧 When Stuff Hisssses and Breaks <a name="troubleshooting"></a>

- **Backend Connection Issues**: Make sure the FastAPI server is running at `http://localhost:8000`. No server = sad snake with nowhere to slither 😢
- **CORS Errors**: The backend is configured to allow requests from anywhere. If you hit CORS issues, check your browser's security settings (they're being overprotective of your snake).
- **Game Performance**: If the game is crawling slower than an actual snake in molasses, try closing those 50 other browser tabs you have open. We see you, tab hoarder! 👀
- **UV Issues**: If UV is shedding its skin at the wrong time, check the [official docs](https://github.com/astral-sh/uv). They know their snake stuff!
- **Virtual Environment Activation Issues**: 
  - On Windows PowerShell: use `.\.venv\Scripts\Activate.ps1`
  - On Windows Command Prompt: use `.venv\Scripts\activate`
  - On macOS/Linux: use `source .venv/bin/activate`

## 📜 Legal Boring Sssstuff <a name="license"></a>

This project is open source and available under the [MIT License](LICENSE). That means you can do pretty much whatever you want with it - go wild! Just don't blame us if your snake has an existential crisis. That's between you two. 🐍💭

---

Now go forth and contemplate existence while eating digital fruit! 🍎 Remember: the unexamined snake game is not worth playing. - Ssssocrates (probably)

P.S. Did you know that snakes don't actually have existential crises? That's because they're too busy being absolutely fang-tastic! 🐍✨
