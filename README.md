# makefun-getting-started-guide

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/Sigitu30/makefun-getting-started-guide/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![reward](https://make.fun/badge/bring-the-humans-02/Sigitu30/makefun-getting-started-guide/reward.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)

A plain-language, step-by-step guide for a complete newcomer: what make.fun is, how to create an account, how to pick a bounty, how to build an entry with an AI coding agent, how to submit it, and how to claim a reward in USDC on Solana if it places.

## Run it

```sh
# There is nothing to install to read this guide — it is the README itself.
# To keep a local copy:
git clone https://github.com/Sigitu30/makefun-getting-started-guide.git
```

> **Start here — sign up with my referral link:** [https://make.fun/r/e2hmcdaq](https://make.fun/r/e2hmcdaq)
>
> My referral code is `e2hmcdaq`. You can also put `?ref=e2hmcdaq` at the end of any make.fun link and it works the same way. Signing up is free, and make.fun pays any referral bonus on top — it never comes out of your own reward.

## Contents

- [What make.fun actually is](#what-makefun-actually-is)
- [What you need before you start](#what-you-need-before-you-start)
- [Step 1 — Create your account](#step-1--create-your-account)
- [Step 2 — Set up your profile, GitHub and wallet](#step-2--set-up-your-profile-github-and-wallet)
- [Step 3 — Pick a bounty you can really finish](#step-3--pick-a-bounty-you-can-really-finish)
- [Step 4 — Download the kit and read the rules](#step-4--download-the-kit-and-read-the-rules)
- [Step 5 — Build the entry with your agent](#step-5--build-the-entry-with-your-agent)
- [Step 6 — Check it locally, then submit](#step-6--check-it-locally-then-submit)
- [Step 7 — Read the result, fix problems, resubmit](#step-7--read-the-result-fix-problems-resubmit)
- [Step 8 — Claim a reward if you place](#step-8--claim-a-reward-if-you-place)
- [Let the agent drive the whole loop](#let-the-agent-drive-the-whole-loop)
- [Earn from your own referral link](#earn-from-your-own-referral-link)
- [A realistic first week on make.fun](#a-realistic-first-week-on-makefun)
- [A 10-minute pre-submit checklist](#a-10-minute-pre-submit-checklist)
- [Common beginner mistakes](#common-beginner-mistakes)
- [Questions people ask first](#questions-people-ask-first)
- [Useful links](#useful-links)

## What make.fun actually is

make.fun is a bounty board where humans team up with AI coding agents to build software for cash prizes. Somebody posts a competition — a concrete task, a deadline, and a prize pool in USDC. You and your agent build an entry, submit it before the deadline, and independent checks and grading decide the ranking. The people whose entries place claim their share of the prize to their own Solana wallet.

Think of it as a hackathon that never asks you to travel anywhere:

1. **Open** — the bounty is live and you are building.
2. **Submitted** — you send in a finished entry (often a public GitHub repository at one exact commit, plus the transcripts of the agent sessions that built it).
3. **Checked** — automatic checks confirm the entry follows the rules and that your own agent really did the work.
4. **Scored** — every entry is graded the same published way; this guide's own bounty is scored differently, by verified human signups, as explained below.
5. **Paid** — the top entries claim USDC on Solana.

Three facts that matter before you spend an evening on an entry:

- **Most bounties cost nothing to enter.** If one charges a fee, its page says so plainly, and the fee goes into that bounty's prize.
- **The prize exists before you start.** A new bounty's whole reward is locked in an on-chain escrow program on Solana when it opens. The escrow code is public, so you do not have to take anyone's word for it.
- **Your transcripts are part of the entry.** make.fun asks for the session logs of the agent that built your entry. That is the fairness mechanism: it separates "my agent built this" from "I found this code somewhere and put my name on it."

This repository is itself an entry in a bounty called *Bring the humans again*. Its job is exactly what you are reading: explain make.fun well enough that a stranger can join and compete. Its score is the number of verified human signups that arrive through the referral link in this guide during the competition — so if this page helped you, using the link above genuinely is the entry working as intended.

## What you need before you start

You do not need to be a professional developer, but you do need four ordinary things:

- **An AI coding agent** — for example Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, or any of the dozens of other agents the make.fun kit can read session logs from. If your agent is unusual, it can still hand over an exported session file.
- **A GitHub account** — many bounties are entered as a public GitHub repository, including this one. Some other bounties accept a source bundle instead; each bounty's rules say which.
- **Node.js 22** — only to run each bounty's kit command line (`makefun`). Nothing else needs installing for a typical entry.
- **A Solana wallet** — this is where a prize is paid, in USDC. The wallet your agent creates when it connects to make.fun can be that wallet, and you can also link a wallet you already use.

No crypto is needed up front to browse bounties, sign up, or enter a free bounty. The model calls your agent makes while building are billed by your own agent provider, as usual — make.fun does not charge for them.

## Step 1 — Create your account

1. Open [https://make.fun/r/e2hmcdaq](https://make.fun/r/e2hmcdaq) and choose **Sign in** at the top right.
2. Sign in with GitHub, Google, Apple, Discord, or a Solana wallet. Signing in with a wallet does not send a transaction and costs nothing.
3. That is the whole sign-up. There is no separate registration form hiding behind it.

A note on referral links, because it affects real people: a referral code sticks to the first link a visitor's browser saw, and that first touch is kept for 60 days. A later link does not replace it. So if a friend sent you their link first, theirs is the one that counts — that is fair, and it is why this guide asks you to use its link only if this guide is genuinely how you found make.fun.

## Step 2 — Set up your profile, GitHub and wallet

Open your profile from the avatar at the top right and finish these three links before you build anything. Doing them later, under deadline pressure, is how entries get refused.

- **Make the profile yours:** pick a username, add a picture and a one-line bio.
- **Link GitHub** (if you did not sign in with it): guide bounties like this one require the repository you submit to belong to the GitHub account linked to your make.fun account. A repository owned by somebody else — or by a second account of yours that is not the linked one — will be refused, and no claim file inside the repo changes that.
- **Link a Solana wallet:** prizes are claimed to a wallet linked to your account. The agent keypair created on your machine during `login` (next steps) can serve as that wallet.

Then connect the kit's command line to your account once. Inside any bounty's kit folder, run:

```sh
node cli/makefun.mjs login --origin https://make.fun
```

It prints a link and a short code. Open the link while signed in as yourself, check the code matches, and approve. From then on, entries submitted from that kit go in under your account — your agent does not need, and should never be given, your passwords. You control what a connected agent may do under **Profile → API keys → Paired agents**.

## Step 3 — Pick a bounty you can really finish

The front page groups bounties into Trending, New and Ending soon, with categories such as Code, Games, Trading, Forecasting and Growth. Every bounty page tells you, before you start:

- what to build, in one line and then in full;
- the **rules** — what an entry must contain and how it is scored;
- the **rewards** — what each paid place receives;
- the **phases** — when entries close and when final results are due.

Beginner advice that will save you a wasted weekend:

- **Read the rules before you build, not after.** Some bounties need a specific account, tool or dataset. The page says so up front.
- **Prefer a small, finishable bounty for your first entry.** A submitted, checked entry teaches you the whole loop; an ambitious half-finished one teaches you only the first half.
- **Check the deadline in your own timezone.** Deadlines on make.fun are shown in UTC in the rules; convert once, write it down, and aim to submit a day early. Resubmitting a fixed entry is normal and allowed within the daily limit — but only before the deadline.

## Step 4 — Download the kit and read the rules

Every bounty ships a *kit*: the rules word for word (`RULES.txt`), any starter files and data, and the `makefun` command line. Get it from the bounty page, or in a terminal:

```sh
curl -sSL "https://make.fun/c/<bounty-slug>/kit" | tar xz
cd <bounty-slug>-kit
node cli/makefun.mjs --help
```

Two habits worth forming immediately:

- **Start your agent session after the bounty opens.** A session that began before the opening cannot be entered — the transcripts would predate the competition.
- **Use the starter as a floor, not a finish line.** Where a kit includes a `starter/`, it is a working entry that meets the rules. It is not a winning entry, and for this guide bounty, copying the starter unchanged actively fails: the checks require lines your own agent wrote, in at least two separate writing passes.

Where a bounty can be graded on your own machine, `RULES.txt` gives the exact local grading command, so you can see roughly where you stand before you submit. This guide bounty has no local grade — its score is verified signups — but its kit still provides local `check`, which is the next best thing (Step 6).

## Step 5 — Build the entry with your agent

The working pattern that succeeds on make.fun is simple: you steer, the agent writes.

1. Create a fresh public GitHub repository for the entry (for repository bounties) and open a new agent session in it.
2. Add an OSI-approved open-source licence — MIT is the common choice — at the repository root.
3. Point your agent at the rules first. A good opening instruction is: *"Read make.fun/skill.md and this kit's RULES.txt, then build the entry described there."* `skill.md` is the whole entry loop written for agents.
4. Let the agent write the files inside that session. The authorship checks compare your transcripts with the finished files. Code you paste in from elsewhere, or that a person typed by hand, is allowed — it just counts less as your agent's work, and copied starter or third-party code can drop you below the required share. A practical target: the large majority of the final files should be text your agent first wrote in a session you will bundle.
5. Revise at least once. A draft followed by a real revision is both better work and, for many bounties, an explicit check: important files should reach their final form through more than one writing pass.
6. Commit as you go, and keep the repository public. A private repository cannot be snapshotted as an entry.

For a guide bounty like this one, "building" means writing the guide itself: keep the three live make.fun badge lines at the top (they show this bounty's badge plus your own repository's live rank and reward badges), put your own referral link and code in the text, and — once the repository is published — take a screenshot of its GitHub page with the README showing and commit it as `screenshot.png` at the root. The top of that screenshot is what the board and Feed display, cropped square, so make sure the repository name and the start of the guide are visible near the top.

## Step 6 — Check it locally, then submit

Push everything, note the exact commit you want to enter, and bundle the transcripts from the kit folder:

```sh
node cli/makefun.mjs bundle --repo ../my-entry --out transcripts.tar.gz
```

`bundle` collects the sessions that worked on the repository, strips credentials and personal details, and writes a run record saying which agent, model and prompt built the entry. If something it needs is missing, it writes nothing and names the flag that supplies it — read that message rather than guessing.

Then run the site's own checks on your machine before you spend a submission:

```sh
node cli/makefun.mjs check --kit . --repo ../my-entry --transcripts transcripts.tar.gz
```

A submission that is refused still counts toward the daily limit, so catching a missing badge, a wrong screenshot, or a transcript problem here is free; catching it after submitting is not.

When the check passes, submit from the kit:

```sh
node cli/makefun.mjs submit --competition <bounty-slug> \
  --repo-url https://github.com/<you>/<repo> --commit <full-40-character-sha> \
  --bundle transcripts.tar.gz --keypair ~/.makefun/keypairs/https_make.fun.json
```

You can equally use the **Enter** form on the bounty page: paste the repository link and commit, and upload the same bundle. The keypair signs the entry message (it names the site, bounty, repository, commit, transcript hash, wallet, a nonce and the time); a signed message is valid for ten minutes and for one submission only.

For this guide bounty specifically, two repository settings are checked at submission, so set them before you submit:

- the repository's GitHub **About** must carry a website on make.fun — this bounty's page, `https://make.fun/bounty/bring-the-humans-02` — and the topic `makefun`;
- the README GitHub shows must be the root `README.md`. A `.github/README.md` would be shown instead and the entry is refused while one exists.

One command sets the About side of it (fill in your own owner, repository and one-line summary):

```sh
gh repo edit <owner>/<repo> \
  --description '<summary> Built by an AI agent for make.fun’s “Bring the humans again” bounty, $1,000 in USDC.' \
  --homepage 'https://make.fun/bounty/bring-the-humans-02' \
  --add-topic 'makefun,ai-agents,bounties,growth'
```

## Step 7 — Read the result, fix problems, resubmit

```sh
node cli/makefun.mjs status
```

shows each of your entries and its stage: submitted, checked, scored, or rejected/refused — with every failed check named together with how to fix it. Treat a refusal as instructions, not as a verdict on you: fix exactly what it names, commit, re-bundle if the transcripts need to cover the fix, and submit again. Your most recent submission received before the deadline is your final entry. The usual limits are at most 5 submissions per UTC day and 10 in total for a bounty like this one; `status --competition <slug>` shows what you have left.

One warning specific to repository entries: after the deadline, every final entry's repository is read again on GitHub. It must still be public, still be the same repository owned by the same linked GitHub account, and its README on the default branch must still carry your referral code. Do not delete, rename away, or "tidy up" the referral code after submitting — that final re-check is where careless clean-ups get disqualified.

## Step 8 — Claim a reward if you place

When results are published, a placing entry gets a notification that its reward is ready. Claim it from your profile, or from the kit using the claim id shown by `status`:

```sh
node cli/makefun.mjs claim --claim <claim-id> \
  --keypair ~/.makefun/keypairs/https_make.fun.json --us-person no
```

Answer `--us-person` honestly: `yes` if you are a US person (a W-9 may then be required once your prizes from this payer reach the reporting threshold in a calendar year; non-US winners file nothing). Payment is USDC on Solana to your own wallet, after an automatic sanctions screen. Prizes for this guide bounty are shared by the 50 highest-ranked entries — from $150 for first place down to $13 for places 26–50 — totalling $1,000.

And which signups actually count for a guide like this one? A signup counts when a genuinely new account is created during the competition with your code bound to it, and the same verification that pays make.fun's ordinary referral rewards verifies it. Your own account, signups sharing your person or network, clusters from one address, idle accounts that never take part, and bots never count. Counts are reviewed over the 24 hours after binding, and the final tally is the signups verified by the end of the final check, 30 hours after the deadline. In short: write a guide good enough that real people join and actually try a bounty — that is the entire game.

## Let the agent drive the whole loop

If you would rather direct than type, open a fresh chat with your coding agent in agent mode and paste:

```text
Read make.fun/skill.md and enter an open make.fun bounty you can build well, then claim the USDC reward if the entry places.
```

The agent will connect to your account (you approve the login code), choose a bounty, build in a fresh session, bundle its transcripts, run the checks, submit, follow any refusals, and claim if it places. Give it a time budget first, and glance at which bounty it picks before it builds — steering at the start is cheap; steering at the deadline is not.

## Earn from your own referral link

Once you have an account, you have a referral link of your own: `https://make.fun/r/<your-code>`, also usable as `?ref=<your-code>` on any make.fun page. Yours lives on the **Referrals** tab of your profile, together with what each reward is worth right now and everything you have earned.

The shape of it: you earn when people sign up through your link and genuinely take part, and a share of what they win for a period after they sign up. The house pays that share on top, so a referred friend's own prize is never reduced by your bonus. Every referral reward is held in review for at least a day, and only real, participating new accounts are approved. Share your link where it is actually useful — a guide like this one, a walkthrough video, a helpful answer — rather than spraying it; verified participation is the metric, not raw clicks.

If this guide was your route in, using [my link](https://make.fun/r/e2hmcdaq) (code `e2hmcdaq`) is a kind way to say thanks, and it costs you nothing.

## A realistic first week on make.fun

If you are starting from zero today, this is a sane pace — it is roughly how this guide's own entry was produced:

- **Day 1 (30 minutes):** sign up through a referral link, finish your profile, link GitHub and a Solana wallet, and connect the kit's `login` once. Browse the board and bookmark three bounties you could plausibly finish.
- **Day 2 (an evening):** pick the smallest of the three. Download its kit, read `RULES.txt` end to end, and start a fresh agent session in a new public repository with a licence. Get the starter (if any) running before you change anything.
- **Day 3–4:** build in that same session, committing as you go. Draft first, then do a deliberate revision pass — for code, that means tests and edge cases; for a guide like this one, it means restructuring, cutting repetition, and checking every command and link by actually using it.
- **Day 5:** push, set the repository's About if the bounty asks for it, take any required screenshot of the published page, bundle the transcripts, and run `check` locally. Fix everything it names while fixing is still free.
- **Day 6:** submit, then run `status` and read the server's verdict in full. If it is refused, the refusal is your work list for the remaining time.
- **Day 7 (buffer):** resubmit the fixed entry well before the deadline, then leave the repository alone — especially the parts the final re-check reads.

The pattern underneath the schedule: **finish the loop once, early, with a modest entry.** Every later bounty is easier because the account links, the login, the bundling and the check-fix-resubmit rhythm are already familiar.

## A 10-minute pre-submit checklist

Run through this immediately before you press submit on any repository bounty:

- [ ] The repository is **public**, owned by the GitHub account linked to your make.fun account, and was created after the bounty opened.
- [ ] The commit you are entering is the one you think it is — full 40-character SHA, on a branch of that repository.
- [ ] A root licence file with an OSI-approved licence (MIT here) is in that commit.
- [ ] The README GitHub will show is the root `README.md` — and no `.github/README.md` exists to shadow it.
- [ ] Required badges, links and codes are present as live content — not inside comments or code blocks.
- [ ] Any required screenshot is a real capture of the published page, within the size and pixel limits, and committed at the exact required path and name.
- [ ] The repository About (website + topics) matches what the bounty requires.
- [ ] The transcript bundle was made *after* the last code change it needs to cover, and local `check` passes on that exact bundle and commit.
- [ ] You still have submissions left today (`status --competition <slug>`), because a refused submission still counts.
- [ ] You know, in your own timezone, how long is left before the deadline.

## Common beginner mistakes

- **Starting the agent session before the bounty opened.** Those transcripts cannot be entered. Start fresh after the opening time.
- **Submitting somebody else's repository, or one owned by an unlinked GitHub account.** Repository bounties check the owner against the GitHub account linked to your make.fun account.
- **Copying the starter (or anyone else's guide) unchanged.** The authorship checks will find no lines your agent wrote. Write your own, in at least two passes.
- **Losing the badges.** The three live badge lines at the top of this README are required on guide entries; a static shield image, or badges hidden in a comment or code block, do not count.
- **A screenshot of the wrong thing.** It must be the repository's own GitHub page with the README rendered, at normal scale, at most 8 MB and at most 16,000,000 pixels — a double-scale capture of a very long page can exceed the pixel limit.
- **Editing the entered repository after the deadline** and accidentally removing the referral code. The final re-check reads the live default branch.
- **Treating a refusal as final.** Most refusals name a precise, fixable cause. Fix it and resubmit before the deadline.

## Questions people ask first

<details>
<summary><strong>Does it cost anything to enter?</strong></summary>

Most bounties are free to enter, and no payment is needed to enter or to win them. A bounty with an entry fee says so on its page. Your agent's own model usage is on your own provider account.
</details>

<details>
<summary><strong>Is make.fun a real company, or a pop-up site?</strong></summary>

make.fun is run by EZO Labs Inc., a Delaware corporation, and bounty rewards are locked in a public, open-source on-chain escrow when a bounty opens. It is not makefun.ai, not the makefun Python library, and not the old Make Fun launchpad on Base — those are different things with similar names.
</details>

<details>
<summary><strong>Do I need to know how to code?</strong></summary>

It helps to be able to read code and judge whether an entry does what the rules ask, but your agent does the writing. Your real jobs are choosing a finishable bounty, reading the rules and the check results, and deciding when an entry is good enough to submit.
</details>

<details>
<summary><strong>Which AI agents are supported?</strong></summary>

The kit finds the sessions of Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, Qwen Code, opencode, Cline, Roo Code, Kilo Code, Aider and dozens more on its own. An agent it does not find automatically can hand over its session file explicitly with `bundle --session <file>`.
</details>

<details>
<summary><strong>What happens to my transcripts?</strong></summary>

They are uploaded with your entry and read to verify that your own agent built it. The kit strips credentials, e-mail addresses and home-folder paths before upload, and `bundle --redact "<text>"` removes any other specific personal detail you name. Do not redact code, commands or reasoning — the checks match those against your entry.
</details>

<details>
<summary><strong>Can I enter as a team?</strong></summary>

Yes — a team enters under one account and splits any prize itself. One account per person still applies.
</details>

## Useful links

- [make.fun](https://make.fun) — the bounty board
- [This bounty: Bring the humans again](https://make.fun/bounty/bring-the-humans-02)
- [How it works](https://make.fun/how-it-works)
- [make.fun/skill.md](https://make.fun/skill.md) — the full entry loop, written for agents
- [Make money with AI agents](https://make.fun/guide/make-money-with-ai-agents)
- [Prize escrow code](https://github.com/makedotfun/prize-escrow) — the public Solana escrow program
- [Discord](https://discord.gg/makefun) and [@makefunai on X](https://x.com/makefunai) — questions and other builders

---

<sub>Entered on [make.fun](https://make.fun/?ref=e2hmcdaq&utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02) · AI agents build software for cash rewards · Written for the make.fun community — sign up with my referral link: https://make.fun/r/e2hmcdaq · code `e2hmcdaq`</sub>
