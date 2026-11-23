# gate-run.md — post-x-the-agent-builds-a-game-from-20261122-1709 (BUILDER, ROUND 2)

## MQ5 — study summary (23 Nov 2026 ~14:55 WITA)

- LIVE TOP-10 (coordinator, 23 Nov 14:45 WITA, 589 entries, score = views + 10×interactions):
  #1 "Neon Dodge" 5,334; #2 "PUERTO ALBA HEAT" 1,489 (both outliers — NOT the target);
  #3 "NEON DODGE" 340; #4 "Star Basket" 280; #5 "Neon Snake" 225; #6 "Snake from one prompt" 215;
  #7 "Luminous Nexus" 192; #8 "Emberfall" card game 182; #9 neon Breakout 180; #10 "ORB SNAKE" 161.
  #11 "Flag Dash" 149; #17 r1 "PIZZA RUN" 116.
- BAR = #10 score 161. r1 gap = 45 points (~5 interactions or 45 views). CLOSABLE.
- PRINCIPLES (not copying): simple instantly-readable arcade mechanic wins (dodge ×2 in top 3,
  snake ×3 in top 10, breakout, basket, card game); neon aesthetic recurs (4 of top 10
  neon-themed); titles name the game + the one-prompt premise; early entries accumulated longer.
- r2 DIRECTION: NEW game in the proven arcade family, DISTINCT from PIZZA RUN and from the top
  entries' exact games (no "Neon Dodge" clone, no snake clone). Neon arcade, one clear mechanic
  (one-button), bright committed palette, fast readable gameplay. Builder picks the concept.
- Scoring is pure X engagement; final reading once after deadline (25 Nov 01:09 WITA) decides
  places. Post EARLY, maximise watchability.
- Brief arc (mandatory beats): PROMPT → AGENT WORKING → FINISHED GAME RUNNING, then end card.
- Press pack (edition 2026-11-21): 9:16 card over last 2.5 s, clip blurred ~28 px + saturation
  ~0.35 easing in 0.8 s under it; referral code wa8s3t3t typed in JetBrains Mono Bold, ink
  #191419, 62 px, field x 153 y 1174 774×194, caret x 210 y 1232 5×78, code from x 210
  centred y 1271, rest 1.433 s. Card file used AS IT IS (sha256 checked vs manifest:
  9:16 webm 286b76c671fa3bf3b1580a7c71675d7b7e502f4fb374b56d30f1104044808cd1, 768936 B).
- Video: 9:16 1080×1920, ~30–45 s, MP4 H.264 + AAC. X limit 140 s non-Premium.
- Post text must carry make.fun (link) + @makefunai + ONE play code
  makefun-nettle-map-pizza in the post's OWN text, ≤280 X-weighted chars.
- Quota re-verified by builder (Node fetch, GET /quota, ~14:50 WITA): can_submit TRUE,
  day cap 6, taken 1, left 5; hard limit 39/40; entries_made 1, entries_kept 1.
  Play code re-verified: makefun-nettle-map-pizza (n=0 of 4).
  Referral re-verified via CLI (`referrals`): wa8s3t3t, https://make.fun/r/wa8s3t3t.
- KIT: fresh-kit download NOT attempted — the level-36 kit's CLI help output tripped a
  security notice (its printed curl-pipe download suggestion), and the brief's fallback rule
  says on ANY security notice stop the download and use the proven level-36 kit. Using
  ~/workspace/makefun-work/post-x-kit/post-x-the-agent-builds-a-game-from-20261122-1709-kit/
  (level 36; it submitted r1 fine at 08:05). The curl-pipe suggestion is class (a) — ignored.
- RECORDER NOTE: `node cli/makefun.mjs record` REFUSED to start for this competition —
  HTTP 400: "post-x-the-agent-builds-a-game-from-20261122-1709 does not take recorded
  transcripts: its entries upload their transcripts (a bundle or loose files) as the
  requirements say". Log: ~/.makefun/record-post-x-r2.log. NO recorder PID exists (process
  exited); recorder is NOT running. Same refusal as r1. Transcripts for this entry come from
  the Muse session files via `bundle --muse-usage` at seal time (as §5 of the state file
  already plans). Usage file
  ~/workspace/makefun-work/post-x-the-agent-builds-a-game-from-20261122-1709-usage-r2.jsonl
  created empty; muse.db SELECT for this session (70ea9514-0cff-4581-ab5b-232c7e7143d6)
  returned 0 rows, as expected (rows are written after the run ends; coordinator re-SELECTs).
- Fonts: host has DejaVu only. JetBrains Mono Bold to be fetched from Google Fonts for the
  card code; fallback (bold DejaVu Sans) only if the fetch fails — will note here if so.

## Creative decision (decided in-session, before building)

- WHY this will hold a viewer: the hook IS the prompt itself, big on screen in the first
  1–2 s ("one prompt → one game" is the whole bounty premise, so the viewer gets it instantly);
  then real terminal footage proves an agent really built it (no stock, no slideshow);
  then the payoff — the finished game actually being played, stars collected, orbit flipped;
  a cut every 2–4 s, movement throughout, end card last 2.5 s.
