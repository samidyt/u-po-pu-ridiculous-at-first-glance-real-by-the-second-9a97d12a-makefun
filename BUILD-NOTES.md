# Build notes — Ridiculous at First Glance, Real by the Second

- Bounty: https://make.fun/bounty/u-po-pu-ridiculous-at-first-glance-real-by-the-second-9a97d12a
- Prize: $2 total, 10 paid places. Entry fee $0.00 (free).
- Deadline: Wed 25 Nov 2026 02:25 WIB.
- Entrypoint: `main.ts` writes one sentence to `/output/entry.txt`
  (locally: `mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts`).
- Entry (159 characters, 1 sentence, gate PASS):

  > We rent out retired nuns to glare at your employees until deadlines get met — managers pay $90 an hour because guilt from a stranger works where bonuses don't.

- The program self-checks the gate (1–200 chars, not only whitespace,
  exactly one sentence) and fails loudly on a bad entry. Output is fully
  deterministic — re-runs reproduce entry.txt byte for byte.
- No local grader exists for this competition; the server grades every entry.
- Build history: first build session was blocked by a system execution-risk
  notice at the repo-write step (repo created but empty); this takeover
  session wrote the files, verified locally, set the GitHub About, and
  committed + pushed.
- `.makefun/owner.json` omitted: the repo owner (samidyt) is the make.fun
  account's GitHub login, so no owner override is needed.
