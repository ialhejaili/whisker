<div align="center">

<img src="screenshots/icon.png" width="128" height="128" alt="Whisker app icon">

# Whisker

### Your day and your dev work, right on your Mac's desktop.

Interactive widgets with a calm, cat-themed design. Join a meeting, tick off a to-do,<br>
approve a merge request or open a ticket without leaving the desk.

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

## At a glance

<table>
<tr>
<td width="33%" valign="top">

**For your day**

- Agenda from Apple Calendar, with one-click Join
- To-dos you can type naturally
- Prayer times with iqama, for your city
- Batteries, your Mac, quick links
- A new cat photo every hour

</td>
<td width="33%" valign="top">

**For your dev work**

- GitLab review inbox: approve, merge, reply
- Plane tickets: create, move, comment
- Create merge requests in one step
- Notified when your MRs or tickets change
- Your repo, branches and worktrees
- Dev server, containers and checks

</td>
<td width="33%" valign="top">

**Made for the Mac**

- Lives on the desktop, behind your windows
- Or add single widgets next to your own
- <kbd>⌥ Space</kbd> brings it to the front
- A menu-bar cat lists what needs you
- Five themes, or your own colour
- Updates itself, data stays on your Mac

</td>
</tr>
</table>

<br>

## From ticket to merge request

Whisker links your Plane tickets, your repo and GitLab, so every ticket you're working on shows its next step.

<table>
<tr>
<td width="50%" valign="top"><img src="screenshots/new-ticket.png" alt="Creating a Plane ticket in Whisker"></td>
<td width="50%" valign="top"><img src="screenshots/new-mr.png" alt="Creating a merge request in Whisker"></td>
</tr>
<tr>
<td valign="top"><b>1. Create the ticket.</b> Press <b>+</b> on the Plane tile: title, description, state, priority, labels and due date, assigned to you. You can also turn a to-do or a failing check into a ticket, already filled in.</td>
<td valign="top"><b>3. Open the merge request.</b> The title and description come from the ticket and your commits. Whisker pushes the branch if needed, opens the MR, and offers to move the ticket to review.</td>
</tr>
</table>

**2. Start the branch.** One click creates a branch (or a worktree) named after the ticket.<br>
**4. Merge.** Approve and merge from the review inbox. Once it's merged, Whisker suggests the ticket's next state.

You choose which states those are in **Settings › Developer**, to match your team's workflow.

<br>

## Widgets for your Mac's desktop

Want just one or two? Every Whisker tile is in the macOS widget gallery too, so you can place it next to your own. Right-click the desktop, choose **Edit Widgets…** and search for Whisker.

![Whisker widgets in the macOS widget gallery](screenshots/mac-widgets.png)

All 19 of them, in the sizes macOS offers: Up next, Agenda, Prayer times, Clock, Cat fact, To-do, Reminders, Habits, Focus timer, Sticky note, Needs you, Plane tickets, Review inbox, Repo, Dev stack, Cat of the hour, Batteries, This Mac and Quick links.

- **They have the desk's buttons.** Tick to-dos and reminders, approve and merge MRs, retry pipelines, start a branch or an MR, fetch and pull, start your dev server, run checks, count habits, run the focus timer. A short note under the widget says how it went.
- **Anything that needs typing opens just that panel.** A comment, a reply, a new ticket or to-do floats over your windows with everything the desk has, and goes away when you're done.
- **Click a widget's header to see everything.** The whole desk comes up, where the tile shows all of its items.
- **They fit in.** Your theme, every size, and macOS's tinted desktop style.

Whisker needs to be running to keep them up to date.

<br>

## Keyboard

| Keys | From any app |
|---|---|
| <kbd>⌥ Space</kbd> | Show or hide the desk |
| <kbd>⌥ ⇧ Space</kbd> | Today: everything that needs you |
| <kbd>⌃ ⌥ H</kbd> | Hide or show the widgets |

On the desk: <kbd>T</kbd> Today, <kbd>A</kbd> arrange tiles, <kbd>?</kbd> every shortcut, <kbd>Esc</kbd> back. Pick another desk shortcut in **Settings › Look**.

<br>

## Widgets on the desk

Turn widgets on or off and reorder them in **Settings › Widgets**, or drag them into place with **Arrange Tiles** in the menu-bar cat.

### For developers

![Review inbox and Plane tickets](screenshots/dev.png)

