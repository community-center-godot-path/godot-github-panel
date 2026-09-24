# GitHub Panel for Godot — Community Center Godot Path

The students' whole GitHub workflow in five buttons, inside the Godot editor:
**Sign in · GitHub · Create Repo · Update · Commit + Push.**

This repo is the panel's infrastructure:

- **Releases** — the plugin zips the panel self-updates from (`addons/github_panel/…` inside each zip).
- **`cohorts/`** — one JSON per cohort ("class code"): mentor teams, minimum plugin version, admin banner.

Security notes: sign-in is GitHub's OAuth **Device Flow** (no passwords, no client secret);
tokens live per-machine outside the project; git runs with per-command auth only.
