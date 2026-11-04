# Brand repo starter (any AI tool)

Build a folder that teaches your AI your brand once, so every prompt after that starts from your real guidelines instead of a guess.

This version works with any AI tool that can read and write files in a folder on your computer. **Using Claude?** The Claude version is simpler, with one-word commands: [Brand repo starter for Claude](https://github.com/bethhewitt/brand-repo-starter).

No coding needed. Set aside about 30 minutes. You can stop partway and carry on later.

## Before you start

You need:

- **An AI tool that works with folders on your computer**, such as:

  | Tool | Where you type |
  |---|---|
  | OpenAI Codex | The Codex app, or the `codex` command |
  | Cursor | The chat panel, in Agent mode |
  | GitHub Copilot | Copilot Chat in VS Code, in Agent mode |
  | Gemini CLI | The `gemini` command |
  | Claude Code | The Code tab in the Claude desktop app |

  Check that your plan includes it. Chat-only tools such as ChatGPT or Gemini in a browser can't work with folders: see [Chat-only tools](#chat-only-tools).
- **Your brand material, if you have it:** brand guidelines, 3 to 5 of your best past posts or emails, decks and logo files. Save Word files, Google Docs and slides as PDF first. If you have very little, that's fine: your AI will ask more questions instead.

## Install

1. **Download the kit.** On this page, click the green **Code** button, then **Download ZIP**.
    - *You should see:* a file called `brand-repo-starter-any-ai-main.zip` in your Downloads folder.
2. **Unzip it and give it a home.** Double-click the ZIP to unzip it. Rename the folder after your brand, for example "Northside Bakery brand", and move it to Documents. Move the whole folder, not the files inside it.
    - *You should see:* `README.md`, `AGENTS.md` and a `setup` folder inside it.
3. **Open the folder in your AI tool.** Use its "open folder" option, or in a terminal, go to the folder and start the tool there. If it asks whether you trust the folder, say yes.

**Using GitHub instead?** If a team will share the brand files, click **Use this template** on this page to make your own **private** copy, then clone it and open that folder in step 3.

## Set up your brand

1. **Start the setup.** Type: *Read setup/brand-starter.md and follow it.*
    - *You should see:* a short message about what's going to happen, then a request for your brand name, your website and any material you have.
2. **Add your material.** Your AI makes a `sources` folder inside your brand folder. Drop your files in there, then tell it you're done, with your brand name and website in the same message.
    - *You should see:* a short summary of what it found and what looks thin.
3. **Answer the questions.** It asks one question at a time, with numbered suggestions. Reply with a number or in your own words. Expect 10 to 20 questions.
    - When it asks to create files or read your website, allow it. It only works inside your brand folder.
    - To stop, just close the session. Later, open the folder again and type the step 1 message: it carries on where you left off.
4. **Let it build your brand files.** After the last question, it writes your brand files and tells you which gaps are left.
    - *You should see:* new `knowledge`, `brand`, `templates`, `work` and `outputs` folders, and a new `AGENTS.md` with your brand's name at the top. Anything it couldn't confirm is marked `[gap: …]` instead of guessed.
5. **Judge three test pieces.** It writes a short post, a longer piece and a simple visual using only your brand files, and tells you where the visual is saved. Open it in your browser. Mark each piece **1 On-brand**, **2 Close, but something's off** or **3 Off-brand**, and say what's wrong.
    - When something's off, it shows you the change it would make to a brand file. Approve it, and it tries again.
    - *You should see:* a message saying your brand is ready once all three pieces pass.

## Use it day to day

Open your brand folder in your AI tool and ask for things in plain English. For example:

- "Write three LinkedIn posts about our new product launch"
- "Give me ten content ideas for next month based on our audience"
- "Turn this blog post into a newsletter"

Most tools read `AGENTS.md`, and with it your brand files, at the start of every session. If yours doesn't seem to follow your brand, start with: *Read AGENTS.md first.*

Under each piece, your AI lists anything it had to invent or assume. Check that list before anything goes out. When you correct something, it suggests a change to your brand files so the same mistake doesn't happen again. After changing the brand files, type: *Read setup/brand-check.md and follow it.*

To stress-test a plan or idea before you start on it, type: *Read setup/grilling.md and follow it.* Your AI asks one question at a time, with numbered suggestions, until every decision is settled.

Keep your copy **private**. Once it's set up, it holds your brand material.

## Share it with your team

Put the finished folder on GitHub so your whole team works from the same brand files, and a fix one person makes reaches everyone. Teammates can even use different AI tools. [SHARING.md](SHARING.md) walks you through it step by step with GitHub Desktop, no coding needed.

## If something goes wrong

| Problem | Fix |
|---|---|
| "I can't find setup/brand-starter.md" | You've opened the wrong folder. Open the brand folder itself, the one with `AGENTS.md` and `setup` in it. |
| It can't create files | Your tool may be in a read-only or "ask" mode. Switch it to agent mode, or allow file edits when asked. |
| It doesn't mention your files | Check they're inside the `sources` folder in your brand folder, then tell it they're there. |
| Setup stopped halfway | Open the same folder and type the step 1 message again. It carries on where it left off. |
| It ignores your brand in new sessions | Start with *Read AGENTS.md first*, or ask it to set up its own rules file for your tool. |

## Chat-only tools

ChatGPT, Gemini and other browser chat tools can't open a folder, but you can still use the brand files there once they're built:

1. Build them first with a folder-based tool, using the steps above.
2. In a ChatGPT Project, Custom GPT or Gemini Gem, upload the files from `knowledge/` and `brand/` as its knowledge.
3. Paste everything from `AGENTS.md`, from "Rules for every task" down, into its instructions.
4. Save finished pieces yourself. Chat tools can't write to your folder, so update the brand files by hand when you correct something.

## What gets built

| Folder | What goes in it |
|---|---|
| `AGENTS.md` | The rules your AI reads at the start of every session |
| `sources/` | Your raw material and interview answers. Used for setup only, never copied into new content |
| `knowledge/` | Who you are, who you're for, how you sound, what you say |
| `brand/` | Colours, fonts, logos |
| `templates/` | Formats you repeat (a weekly post, a monthly email) |
| `work/` | Drafts in progress. Kept on your computer only, never shared on GitHub |
| `outputs/` | Approved, finished pieces, which your AI also uses as examples |
| `setup/` | The setup and check instructions |

## Credits

The grilling instructions are adapted from Matt Pocock's [grill-me skill](https://github.com/mattpocock/skills/tree/main/skills/productivity/grill-me), used under the MIT License. His licence is in `setup/grilling-LICENSE`.
