# colab-demo

A demo project by mayabarak00.

## Creative ideas in Google Colab

`creative_ideas.ipynb` asks for everyday objects and uses the OpenAI Responses API with `gpt-6-luna` to suggest three numbered unusual, practical ideas for each object. Keep trying objects in one session; type `quit` to stop.

### Run the notebook

1. Open [Google Colab](https://colab.research.google.com/).
2. Choose **File > Upload notebook** and select the local `creative_ideas.ipynb` file.
3. Connect to a Python runtime and run the SDK installation cell.
4. Run the next code cell and enter your OpenAI API key once in the hidden prompt.
5. Enter an object (for example, `paper clip`) and read the three numbered ideas.
6. Enter another object at the next prompt without restarting or rerunning the cell. Blank input is skipped.
7. Type `quit` to stop (capitalization does not matter). To start a new session afterward, rerun the second code cell and enter your key again.

Tested successfully in Google Colab with `umbrella`, `bicycle`, and `coffee cup`: each object produced three numbered ideas, repeated input worked, and `quit` stopped the session.

You need an OpenAI API key, model access, and API billing or credits. Each nonblank object request may incur an API charge; your object description is sent to OpenAI. Typing `quit` makes no API request. If a request fails, check your key, access to `gpt-6-luna`, credits, and internet connection, then try again or type `quit`. To enter a different key, quit and rerun the cell.

### Keep your key private

- Enter it only in the runtime `getpass` prompt. Never paste it into code, Markdown, output, chat, or Git.
- The notebook does not save the key to files or print it. If hidden input is unavailable, it stops rather than accepting visible input.
- Disconnect and delete the Colab runtime when finished to discard its in-memory state.
- Before sharing or committing a tested notebook, clear its outputs and check that no secrets were added.

The notebook installs the official `openai` SDK in Colab; its other imports are from Python's standard library. See the [OpenAI Responses API text-generation guide](https://developers.openai.com/api/docs/guides/text?lang=python).

## Basic Python example

`hello_colab.ipynb` demonstrates addition and multiplication without extra packages.
