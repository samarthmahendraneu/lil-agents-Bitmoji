# lil agents

<img width="1264" height="814" alt="image" src="https://github.com/user-attachments/assets/2fb0d4d0-f11f-49b8-8d95-14eb03e9375e" />

Tiny AI companions that live above your macOS Dock.

In this fork, **Bruce** and **Sam** stroll across the Dock, idle, think, and open a lightweight AI chat when you click them. It is part desktop toy, part menubar utility, part CLI companion.

The app works with local AI CLIs including **Claude Code**, **OpenAI Codex**, **GitHub Copilot**, **Google Gemini**, and **OpenCode**. You can switch providers from the menubar without relaunching the app.

## features

- Animated Dock companions rendered from transparent `.mov` loops
- Per-character movement tuning, pacing, and positioning
- Click a character to open a themed popover chat UI
- Menubar controls for provider, character size, theme, sounds, and display selection
- Supported providers: Claude, Codex, Copilot, Gemini, and OpenCode
- Slash commands in chat: `/clear`, `/copy`, `/help`
- Thinking bubbles and completion bubbles while the agent works
- Completion sound effects
- First-run onboarding flow
- Sparkle-based app updates

## requirements

- macOS 14.0 or newer
- Xcode 15 or newer for local builds
- At least one supported CLI installed and authenticated

Provider install examples:

- Claude Code: `curl -fsSL https://claude.ai/install.sh | sh`
- OpenAI Codex: `npm install -g @openai/codex`
- GitHub Copilot: `brew install copilot-cli`
- Google Gemini CLI: `npm install -g @google/gemini-cli`
- OpenCode: `curl -fsSL https://opencode.ai/install | bash`

## building

There is no command-line build setup in this repo.

1. Open [lil-agents.xcodeproj](/Users/samarthmahendra/PycharmProjects/lil-agents/lil-agents.xcodeproj) in Xcode.
2. Select the `LilAgents` scheme.
3. Build and run.

## privacy

lil agents itself is a local macOS app.

- The app renders bundled character animations and reads Dock layout information so it can position characters correctly.
- Chat requests are handled by the CLI provider you choose to run on your machine.
- The app does not run its own backend or account system.
- Any network access comes from the provider CLI you use and from Sparkle update checks.

## license

MIT. See [LICENSE](LICENSE).
