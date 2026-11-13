# MotownPocket

Focused MVP: Four-bar Motown/soul pocket desk using live FluidR3 GM instrument samples (bass, drums, Rhodes).

Set BPM (60-180), key, and 4-chord progression. Play with lookahead scheduler on AudioContext clock. Live changes (mutes, tempo, chords) apply on next step. Stop silences immediately.

Export WAV (48 kHz, 24-bit stereo, exact bar length, first downbeat at sample 0, seamless loop by folding tail, peak ≤ -1 dBFS) and matching MIDI (per-chair tracks, tempo/time sig).

Settings persist in localStorage.

**Free** for now. Recommended pricing: one-time $14 on Gumroad (or Lemon Squeezy). Best place to sell: Gumroad for simple license keys, or integrate WorkinWithAI entitlement.

Distinct from prior pocket desks (PocketBass, GrooveFour, etc.) by focusing on classic Motown rhythm section feel.

## Acceptance checks (section 9)
1. Export at 92 BPM, 8 bars, 48 kHz: exact sample count calculated, first transient near 0.
2. Loops seamlessly in DAW, no drift.
3. Tab switch stops cleanly.
4. Live changes within one bar.
5. Missing samples named in UI.
6. Pads sustain (envelopes).
7. No @main, no Math.random in export, voice names match samples.

Built per WorkinWithAI Audio Engine Rules.
