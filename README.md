🤖 AI Debate Arena 🤺
Ever wanted to see two AIs go head-to-head on a topic you choose? Well, now you kinda can!

This project lets you set up a debate between a paid OpenAI model (like GPT-3.5-turbo or GPT-4) and a free model from OpenRouter. You provide the topic, set some rules, give each AI a personality, and watch the "discussion" unfold in a simple web UI.

It's all designed to run easily in a free Google Colab notebook.

Why Tho? 🤔
Mostly for fun and experimentation! It was a cool way to:

Play with the OpenAI and OpenRouter APIs side-by-side.

See how different models (paid vs. free) tackle the same prompts.

Mess around with system prompts to give the AIs different "personas."

Build something interactive quickly using the awesome Gradio library.

The Cool Stuff ✨ (Features)
Paid vs. Free Showdown: Pit a premium OpenAI model against a free-tier OpenRouter model.

You're the Moderator: Enter any debate topic you can think of.

Customize Your Fighters:

Choose specific model names for both OpenAI and OpenRouter.

Set the maximum length (tokens) for each AI's response.

Give each AI a unique system prompt to define its personality, stance, or rules of engagement!

Simple Web UI: Thanks to Gradio, you get a straightforward interface to control everything.

Runs on Colab (Free!): No need for fancy servers, just a Google account.

Smarter Banter (Hopefully!): The prompts encourage the AIs to actually respond to each other's points, not just talk past each other (v5 improvement).

How to Run It ▶️ (Getting Started)
Super simple, designed for Colab:

Grab the Code: Download the .ipynb file from this repository.

Head to Google Colab: Go to colab.research.google.com.

Upload: Go to File -> Upload notebook... and select the .ipynb file you downloaded.

Run the Cells: There are usually 3 code cells. Run them one by one, in order:

Cell 1: Installs Libraries: Wait for this to finish. It installs gradio and openai.

Cell 2: Defines Functions: This sets up all the Python code. No visible output here usually.

Cell 3: Launches the UI: This starts the Gradio app.

Click the Link! After running Cell 3, you'll see output including Running on public URL: https://....gradio.live. Click that public URL to open the web interface in a new browser tab.

How to Use It 🚀 (Let the Debate Begin!)
Once the Gradio interface loads in your browser:

Enter Your Topic: Type the debate subject into the "Debate Topic" box.

API Keys are Key! 🔑

Paste your OpenAI API key into the corresponding password field.

Paste your OpenRouter API key into its field.

🚨 SUPER IMPORTANT SECURITY NOTE: These keys are used by the Colab backend. NEVER share your Colab notebook or the public Gradio link if you have entered your real API keys! Treat them like passwords.

Pick Your Fighters: Enter the exact model names you want to use (e.g., gpt-4-turbo-preview, mistralai/mistral-7b-instruct:free). Check the OpenAI/OpenRouter docs for available model IDs.

Give 'em Personalities: Edit the "System Prompt" boxes. Tell the AI how to behave (e.g., "You are a skeptical scientist," "You are an optimistic historian," "Argue strongly for the 'pro' side").

Set the Rules: Adjust the "Max Tokens per Turn" slider to control how long each AI's response can be.

Hit Start! Click the big "🚀 Start Debate" button.

Watch the Sparks Fly (or... text appear):

The "Status" box will show which AI is thinking.

The "Debate Transcript" panel on the right will fill up turn-by-turn.

What's Under the Hood? 🛠️ (Tech Stack)
Python: The main programming language.

Gradio: For creating the super-easy web UI.

OpenAI Python Library: Used to interact with both the official OpenAI API and the OpenRouter API (which cleverly mimics the OpenAI structure).

Google Colab: The environment where the Python code runs.

OpenAI API: Powers one side of the debate.

OpenRouter API: Powers the other side, often with free models.

Heads Up! ⚠️ (Important Notes & Limitations)
API Keys & Costs: Seriously, keep your keys safe. Using OpenAI models will cost money based on your usage – keep an eye on your OpenAI dashboard. OpenRouter free models might have rate limits (the code tries to handle this with small delays, but YMMV).

Colab Limits: Free Colab sessions eventually time out. If your Colab disconnects, the Gradio link will stop working. The public URL is temporary!

Context Window: The AIs "remember" the conversation by sending the history back with each request. Very long debates (many turns or very long responses) might eventually hit the maximum "context window" size for a model, causing errors.

Debate Quality: It's AI, folks! The quality, coherence, and how well they actually debate depends heavily on the models chosen and how good your system prompts are. Sometimes they might just agree or go off-topic. It's experimental!

Future Ideas? 💡 (Maybe Someday)
Proper memory management (summarizing history to avoid context limits).

Allowing more than two debaters? Chaos!

Option to save/load debate transcripts.

Dropdowns to select models instead of typing names.

More sophisticated debate structuring (e.g., timed responses, specific rebuttal rounds).

Contributing 🤝
Hey, feel free to fork this, suggest improvements, or open an issue if something's broken! It's just a fun little project.

License 📜
MIT License (Basically, do what you want with it, but no warranty!)

Hope this captures the casual vibe you wanted! Let me know if you'd like any adjustments.
