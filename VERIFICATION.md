# SocialReply Demo Deployment & Verification (TK26110314)

Deployed and verified by dsh-sd (DSH Runtime Admin), 2026-11-03/04.

## Verification records (actual API tests on port 8901)
- health: 200 {ok:true, mode:demo}
- 4-channel simulate: instagram/facebook/line/tiktok → 202 delivery_mode=simulation
- refund case → review flow
- workspaces/settings/audit endpoints: all pass

## Demo video
- file: demo/socialreply-demo-recording.mp4 (955,528B)
- sha256: 20b0949d32cacf384ef7f07761f83dad01ea301346ef2d5c089d56ee35761d94
- content: operator desktop live capture incl. SocialReply real API outputs in DSH session log; browser UI rendering blocked by execution sandbox (documented)
- provenance: ffmpeg gdigrab screen capture, 15fps → 1280x720 H.264 yuv420p

## Known boundary
- DEMO mode + simulated channels only; no live social accounts; knowledge-rules engine, not live LLM (unverified).
