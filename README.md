<br>
<p align="center">
<img src="https://raw.githubusercontent.com/user-attachments/assets/b8c1a603-2960-428e-a382-7f626378f63f/ai-debate-arena-logo.png" width="150" alt="AI Debate Arena Logo">
<h1 align="center">🤖 AI Debate Arena 🤺</h1>
<p align="center">
<i> Ever wanted to pit two AIs against each other in a battle of wits? Now you can! </i>
<br>
<br>
<b> Set up AI debates in Google Colab, customize their personalities, and watch the chaos unfold! </b>
</p>
</p>
<br>
🤔 So, What's This All About?
This project is your ringside ticket to an AI showdown! 🥊

It lets you stage a debate between a paid OpenAI model (think GPT-3.5/4) and a free model from OpenRouter. You call the shots: pick the topic, choose the AI fighters, give 'em unique personalities via system prompts, and watch the verbal sparring happen in a dead-simple web UI.

Best part? It runs entirely within a free Google Colab notebook. No servers, no complex setup, just pure AI debating fun (or nonsense, depending on the models 😉).

✨ Features That Don't Suck
🏆 Premium vs. Free Tier Bout: OpenAI's finest vs. OpenRouter's free contenders.

🎤 You're the Moderator: Input any topic you want debated.

🔧 Customize Your Combatants:

Specify exact model names (e.g., gpt-4-turbo-preview, mistralai/mistral-7b-instruct:free).

Control response length with a Max Tokens slider.

Craft unique System Prompts to dictate each AI's persona, role, or arguing style. Make one a skeptic and the other an optimist!

💻 Simple Web UI: Powered by Gradio for easy interaction. No command-line stuff needed.

💸 Runs on Colab (Free!): Google's got your back.

🧠 Enhanced Banter (v5): Prompts are tweaked to encourage AIs to actually engage with each other's points, not just monologue.

▶️ Getting Started (It's Easy, Promise!)
Designed for maximum Colab laziness:

📥 Grab the Code: Download the .ipynb notebook file from this repo.

☁️ Head to Google Colab: colab.research.google.com

⬆️ Upload: File -> Upload notebook... -> Choose the file you downloaded.

⏯️ Run the Cells: Execute the code cells one by one, in order:

Cell 1: Installs Stuff: pip install gradio openai (takes a moment).

Cell 2: Defines the Magic: Sets up the Python functions. No output expected.

Cell 3: Launches the UI: Starts the Gradio app.

🔗 CLICK THE LINK! Look for the line Running on public URL: https://....gradio.live in the output of Cell 3. Click that public URL. It opens the app in a new browser tab.

(Optional: Add a GIF here showing the UI in action!)
![AI Debate Arena Demo](link_to_your_demo.gif)

🚀 Let the Games Begin! (How to Use)
Okay, the UI is open, now what?

🗣️ Topic Time: Fill in the "Debate Topic".

🔑 API Keys:

Paste your OpenAI API Key (looks like sk-...).

Paste your OpenRouter API Key (looks like sk-or-...).

🚨 SECURITY ALERT! 🚨 These keys are powerful. They are used by the Colab backend while the app runs. NEVER EVER share your Colab notebook or the public Gradio link if you've entered real keys! Treat 'em like passwords!

🤖 Choose Models: Type in the official model names you want to use. Find names in OpenAI/OpenRouter docs.

🎭 Assign Personas: Get creative in the "System Prompt" boxes! Tell the AIs who they are or how to argue. This is where the fun is!

📏 Set Limits: Use the "Max Tokens per Turn" slider. Shorter = faster/cheaper, Longer = more detailed (maybe).

💥 Hit Start! Smash that "🚀 Start Debate" button.

🍿 Grab Popcorn: Watch the "Status" update and the "Debate Transcript" fill up. Enjoy the AI-generated arguments!

🛠️ Tech Stack (What Makes It Tick)
🐍 Python: The brains of the operation.

🎨 Gradio: For the quick & easy web UI.

<img src="https://openai.com/favicon.ico" width=16> OpenAI Python Library: Talks to both OpenAI & OpenRouter APIs.

<img src="https://www.google.com/favicon.ico" width=16> Google Colab: The free runtime environment.

<img src="https://openai.com/favicon.ico" width=16> OpenAI API: Powers one AI brain.

<img src="https://openrouter.ai/favicon.ico" width=16> OpenRouter API: Powers the other AI brain (often with free models!).

⚠️ Important Stuff & Limitations
💰 Keys & Costs: Keep keys secret! OpenAI API usage costs 
$. Check your OpenAI billing. OpenRouter free models can have rate limits (might see errors if you run too fast/much).

⏳ Colab Timeouts: Free Colab sessions don't last forever. If it disconnects, the Gradio link dies. It's temporary!

🧠 Context Limit: AIs "remember" by re-reading the history. Super long debates might exceed a model's memory ("context window"), causing errors. Keep debates reasonably short or use models with huge context windows.

🤷 AI is AI: Debate quality varies wildly! Depends on models, prompts, and cosmic luck. Sometimes they're brilliant, sometimes they're baffling. It's an experiment!

💡 Future Ideas (Things I Might Add If I'm Bored)
Smarter memory (summarizing old turns?).

More than 2 debaters? 🤯

Save/Load debate transcripts.

Model selection via dropdowns.

Fancy debate structures (opening/rebuttal/closing).

🤝 Contributing
Got ideas? Found a bug? Feel free to fork it, submit a Pull Request, or open an Issue. It's all just for fun and learning!

📜 License
MIT License

(Do whatever you want, just don't blame me if your AI debate accidentally summons Skynet.)

27.4s
