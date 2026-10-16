# GitHub to X Posts

![GitHub to X Posts social preview](assets/social-preview.png)

A Codex skill for turning useful GitHub discoveries into Chinese-language X posts that people outside developer circles can understand. It finds a promising project, verifies what someone can actually do with it, and hands over post copy, a demo video with checked reuse rights, and a separate GitHub link for the first reply.

This is a content research and writing workflow for creators who want more reach. It improves the odds of finding a compelling, credible story; it does not promise a viral post. **The instructions are in English, but the default post output is in Chinese.**

## Quick start

**1. Open Codex.** Give it web access for live research. You do not need to connect your X account to get the copy. To have Codex type the main post into X, make your external Chrome or Edge session available. This workflow does not use Codex's in-app browser.

**2. Install the skill.** Paste this into a new Codex chat:

```text
Use $skill-installer to install the skill at the root of https://github.com/Balance0014/github-to-x-posts. Select path "." and name it "github-to-x-posts".
```

Prefer the terminal? Clone the public repository into the [documented user skills directory](https://learn.chatgpt.com/docs/build-skills):

```bash
mkdir -p ~/.agents/skills
git clone https://github.com/Balance0014/github-to-x-posts.git ~/.agents/skills/github-to-x-posts
```

Start a new chat after installation. If Codex does not recognize the skill, restart Codex and try again. Closing a chat does not remove a locally installed skill. On another computer or with a fresh Codex setup, install it again from this public repository. The published instructions do not depend on the original chat or account; access to an X browser session must be set up again separately.

**3. Run your first search.** Copy this prompt and adjust the category if needed:

```text
Use $github-to-x-posts to find one GitHub tool worth posting about on Chinese X today. Prioritize video creation or editing for everyday users. Verify the central benefit and material limits, then write a strong user-first Chinese post. If my external X browser is available, type only the main-post text there. Give me a direct demo-video download link or save the unmodified video to my Desktop; I will upload it and click Post. Give me the GitHub URL separately so I can paste it into the first reply.
```

You should receive one recommended project and the reason it was chosen, a clear distinction between firsthand testing and source claims, the finished post, a usable video location, the exact first-reply GitHub link, and any important caveats. If no candidate passes the checks, the skill should say so instead of inventing one.

## How the workflow works

1. Start with a result an everyday user wants, especially in video creation, editing, design, or other visual tasks.
2. Check the project, the live product, and the path from input to finished output. Test it when practical.
3. Search X for competing posts and look for a distinct, useful angle.
4. Write around the reader's situation and outcome: a strong opening, one clear benefit, and only the proof the claim needs.
5. Prefer a reusable, ready-to-upload author demo. Hand over its direct download URL or a verified file on the user's Desktop; avoid video conversion and uploads unless requested.
6. Deliver the exact main-post copy and separate GitHub reply link. When an external X browser is available, type only the main-post text. The account owner uploads the video, publishes, and adds the reply.

The operating instructions are in [SKILL.md](SKILL.md). Use the [candidate and draft worksheet](references/run-sheet.md) to keep evidence close to the claims it supports.

## Evidence and media

Separate firsthand observations from an author's demo and from inference. Check reuse rights before using someone else's media; attribution alone is not permission. Recheck time-sensitive details such as pricing, GitHub stars, and X rules each time you use the skill.

This repository is the portable source of truth for the skill. It contains a general workflow and a blank worksheet, without private account analytics, personal experiments, unpublished post assets, or credentials.

## License

MIT. See [LICENSE](LICENSE).