| | |
|---|---|
| **Review inbox** (GitLab) | The merge requests that need you, most urgent first: failing pipelines and conflicts on yours, replies you owe, reviews you've been asked for. Approve, merge now or when the pipeline passes, retry a pipeline, read the job log and reply to threads. You get a notification when one of your MRs fails or passes its pipeline, is approved, becomes ready to merge, gets conflicts, a new comment or an unresolved thread, or is merged or closed by someone else. Click it to open the MR. |
| **Plane tickets** | Your work items by Doing, Waiting, Todo and Done, with due dates, cycles and priority. Create tickets, change state or priority, comment, and see each ticket's branch and merge request. You get a notification when someone else moves one of your tickets, and when anyone mentions you on any ticket, in a comment or the description. |

<table>
<tr>
<td width="40%" valign="top"><img src="screenshots/repo-stack.png" alt="Repo and dev stack widgets"></td>
<td valign="top">

**Repo.** Branch, ahead and behind, changed files, stashes and recent commits, plus the branch's ticket and merge request. Fetch, pull, switch or create branches, stash, create merge requests and clean up old worktrees. A strip of paw prints counts your commits per day.

**Dev stack & checks.** Start, stop and restart your dev server and read its log. It only shows as running when the app really answers. Bring Docker Compose up or down, watch each container, and run your checks with a pass/fail history. You get a notification when something breaks.

</td>
</tr>
</table>

### For your day

<table>
<tr>
<td width="22%" valign="top"><img src="screenshots/personal.png" alt="Cat photo, batteries and This Mac"></td>
<td width="22%" valign="top"><img src="screenshots/day.png" alt="Agenda and to-do list"></td>
<td valign="top">

**Agenda.** Today and tomorrow from Apple Calendar, including the Google and Exchange calendars you've added there. The next meeting gets a big card with **Join** for Zoom, Meet and Teams. Open any day, add events, and tick off dated reminders.

**To-do.** Type naturally: `call the bank tomorrow !` sets the due date and priority (`!` high, `!!` urgent). Turn any to-do into a Plane ticket.

**Batteries.** Mouse, keyboard, AirPods and their case, with charging state.

**This Mac.** CPU, memory, disk, and the apps using the most memory.

**Cat photo.** A new cat every hour. Every photo is checked on your Mac to make sure it really is a cat, and not a meme or a dog. Keep favourites, or hide one for good.

**Quick links.** The sites you open all day, with their real icons.

</td>
</tr>
</table>

![Prayer times](screenshots/prayer.png)

**Prayer times.** The next prayer with a countdown, all five prayers with adhan and iqama times, and sunrise. Calculated on your Mac for your city with the method you choose (Umm al-Qura, Muslim World League, ISNA, Egypt, Karachi, Dubai, Kuwait, Qatar, Singapore or Turkey). Set iqama offsets and get an alert before each prayer.

Also available: **Clock & greeting**, **Focus timer**, **Habits**, **Sticky note**, **Apple Reminders** and **Cat fact & dev tip**.

<br>

## Make it yours

<table>
<tr>
<td width="33%"><img src="screenshots/theme-midnight.jpg" alt="Midnight theme"></td>
<td width="33%"><img src="screenshots/theme-matcha.jpg" alt="Matcha theme"></td>
<td width="33%"><img src="screenshots/theme-lavender.jpg" alt="Lavender theme"></td>
</tr>
<tr>
<td align="center"><sub><b>Midnight</b></sub></td>
<td align="center"><sub><b>Matcha</b></sub></td>
<td align="center"><sub><b>Lavender</b></sub></td>
</tr>
</table>

<img align="right" width="45%" src="screenshots/settings.png" alt="Whisker Settings">

- Five themes (Sakura, Tabby, Lavender, Matcha, Midnight) or your own accent colour
- Mixed, all-dark or all-light tiles
- A matching background with wandering paw prints, or your own wallpaper
- How many rows of tiles, and which display
- A shortcut or hot corner to bring the desk forward
- Cover your desktop files with the background, or keep them in view
- Export your settings to another Mac

<br clear="right">

<br>

## Get started