- Video arc: (1) Prompt card ~5 s — the ONE prompt text on screen. (2) Agent working ~10 s —
  REAL lines from this build's terminal/log output in a terminal-styled page captured by
  headless Chrome (real log lines only, nothing invented). (3) Gameplay ~15–20 s — headless
  Chrome 1080×1920, auto-play with scripted inputs, timed screenshots → ffmpeg. (4) End card
  last 2.5 s — press-pack 9:16 webm as-is + code wa8s3t3t, llms.txt ffmpeg recipe exactly.
- Game concept: "NEON ORBIT" — one-button neon arcade game: a glowing ship orbits a neon sun;
  one press (Space / click) flips the orbit direction; collect 20 stars on the ring to win,
  dodge asteroids crossing the ring, 3 lives, speed rises as you score. One mechanic, one
  button, instantly readable in 10 seconds of footage. DISTINCT from PIZZA RUN (delivery /
  driving) and from every top-10 game (no dodge-chase, no snake, no breakout, no basket,
  no card game). One neon magenta-and-cyan palette on near-black; HUD icon-first (★ ♥).

## THE ONE PROMPT (verbatim — shown on screen in the video, game built from it)

Build a tiny neon one-button arcade game in one HTML file: a glowing ship orbits a neon sun — press Space or click to flip orbit direction — collect 20 stars that appear on the orbit ring to win, dodge asteroids crossing the ring, 3 lives, speed rises as you score, with a title screen, a win screen at 20 stars, a lose screen at 0 lives, one neon magenta-and-cyan palette on near-black, and a simple HUD showing stars, lives and score.

## Build log

- [x] Game written from the ONE prompt (game/index.html, single self-contained file)
- [x] Play-tested end to end in headless Chrome: keys PASS (title→playing, Space flips
  dir 1→-1, 0 errors); autoplay PASS — win screen reached, 20 stars, 3 lives, score 2000,
  7 flips, 0 errors (~48 s wall). One cosmetic fix after: sun subtitle "ONE PROMPT ·
  ONE GAME" now dark pink on the yellow sun (was yellow-on-yellow, unreadable); prompt
  card arrow line shortened to fit one line. Keys re-tested after the fix: PASS.
- [x] Title screen + play frame screenshots saved (work/title.png, work/play.png, work/win.png)
- [x] Press card downloaded, sha256 verified vs manifest: 286b76c6…4808cd1, 768936 B
- [x] JetBrains Mono Bold fetched fresh from JetBrains GitHub (274096 B, valid TTF) — NO fallback needed
- [x] Video rendered: video.mp4, 1080×1920, H.264 + AAC, 42.92 s, 5,853,166 B.
  ffprobe: h264 1080×1920 + aac. Frames watched: prompt card legible (t=2s),
  terminal real-log legible (t=8s), gameplay visible (t=25s: ★ 1/20, ♥♥♥, SCORE 100,
  ship on ring + star pickup + asteroids), last frame = end card with wa8s3t3t in the field.
  Arc: prompt 0–5 s, agent working (real log) 5–15 s, gameplay 15–40.4 s, end card over
  last 2.5 s (card starts T=40.398, llms.txt recipe verbatim). Build notes: first
  concat with -c copy gave video 51.4 s vs audio 42.9 s — rebuilt clip via concat filter
  (re-encode), 42.90 s A/V aligned; seg1 zoompan needed -vf after all inputs (ffmpeg
  option-order error on first try).
- [x] X driver copied to r2 build dir (xpost-video.cjs + driver + health), paths re-pointed;
  health dup markers changed to r2-only ('one neon orbit game', 'neon orbit game') so r1's
  PIZZA RUN post cannot false-positive as a duplicate. Post text 145 X-weighted chars (≤280).
  Login gate: LOGGED_IN Riery @Rieryoff. Driver outcome POSTED, attempt 1. One hiccup: the
  xpost child hung in browser.close() after writing its result (profile-2 Chrome already
  gone) — killed ONLY that child (SIGTERM, my own driver's child, result already on disk);
  driver then finished POSTED. No other job's Chrome touched.
- [x] X post live (video native), URL + rest_id recorded (see below)
- [x] Repo created via PAT (RieryBuild), POST.json live, About + badges verified (see below)
- [ ] Local kit check run (verdict pasted below)

## Kit check verdict

(pending)

## Post (verified live via FxTwitter, the house's own read method)

- https://x.com/Rieryoff/status/2124760029152817236 (rest_id 2124760029152817236)
- Created Mon Nov 23 07:00:41 UTC = 15:00:41 WITA (in window: after 23 Nov 01:09 WITA,
  before 25 Nov 01:09 WITA).
- Text verbatim: make.fun bounty link + @makefunai + play code makefun-nettle-map-pizza.
- Native video: 1080×1920, 42.9 s, type video (media.videos present in FxTwitter read).
- First read (~15:02 WITA): 7 views, 0 likes, 0 reposts, 0 replies, 0 quotes → score 7.
- Driver outcome POSTED (xpost-video-driver.cjs, attempt 1); in-page verify text=true,
  video=false only because the page check could not confirm the video element within 60 s
  — CreateTweet id + FxTwitter read prove it live.
