# Feiliu Home Design for Codex

A Codex plugin containing the `feiliu-home-design` Skill. The Skill fetches the canonical prompt from this repository's `main` branch every time it is invoked, so updating the prompt file does not require updating the Skill/plugin.

## Install once

1. Make sure Codex CLI is available on the computer. In PowerShell, add this repository as a plugin marketplace source:

   ```powershell
   codex plugin marketplace add pridecai1989-czh/home-designer
   ```

2. Open or restart the Codex desktop app and open the Plugins Directory. Select the "Home Designer Team Skills" marketplace, then install "Feiliu Home Design".
3. In a task, type `$` in the composer and choose the Feiliu Home Design skill from autocomplete. Attach the current floor plan and client needs.

## Use

The Skill fetches and verifies the latest prompt at:

https://raw.githubusercontent.com/pridecai1989-czh/home-designer/main/feiliu-home-design-prompt.md

If it cannot retrieve the prompt, it must stop instead of using an older copy. The prompt is in a public GitHub repository, so anyone can read it.

## Update the prompt

Edit `feiliu-home-design-prompt.md` on `main`. The next Skill invocation fetches the new contents. No Skill/plugin reinstall is needed for prompt-only edits.
