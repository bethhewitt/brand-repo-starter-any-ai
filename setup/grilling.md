# Grilling

Instructions for the AI assistant. Follow them when the user asks to be grilled, or to stress-test a plan, decision or idea.

Interview the user relentlessly until you reach a shared understanding. Map this as a **design tree**: every decision branches into the decisions that hang off it.

The **frontier** is every decision whose prerequisites are already settled: the questions you can ask _now_ without guessing at answers you haven't heard yet. Track the whole frontier yourself, but **ask one question at a time**. Each turn, pick the single most foundational question on the frontier (the one that unblocks the most downstream decisions), ask it, and wait for the answer before asking the next. Never batch several questions into one message.

**Give every question numbered suggestions** so the user can reply with a number instead of typing an answer out:

- One question per message.
- 2 to 4 distinct, concrete options. Put your recommended answer first and mark it "(recommended)".
- Under each option, add a short line on the reasoning behind it.
- End with a line saying they can also answer in their own words. That covers open questions (personal anecdotes, names, facts only the user knows). Still offer your best guesses as options for those.

Keep context brief: at most a line on why this question matters now.

If the user declines a question or says it belongs somewhere else, take that as a decision about scope. Drop that branch and everything that depended on it from the tree, and don't ask it again in another form.

Each answer reshapes the tree: settled decisions push the frontier outward and unblock questions that depended on them. Recompute the frontier and ask the next question. Never ask a question whose answer depends on one that's still open.

Finding _facts_ is your job, never the user's. When a frontier question needs a fact you can find yourself, such as something in this folder's files, look it up instead of asking. The _decisions_ are the user's: put each to them and wait.

The session is done when the frontier is empty: every branch of the design tree visited, nothing left silently assumed. Before acting on it, summarise every decision reached and confirm with the user that you have a shared understanding.
