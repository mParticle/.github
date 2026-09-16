<!--
Write the description in these eight sections, in this order, in plain English. These notes are for you. Readers
never see them on the page, but they stay in the body's source: delete each note, whole, once its section is written.

Write for someone who was not in the room and reads once: the Why in under a minute, the rest on one screen. Keep
sentences short. Use the words your readers already use for the service, the region and the product; expand any
other acronym the first time. Say whether each action is done, in progress or planned.

Never leave a heading with nothing under it: a section that does not apply gets the exact line its note gives. Link
every pull request (repository and number) and every page you name, and say what each is. Why and Programme are
prose for a non-engineer: keep code names out of them. Detail only a reviewer needs — logs, commit hashes, file
lists — goes in the collapsed note at the end.

On a public repository everything here is public and permanent: title, body, branch name, commits, comments. Link
only to pages anyone can open; describe the rest in words. Name no partner, client or provider, no internal system or
team, and colleagues by role, not by name.

Outside contributors: fill Why, What changes, Risks and Size; under each other heading write exactly:
"Not applicable: outside contribution."
-->

## Why

<!-- The problem or the outcome, in one paragraph a non-engineer follows: who feels it, what goes wrong today, and
what is true once this lands. Two to six sentences. The first sentence is the problem or the outcome — for a release,
what it gives users, before its version number — never a file list or a summary of the change. -->

## Programme

<!-- The programme, project or plan this serves — a ticket, an epic, a plan page or an incident — linked where the
reader can open it. Where the source is a person's request, say so and link the record. If a keyword such as "Closes"
links or closes your ticket, write it here. If it serves none, write exactly: "Standalone change, no programme." -->

## What changes

<!-- Before and after, in the reader's terms. Say whether documentation, the changelog or a runbook moved with it, or
why not. Where the change is visible, a screenshot or short recording goes here. For anything longer than a screen,
close with where a reviewer starts reading, what to check first and what was deliberately left alone; for a small
change, one sentence of before and after is enough. The code shows how; a file list, if a reviewer needs one, goes in
the collapsed note at the end. -->

## Linked work

<!-- Three lines with these prefixes, every pull request named with its repository and number and linked.
"Depends on:" what must land first — a pull request, a data load, a flag created elsewhere, a decision.
"Unblocks:" what waits on this.
"Related:" the rest.
Leave out a line that has nothing. If all three are empty, write exactly: "None." -->

## Rollout

<!-- How the change reaches production, in four parts with these prefixes, in this order.
"Path:" what merging deploys, applies or publishes, or which release carries it; switched off ("dark") or live; in
what order; any timing constraint. For a schema or data change, whether it runs before or after the code that needs
it, and whether it is reversible.
"Feature flags:" each flag by name in backticks; off or on before and after the merge; who turns it on and what they
check first; when it is removed. Or: "Feature flags: none."
"Turning it off:" how to undo the change and how long it takes. A flag or remote switch takes seconds; a redeploy of
the previous version, minutes; a down-migration or restore, say how long and what data it touches; a library, the
next release — a published version cannot be recalled. Say what each leaves behind.
"What we watch:" the dashboard, alert or query; its value today; how often it is checked during the roll-out and the
number that means "turn it off"; what tells you the change is settled.
If nothing changes in production or in any release, write exactly: "Nothing changes in production; if this is wrong,
revert the pull request." Any change to what production does, stores or carries in load writes the four parts. -->

## Risks

<!-- One bullet per risk you considered, all of them, in three parts separated by semicolons: the risk; what prevents
or contains it; how we would see it. A risk nothing prevents says so: the risk; "not addressed", and why; how we
would see it. For a text-only change, one bullet: "Nothing can break beyond the text itself."
Last line, always: "Risk class: low." or "Risk class: higher — " followed by what could break. Higher means the change
could materially affect what production does — its behaviour, performance, money or data — or cannot be quickly
undone. Everything else is low. No approver's name here: GitHub's review records who approved. -->

## Who

<!-- Six lines with these exact prefixes.
"Written by:" the author — a person, or an automated coding agent named as such — and the plan, incident or request
it came from, linked.
"Code reviewed before opening:" who reviewed the code before this was opened, when, and what was fixed; or "no one".
"Design reviewed before opening:" who reviewed the intent or design, linked; or "no one".
"Decision this implements:" the ticket, design decision or agreement, with its date and a link where the reader can
open it — the record, not the person who asked.
"Checked:" what ran or was read before opening — tests, a local run, a query — and when, in words.
"Not checked:" what did not run, and why. -->

## Size

<!-- "Hand-written:" a lines figure and a files figure — what you wrote by hand, generated files excluded.
"Generated:" write "none", or the number of generated files, each named with the tool that made it in the collapsed
note at the end, never here.
Above 400 hand-written lines or 15 hand-written files, either split the change into smaller pull requests that each
merge on their own, or add a line "Why one pull request:" and say why this is the right shape. A team may set a
different threshold in its own repository's template. -->

<details>
<summary>Notes for reviewers</summary>

<!-- A collapsed note the reader opens by choice: the file list, generated files and the tools that made them, the
numbers behind a claim, test output or a query a reviewer may want. If you have nothing to put here, delete the whole
block, from <details> to </details>: an empty one shows as a toggle that opens onto nothing. -->

</details>
