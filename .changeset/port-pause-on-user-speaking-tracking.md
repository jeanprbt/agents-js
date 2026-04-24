---
"@livekit/agents": patch
---

docs(voice): add scaffolding and Python refs for resume_false_interruption tracking livekit/agents#5535

Adds a `PausedSpeechInfo` interface and `_pausedSpeech` field placeholder on
`AgentActivity`, and updates TODO markers in `onStartOfSpeech`,
`interruptByAudioActivity`, `onEndOfSpeech`, and `onFinalTranscript` with
Python `// Ref:` pointers from Python PR #5535. No runtime behavior changes —
this lays the groundwork for porting the pause / resume / false-interruption
pipeline from Python, and incorporates the agent_state-preserving fix from
#5535 once the base feature is wired.
