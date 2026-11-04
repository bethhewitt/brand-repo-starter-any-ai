# Brand check

Instructions for the AI assistant. Follow them when the user asks to check or test their brand setup, or after the brand files change.

Prove the brand files are enough on their own. If a test piece comes out off-brand, the fix goes into the brand files, so every future prompt benefits.

## 1. Check for gaps

Read `AGENTS.md`, everything in `knowledge/` and `brand/identity.md`. If any file still says "Not filled in yet", or any `[gap: …]` or `[conflict: …]` markers remain, list them in a line or two. Then ask whether to finish the setup first (`setup/brand-starter.md`) or test anyway.

## 2. Make three test pieces

Choose three pieces that suit this brand's channels (from `audience.md`) and cover different skills:

1. **A short written piece** on the brand's main channel, e.g. a social post.
2. **A longer written piece**, e.g. a newsletter intro, product email or web section.
3. **A visual**: a single social image or slide as a self-contained HTML file using the brand's colours and fonts from `brand/identity.md`.

Use only the brand files, and pick topics the brand files already cover so nothing needs inventing. Aim each piece at a named audience or persona from `audience.md`, build it from the pillars in `messaging.md`, and say which you used above the piece. If the brand has personas, aim at least two pieces at different ones. Don't lean on anything listed under "What everyone says" in `competitors.md`. If the logo or another asset isn't in `brand/`, leave a visible placeholder such as `[logo]` rather than drawing one. Save the pieces in `work/YYYY-MM-DD/brand-check/` using today's date.

Under each piece, add two short lists:

- **Rules followed:** the brand rules this piece relied on.
- **Invented or assumed:** every fact, number, detail or comparison that isn't in the brand files, such as opening hours, a statistic or a customer anecdote. Be strict: if you can't point to the file it came from, it goes here.

Every item under "Invented or assumed" is a gap. In step 4, deal with it even if the user calls the piece on-brand: either the fact goes into the brand files, or a rule says not to use it.

## 3. Let the user judge

Tell the user where the visual is saved so they can open it in their web browser (open it for them if you can). Then show the user each piece, one at a time, and ask them to reply with a number:

1. On-brand
2. Close, but something's off
3. Off-brand

If it isn't on-brand, ask what's wrong.

## 4. Fix the files, not the prompt

For each piece that isn't on-brand:

- Work out why: which brand file was missing something, too vague, or contradicted itself.
- Show the user the exact edit you'd make to that file, such as a new banned word, a clearer rule or a better example line. Make the edit once they agree.
- If the problem is broad enough to matter in every task, also add a rule to the "Brand rules" section of `AGENTS.md` (10 rules at most).
- Remake that piece from the updated files and ask again.

## 5. Finish

When all three pieces are on-brand, say so and summarise what changed in the brand files. If `outputs/` has no example for a channel one of the pieces covers, suggest saving that piece there as an example of what good looks like.
