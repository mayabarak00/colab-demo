# colab-demo

A demo project by mayabarak00.

## Creative ideas in Google Colab

`creative_ideas.ipynb` asks for an everyday object and uses the OpenAI Responses API with `gpt-6-luna` to suggest one unusual, practical use.

### Run the first version

1. Open [Google Colab](https://colab.research.google.com/).
2. Choose **File > Upload notebook** and select the local `creative_ideas.ipynb` file.
3. Connect to a Python runtime and run the SDK installation cell.
4. Run the next code cell, enter an object (for example, `paper clip`), and enter your OpenAI API key in the hidden prompt.
5. Read the generated idea. Run the second code cell again to try another object.

You need an OpenAI API key, model access, and API billing or credits. API calls may incur charges; your object description is sent to OpenAI. If a request fails, check your key, access to `gpt-6-luna`, credits, and internet connection.

### Keep your key private

- Enter it only in the runtime `getpass` prompt. Never paste it into code, Markdown, output, chat, or Git.
- The notebook does not save the key to files or print it. If hidden input is unavailable, it stops rather than accepting visible input.
- Disconnect and delete the Colab runtime when finished to discard its in-memory state.
- Before sharing or committing a tested notebook, clear its outputs and check that no secrets were added.

The notebook installs the official `openai` SDK in Colab; its other imports are from Python's standard library. See the [OpenAI Responses API text-generation guide](https://developers.openai.com/api/docs/guides/text?lang=python).

## Basic Python example

`hello_colab.ipynb` demonstrates addition and multiplication without extra packages.
