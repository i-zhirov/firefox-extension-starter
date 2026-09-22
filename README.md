# Firefox Extension Starter

A minimal starter for building a small personal Firefox extension with an
AI coding agent.

It intentionally has no framework, build step, package manager, or tests. Start
with one browser annoyance and ask the agent for the smallest visible result.

## Workshop slides

[How to vibe-code your own browser extension](https://docs.google.com/presentation/d/1dmGO9mRsZkxoAsaXVFD39EdQ4gLamleBLnX2DALNcug/edit?usp=sharing)
— the participant version without speaker notes.

## Start in five minutes

1. Get the repository:
   - with Git: `git clone https://github.com/i-zhirov/firefox-extension-starter.git`
   - without Git: click **Code → Download ZIP**, then unzip it
2. Open the repository folder in your AI coding editor or agent.
3. Describe one thing you want to change in the browser.

For example:

> On example.com, replace every letter “A” with a fish emoji. Make the smallest
> working version, then tell me exactly how to load and test it in Firefox.

The agent should read [`AGENTS.md`](AGENTS.md) and [`manifest.json`](manifest.json),
then add only the files the extension actually needs.

## Load it in Firefox

1. Open `about:debugging` in Firefox.
2. Click **This Firefox**.
3. Click **Load Temporary Add-on…** and select the `manifest.json` file in
   this repository folder (Firefox reads the whole folder).
4. Open the test page and check that the requested change is visible.

A temporary add-on is removed when Firefox restarts. If you restart Firefox,
load it again with the same steps.

After every code change:

1. Click **Reload** on the add-on card in `about:debugging`.
2. Reload the test page.
3. Try the same action again.

## Pick a small first idea

A good workshop idea:

- can be seen on one test page;
- fits in one sentence;
- works without a backend, login, payment, or store publication;
- can be checked manually in a couple of minutes.

Simple examples:

- replace a letter or word with an emoji;
- hide a distracting block on a website;
- highlight items that match a rule;
- add a button that copies useful text or links;
- change the appearance of one site.

## What is included

- `manifest.json` — the minimal Manifest V3 description of the extension,
  including `browser_specific_settings.gecko.id`, the stable identity that
  Firefox uses for the add-on;
- `AGENTS.md` — beginner-friendly instructions for the AI agent;
- `README.md` — the setup and loading steps you are reading now.

Firefox is the default target. If you want Chrome, Safari, or another browser,
say so explicitly in your request to the agent.

Useful official guides:

- [MDN: Your first extension](https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/Your_first_WebExtension)
- [Extension Workshop: Temporary installation in Firefox](https://extensionworkshop.com/documentation/develop/temporary-installation-in-firefox/)
- [MDN: Anatomy of an extension](https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/Anatomy_of_a_WebExtension)
