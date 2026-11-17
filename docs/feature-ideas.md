# Feature ideas

Recorded on 2026-11-10. This is an ideas backlog, not an implementation commitment.

## Teleprompter — user's particular interest

Goal: read a script while speaking to the camera with a more natural gaze. Place the text immediately below the MacBook camera, centered around the notch, to minimize looking away from the lens.

Potential first version:

- Paste or edit a script and display it in a compact panel below the camera.
- Adjust font size, text width, and scrolling speed so the script stays readable near the lens.
- Start, pause, and resume scrolling; support manual scrolling and keyboard controls.
- Keep scripts and reading progress locally.
- Let the user explicitly open and close reading mode, and avoid interrupting the script with agent cards while reading. Work out how pending approvals should remain visible.

Possible later enhancement: follow speech to advance the script, subject to evaluating speech-recognition feasibility, permissions, and privacy. A basic teleprompter does not need camera or microphone access.

Validate placement and readability during a real video call or recording: the key outcome is a natural gaze, rather than merely fitting more text on screen.

## Other ideas

- [ ] Volume and brightness controls: show adjustments and provide controls in the notch.
- [ ] Camera mirror: a quick preview before joining a call, activated explicitly with camera permission.
- [ ] Clipboard history: search and recover copied text, links, and images; design exclusions for sensitive content, retention, and deletion before implementation.
- [ ] macOS Shortcuts: launch user-selected automations from the notch.
- [ ] Quick notes and tasks: capture ideas and pending work without switching apps.
- [ ] Reorderable widgets: let users choose which sections appear and their order.
- [ ] Multiple simultaneous timers: extend the current focus/break timer with independent countdowns.

Comparison sources consulted:

- https://boringnotch.com/
- https://getnotchnook.com/changelog

Nosy Notch already includes music, calendar, a file shelf/AirDrop, a focus timer, battery notices, and agent integrations; the ideas above extend that existing feature set.