1. **[Download Whisker](https://github.com/ialhejaili/whisker/releases/latest/download/Whisker.dmg)**, open it, and drag Whisker into **Applications**.
2. **Open Whisker.** Settings opens on first launch: pick a theme and your city.
3. **Allow what you want.** macOS asks once each for Location, Calendar, Reminders and notifications.

Then turn on **Open at Login** in the menu-bar cat, and your desk is ready every morning.

The developer widgets stay out of the way until you connect them. See [Connect GitLab and Plane](#connect-gitlab-and-plane).

<br>

## Connect GitLab and Plane

Everything below is in **Settings › Developer**. Open Settings from the menu-bar cat. Whisker talks to your own servers with your own sign-in; nothing goes through anyone else.

### What you need first

- **Command Line Tools.** Whisker's data scripts use Apple's `python3` and `git`. If you've never installed them, run `xcode-select --install` in Terminal (macOS also offers this the first time it's needed).
- **Homebrew**, to install the GitLab CLI. See [brew.sh](https://brew.sh).

### GitLab (Review inbox, merge requests)

Whisker uses the official GitLab CLI, `glab`, and its sign-in. Whisker never sees or stores your GitLab token.

1. **Install the CLI.** In Terminal:

   ```sh
   brew install glab
   ```

2. **Sign in.**
   - On gitlab.com: run `glab auth login`, choose **gitlab.com**, then **Web** to sign in with your browser.
   - On your company's GitLab: first make a token. In GitLab, open your avatar › **Edit profile** › **Access tokens** (called **Personal access tokens** in newer GitLab) › **Add new token**, give it the **api** and **write_repository** scopes and an expiry date, and copy it. Then run the command below with your GitLab's address and paste the token when asked:

     ```sh
     glab auth login --hostname gitlab.example.com
     ```

3. **Check it.** `glab auth status` should say you're logged in to that host.
4. **Fill in Whisker.** In **Settings › Developer › GitLab**:
   - **Host**: your GitLab's address without `https://`, for example `gitlab.com` or `gitlab.example.com`.
   - **Username**: your GitLab username (the one after `@`). Whisker uses it to tell your MRs and comments from other people's.
5. **Choose your notifications.** Pipeline results, Approvals, Comments, Unresolved threads, and Merged, closed, conflicts are all on to start with. Turn off any you don't want.

Within two minutes the Review inbox fills in. If it says glab isn't signed in, run the command it shows, then press its refresh button.

### Plane (Plane tickets)

Whisker reads your tickets with a personal access token. It's stored only on this Mac, in Whisker's settings file, and left out when you export your settings unless you choose to include it.

1. **Make a token.** In Plane, open your avatar › **Profile settings** › **Personal access tokens** › **Add personal access token** (on older Plane: **Workspace settings** › **API tokens**). Give it a name like "Whisker", pick an expiry, and copy the token (it starts with `plane_api_`). Plane shows it only once.
2. **Find your workspace slug.** It's the first part of your Plane URLs: in `https://app.plane.so/my-team/projects/`, the slug is `my-team`.
3. **Fill in Whisker.** In **Settings › Developer › Plane**:
   - **Host**: `app.plane.so` for Plane Cloud, or your own Plane's address, for example `plane.example.com`.
   - **Workspace**: the slug from step 2.
   - **Project**: optional. A project's identifier (the letters in its ticket ids, like `WORK` in `WORK-42`) shows only that project. Leave it empty to see your tickets in every project you're a member of (up to 10).
   - **API token**: paste the token from step 1.
4. **Match your workflow.** **After opening an MR** and **After the MR merges** name the states Whisker offers to move a ticket to, such as `In Review` and `Ready for QA`. Leave them empty and Whisker picks a review state and your first done state.
5. **Choose your notifications.** **Ticket moved** and **Mentions** are on to start with.

The first load reads all your tickets and can take a little while; after that, Whisker only asks Plane for what changed, every two minutes.

### Branches and merge requests from tickets

To start branches and open merge requests from a ticket, Whisker also needs your checkout:

1. In **Settings › Developer › Git**, press **Choose folder…** and pick your repository.
2. Make sure `git push` works in that folder from Terminal (SSH key or saved credentials). Whisker pushes with your own git setup.

### Notifications

macOS asks once whether Whisker may send notifications. If you said no, turn them on in **System Settings › Notifications › Whisker**.

### If something doesn't show

- **A tile says it's offline:** the server didn't answer. Whisker keeps showing the last list and tries again on its own.
- **Plane says "Token rejected":** the token expired or was deleted. Make a new one and paste it in.
- **Plane says it refused access (403):** check the workspace slug, and that you're a member of that workspace.
- **Mentions are a little late:** Plane has no mentions feed for tokens, so Whisker finds them by reading the newest comments on tickets that changed. They show within a couple of minutes.

<br>

## Updates and privacy

- **Automatic updates.** Whisker checks once a day. When a new version is out, you get a notification and an **Install** item in the menu-bar cat. Your settings and permissions stay. Every update is signed and checked before it installs.
- **Your data stays on your Mac.** Settings, to-dos and favourites live in `~/Library/Application Support/Whisker`. Nothing is sent anywhere.
- **Only the services you set up.** Whisker talks to your own GitLab and Plane, to cataas.com for cat photos, and to each quick link's site for its icon.
- **Nothing loads from the web.** Widgets can't load anything from the internet. Photos and icons are downloaded, checked and re-encoded by Whisker, then shown as local images.

<br>

---

<div align="center">
<sub>Made with care, and cats, by Ibtihal Alhejaili.<br>This repository hosts Whisker's releases.</sub>
</div>
