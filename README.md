# HOLO AI v2 · TalkingHead 3D

GitHub Pages static website featuring the MIT-licensed [TalkingHead](https://github.com/met4citizen/TalkingHead) library and the CC0 MPFB example avatar from its repository. Source is loaded from pinned TalkingHead v1.7 CDN; the MPFB model is served from the upstream GitHub repository. The MPFB model is ~36.8 MB, so mobile loading may be slow. Three.js is MIT licensed.

## Current functionality
- Realistic human 3D head with idle facial animations and eye contact via TalkingHead.
- Microphone input via browser SpeechRecognition where supported.
- Voice responses via browser speechSynthesis, without accurate synchronized lip movements yet.
- Permission-gated camera preview and camera switching; no vision inference or upload.
- Typed messages, stop control, sound toggle, mobile-friendly interface.

## Important limitations
- This is a **front-end avatar upgrade**, not yet a real conversational AI. Replies are intentionally rule-based. No AI model or vision model is connected.
- Browser speech recognition may send audio to the browser vendor. The camera preview is local-only.
- Accurate phoneme/viseme lip-sync requires integrating HeadTTS/HeadAudio or another compatible TTS/audio engine; browser speechSynthesis does not expose viseme timings.
- The CC0 MPFB sample may not be the final desired appearance. Replace with an appropriately licensed and compatible rigged GLB for commercial use.
- GitHub Pages cannot host a traditional AI inference server. No secrets or private API keys should be added to public source code.

## Publish
GitHub Settings > Pages > Deploy from a branch > main / root.

## License
Original HOLO AI glue code: MIT. TalkingHead: MIT (see upstream LICENSE). MPFB example avatar: CC0 per upstream TalkingHead README. All third-party copyrights and licenses remain with their respective owners.
