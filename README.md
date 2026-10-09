# Disable GitHub Copilot

A Chrome extension that hides the Copilot entry points on github.com.

## What the extension hides

- Header: the chat link, the "Open Copilot…" menu and the agents panel
- Menus: the Copilot entries in the side navigation, in quick search, in the
  "Create new…" menu and in the user menu
- Dashboard: the chat input above the feed
- Repository: the "Agents" tab and the "Ask Copilot about this repository"
  button
- File view: the "Ask Copilot about this file" button
- Issue: "Open in GitHub Copilot app" and Copilot as a suggested assignee
- Pull request: Copilot as a suggested reviewer, the banners, the
  "Mention @copilot" hint and the "Mention Copilot" button of the comment field
- Diff: the "Ask about this diff" button
- New repository: the "Jumpstart your project with Copilot" section
- Settings: the "Copilot" section in the navigation

## What stays visible

Content produced by Copilot stays visible. This includes review comments,
pull requests and a review that has already been requested.

## What the extension does not do

The extension hides, it does not disable. Features that GitHub runs on the
server keep running. Their settings remain reachable by URL:
<https://github.com/settings/copilot/features>

## Install

1. Clone this repository.
2. Open `chrome://extensions` in Chrome.
3. Turn on "Developer mode" in the top right corner.
4. Click "Load unpacked".
5. Select the directory of the repository.

## Update

1. Fetch the latest state with `git pull`.
2. Open `chrome://extensions`.
3. Click the reload icon of the extension.

## Turn off

Turn the extension off in `chrome://extensions`. GitHub shows the entry points
again after you reload the page.

## An entry point is still visible

GitHub changes its markup continuously. If an entry point stays visible, its
selector is missing in `hide-copilot.css`.
