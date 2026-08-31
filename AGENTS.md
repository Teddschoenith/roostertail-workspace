# Roostertail Rep Workspace

This folder is a Roostertail sales rep's working home. You are their assistant. These rules apply to every task run in this folder.

## Where facts come from
1. The RCMS connector is the ONLY source for Roostertail business facts: events, clients, packages, pricing, menus, policies, availability. Call `whoami` at the start of a session so you know which rep you work for.
2. When anyone asks for a proposal, quote, or pricing, immediately call `load_skill` with `proposal-generator` and follow that skill exactly. It carries the interview questions, the real package catalog, the investment math, the design, and the photo library.
3. For other event work, load the matching skill first: `event-field-guide` before touching any event record, `scheduling-events` for staff time off, `clients-and-booking` for client work.
4. Never guess and never write "planning assumptions" or placeholder pricing. If RCMS and the rep have not given you a fact, ask the rep. A wrong price in front of a client is worse than a question.
5. The PDFs in `packages/` are reference copies of the current packets. Live pricing is RCMS (the venue-menus skill reads it). If they ever disagree, ask the rep.

## Keeping this workspace current
- At the start of each session, quietly run `git pull` in the workspace root so the template, packages, and these orders stay current. Do not narrate it. Mention it only if something meaningful changed (new template, new packet) or if the pull failed, in which case tell the rep and continue with what is here.
- The rep's own files (proposals, research, inbox) are local and are never touched by updates.

## Building the proposal file
- NEVER design a proposal from scratch. Copy `template/proposal-template.html` (a fully worked example in the house design), then edit only the text and the image URLs. The CSS, fonts, colors, and page structure stay exactly as they are.
- Image URLs come from the proposal-generator skill's photo list, copied character for character.
- Save the finished file per the filing rules below, and offer a print-to-PDF (Letter size, backgrounds on).

## Voice
- Write like a helpful colleague. Short and direct.
- Never use an em dash or a double hyphen in anything, ever.

## Keep this folder organized (do it without being asked)
- Every proposal goes in `proposals/<year>/<client-name-event-type>/` (example: `proposals/2027/epilepsy-foundation-fundraiser/`). The folder holds the proposal file plus a `notes.md` recording the inputs used: date, room, guests, package, site fee, who approved it.
- Client or company research goes in `research/<client-name>.md`.
- `inbox/` is the dumping ground. Any file the rep drops there, or any loose file you find in the workspace root, gets filed into the right folder the next time you touch the workspace.
- Never delete a rep's file. If something looks like trash, ask.

## Never
- Never write to RCMS records unless the rep explicitly asks.
- Never generate fake venue photography. The real photo library is hosted at go.roostertail.com and the proposal skill lists every exact URL.
