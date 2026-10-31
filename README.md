<div align="center">

<img src="screenshots/icon.png" width="128" height="128" alt="Whisker app icon">

# Whisker

### Your dev work and your day, right on your Mac's desktop.

GitLab merge requests, Plane tickets, your repo and your local stack, in calm widgets you can act on.

<br>

[![Download for macOS](https://img.shields.io/badge/Download_for_macOS-F27BA8?style=for-the-badge&logo=apple&logoColor=white)](https://github.com/ialhejaili/whisker/releases/latest/download/Whisker.dmg)

![Latest version](https://img.shields.io/github/v/release/ialhejaili/whisker?style=flat-square&label=version&color=3A1D2F)
![macOS 14 or newer](https://img.shields.io/badge/macOS-14%2B-3A1D2F?style=flat-square)
![Apple Silicon and Intel](https://img.shields.io/badge/Apple_Silicon_%7C_Intel-universal-3A1D2F?style=flat-square)
![Notarized by Apple](https://img.shields.io/badge/notarized-by_Apple-3A1D2F?style=flat-square)

</div>

<br>

![The Whisker desk](screenshots/desk.jpg)

<p align="center"><sub>Every screenshot uses made-up sample data from Whisker's demo mode.</sub></p>

<br>

## Built for your dev work

![Review inbox and Plane tickets](screenshots/dev.png)

**GitLab review inbox.** The merge requests that need you, most urgent first.
- Approve, merge (now or when the pipeline passes), retry a pipeline, read the job log
- Reply to threads without opening the browser
- Failing pipelines, conflicts and replies you owe come to the top

**Plane tickets.** Your work by Doing, Waiting, Todo and Done.
- Create tickets, change state or priority, comment
- Due dates, cycles and priority at a glance
- Each ticket shows its branch and merge request

**Notifications.** Whisker tells you when:
- one of your MRs fails or passes its pipeline, is approved, is ready to merge, gets conflicts, a comment or a thread, or is merged or closed by someone else
- someone moves one of your tickets, or mentions you on any ticket

Click a notification to open the MR or ticket.

<table>
<tr>
<td width="40%" valign="top"><img src="screenshots/repo-stack.png" alt="Repo and dev stack widgets"></td>
<td valign="top">

**Your repo.**
- Branch, ahead and behind, changes, stashes and recent commits
- Fetch, pull, switch or create branches, stash
- The branch's ticket and merge request
- Clean up old worktrees in one click

**Your local stack.**
- Start, stop and restart your dev server, read its log
- Docker Compose up or down, every container's state
- Run your checks with a pass/fail history
- A notification when something breaks

</td>
</tr>
</table>

### From ticket to merge request

<table>
<tr>
<td width="50%" valign="top"><img src="screenshots/new-ticket.png" alt="Creating a Plane ticket in Whisker"></td>
<td width="50%" valign="top"><img src="screenshots/new-mr.png" alt="Creating a merge request in Whisker"></td>
</tr>
</table>

1. **Create the ticket** with **+** on the Plane tile, or from a to-do or a failing check.
2. **Start the branch** (or a worktree) named after the ticket, in one click.
3. **Open the merge request.** Title and description come from the ticket and your commits, and Whisker offers to move the ticket to review.
4. **Merge** from the review inbox. Whisker suggests the ticket's next state.

<br>

## Pick your look

Five themes, or your own accent colour. Sakura is the pink one above; here are three more.

![Midnight theme](screenshots/theme-midnight.jpg)
<p align="center"><sub><b>Midnight</b></sub></p>

![Matcha theme](screenshots/theme-matcha.jpg)
<p align="center"><sub><b>Matcha</b></sub></p>

![Lavender theme](screenshots/theme-lavender.jpg)
<p align="center"><sub><b>Lavender</b></sub></p>

Plus **Tabby**, mixed, all-dark or all-light tiles, and a matching background or your own wallpaper.

<br>

## Get started

1. **[Download Whisker](https://github.com/ialhejaili/whisker/releases/latest/download/Whisker.dmg)**, open it, and drag Whisker into **Applications**.
2. **Open Whisker.** Settings opens on first launch: pick a theme and your city.
3. **Allow what you want.** macOS asks once each for Location, Calendar, Reminders and notifications.

Then turn on **Open at Login** in the menu-bar cat. The developer widgets stay out of the way until you connect them below.

<br>

## Connect GitLab, Plane and your local environment

Everything is in **Settings › Developer** (open Settings from the menu-bar cat). Whisker talks to your own servers with your own sign-in.

**First:** Apple's Command Line Tools (`xcode-select --install`) and [Homebrew](https://brew.sh).

### GitLab

Whisker uses the official GitLab CLI and its sign-in, so it never sees your GitLab token.

1. Install the CLI: `brew install glab`
2. Sign in:
   - **gitlab.com:** `glab auth login`, then choose **Web**.
   - **Your company's GitLab:** make a token in GitLab › avatar › **Edit profile** › **Access tokens**, with the **api** and **write_repository** scopes. Then run `glab auth login --hostname gitlab.example.com` and paste it.
3. Check it: `glab auth status`
4. In **Settings › Developer › GitLab**, fill in **Host** (like `gitlab.example.com`) and your **Username**.

The Review inbox fills in within two minutes.

### Plane

1. Make a token in Plane › avatar › **Profile settings** › **Personal access tokens** (older Plane: **Workspace settings** › **API tokens**). Copy it; Plane shows it once.
2. In **Settings › Developer › Plane**, fill in:
   - **Host**: `app.plane.so`, or your own Plane's address
   - **Workspace**: the slug in your Plane URLs (`my-team` in `app.plane.so/my-team/projects`)
   - **Project** (optional): one project's identifier, like `WORK`. Empty shows every project you're in.
   - **API token**: the token from step 1. It's stored only on this Mac.
3. Optional: **After opening an MR** and **After the MR merges** name the states Whisker offers, like `In Review` and `Ready for QA`.

The first load reads all your tickets; after that, only what changed, every two minutes.

### Your repo and local stack

1. In **Settings › Developer › Git**, press **Choose folder…** and pick your checkout. Make sure `git push` works there from Terminal; Whisker pushes with your own git setup.
2. In **Dev server**, add the start command (like `pnpm dev`) and its URL.
3. Turn on **Docker Compose** if your project uses it.
4. In **Checks**, add the commands you run often, like `pnpm test`.

### Notifications

Each kind can be turned off in **Settings › Developer**. If you said no when macOS asked, turn them on in **System Settings › Notifications › Whisker**.

<details>
<summary><b>If something doesn't show</b></summary>

<br>

- **A tile says it's offline:** the server didn't answer. Whisker keeps the last list and tries again.
- **"glab isn't signed in":** run the command the tile shows, then press refresh.
- **Plane says "Token rejected":** the token expired or was deleted. Make a new one.
- **Plane refused access (403):** check the workspace slug, and that you're a member.
- **Mentions are a little late:** Plane has no mentions feed for tokens, so Whisker reads the newest comments on tickets that changed. They show within a couple of minutes.

</details>

<br>

## Also on the desk

<table>
<tr>
<td width="22%" valign="top"><img src="screenshots/personal.png" alt="Cat photo, batteries and This Mac"></td>
<td width="22%" valign="top"><img src="screenshots/day.png" alt="Agenda and to-do list"></td>
<td valign="top">

- **Agenda** from Apple Calendar, with one-click **Join** for Zoom, Meet and Teams
- **To-do** you type naturally: `call the bank tomorrow !`
- **Prayer times** with adhan, iqama and a countdown, for your city
- **Batteries** for your mouse, keyboard and AirPods
- **This Mac**: CPU, memory, disk
- **Quick links** to the sites you open all day
- **A cat photo** every hour, checked to really be a cat

Also: Clock, Focus timer, Habits, Sticky note, Apple Reminders, and Cat fact & dev tip.

</td>
</tr>
</table>

Turn tiles on or off in **Settings › Widgets**, or drag them with **Arrange Tiles** in the menu-bar cat.

<br>

## Widgets for your Mac's desktop

Want just one or two? Every tile is also a macOS widget. Right-click the desktop, choose **Edit Widgets…** and search for Whisker.

![Whisker widgets in the macOS widget gallery](screenshots/mac-widgets.png)

- **The same buttons as the desk:** approve, merge, tick to-dos, start a branch, run checks
- **Typing opens just that panel**, floating over your windows
- **Click a widget's header** to bring up the whole desk

<br>

## Keyboard

| Keys | From any app |
|---|---|
| <kbd>⌥ Space</kbd> | Show or hide the desk |
| <kbd>⌥ ⇧ Space</kbd> | Today: everything that needs you |
| <kbd>⌃ ⌥ H</kbd> | Hide or show the widgets |

On the desk: <kbd>T</kbd> Today, <kbd>A</kbd> arrange tiles, <kbd>?</kbd> every shortcut, <kbd>Esc</kbd> back.

<br>

## Updates and privacy

- **Automatic updates.** Signed and checked before they install. Your settings stay.
- **Your data stays on your Mac** in `~/Library/Application Support/Whisker`.
- **Only the services you set up:** your GitLab and Plane, cataas.com for cat photos, and each quick link's site for its icon.
- **Nothing loads from the web** inside the widgets. Photos and icons are checked and re-encoded first.

<br>

---

<div align="center">
<sub>Made with care, and cats, by Ibtihal Alhejaili.<br>This repository hosts Whisker's releases.</sub>
</div>
