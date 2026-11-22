# Creative web animation skills

Reusable skills for creating cinematic website entrances and scroll-controlled visual stories from your own images or video. Use them with Claude or Codex to plan motion, preserve visual continuity and connect the sequence to a responsive website.

| Skill / readable SOP | Use it for |
| --- | --- |
| [Seamless video entrance](skills/seamless-video-entrance/SKILL.md) | Creating and refining a short video that joins cleanly to a website's opening and final scene. |
| [Scroll video website](skills/scroll-video-website/SKILL.md) | Making scrolling control a video from its first frame and coordinating object motion, responsive layouts and page content. |

## What you can adapt them to

Choose the subject, motion and destination for your own project:

| Example | Motion idea | Relevant workflow |
| --- | --- | --- |
| Product launch | Rotate a shoe, bag or perfume bottle, then settle into the product page | Video entrance, optionally controlled by scroll |
| Interior or venue | Move through a doorway or pull back to reveal a room | Video entrance and scene handover |
| Artist portfolio | Bring an artwork forward, flip it, then place it beside its project details | Object transitions and scroll control |
| Brand story | Scrub through a short visual sequence as the visitor scrolls, with text appearing at selected moments | Scroll video website |

These are adaptation ideas, not supplied demos. The original tested example was a cocktail-and-vinyl portfolio. Its subjects, red lighting and falling motion are optional creative choices.

The scope is short video entrances, scroll-controlled video and coordinated object transitions on websites. Choose generation or coded motion to suit the shot. Character rigging, complete 3D scene modelling and long-form film editing require additional tools and workflows.

## What these are

These are instructions an AI coding assistant can follow, and SOPs a person can read. They are not video models, pre-rendered animations or a complete website template.

They were written **after** the original build to capture the process. General frontend-design and development workflow skills supported that build; the entrance, frame handover and scroll behaviour were custom work. In the original cocktail-and-vinyl example, a generated film supplies the camera movement, website code controls playback or scroll position, and a photographic texture with CSS transforms supplies the record's apparent 3D flip. Other subjects use the same separation between media, interaction and object motion.

## Can this turn an image into a video?

Yes, as a guided workflow with a video generator. **The skill itself is not the video model.**

- **Starting with an image:** bring your image and access to an image-to-video model or app. Higgsfield is one option, not a requirement. Your chosen tool needs to support the motion and references you want; availability and pricing vary.
- **With a connected, authorised generator:** the assistant can use the available tools to prepare references, submit a generation and review the result. Automatic operation depends on what your assistant can actually access.
- **Without a connected generator:** the assistant prepares the prompt, reference roles and review checklist. You generate the clip in your chosen app, then provide the downloaded video so the assistant can continue.
- **With an existing clip:** start with that video. You do not need another generation unless it needs changes that require one.

The website's scroll control is a separate coding step. It does not require Higgsfield. You need a coding assistant with access to your website files and suitable media and browser tools. Subscriptions, API access and generation credits are your own. These instructions do not guarantee a finished animation in one attempt.

## Use a skill

These workflows can be used with **Claude or Codex**. The core instructions are in `SKILL.md`; the `agents/openai.yaml` files provide Codex UI metadata. Tool access determines which steps an assistant can carry out automatically.

### Claude Code

Copy each folder from this repository's `skills/` directory into `~/.claude/skills/` for personal use, or `.claude/skills/` inside your website project. For example, the final path should be `~/.claude/skills/seamless-video-entrance/SKILL.md`.

Invoke it with `/seamless-video-entrance` or `/scroll-video-website`, followed by your request. See [Claude Code's official skills documentation](https://code.claude.com/docs/en/skills).

### Claude app

Download the repository, then ZIP **one skill folder at a time** from inside `skills/`. Each ZIP should contain that named folder with its `SKILL.md` directly inside it. The whole repository ZIP is not a single installable Claude skill.

Enable code execution and file creation, then go to **Customize > Skills > + > Create skill > Upload a skill** and upload each ZIP. Enable the skill and ask Claude to use it. Availability can depend on your organisation's settings. See [Claude's official upload guide](https://support.claude.com/en/articles/12512180-use-skills-in-claude).

Claude still needs access to the website files and the necessary generation, media and browser tools. If a tool is unavailable, use the manual handoff described above. A chat upload does not automatically grant access to your computer or video service.

### Codex

Copy each skill folder into `~/.codex/skills/`. Keep `SKILL.md` and its `agents/` folder together. Reload skill discovery or start a new session if the assistant does not see it yet.

Codex example requests:

- `Use $seamless-video-entrance to turn this image into a short entrance. First check which video tools you can access. If none are connected, prepare the prompt and references for me to generate the clip in my own app.`
- `Use $seamless-video-entrance to make this approved product-turn video settle into the product page. Preserve the product shape, materials and lighting.`
- `Use $scroll-video-website so scrolling controls this interior walkthrough from the first frame, then reveals the booking content.`
- `Use $scroll-video-website to bring this artwork forward, flip it and settle it beside the project details. Keep the transition reversible and usable on phones.`

Supply your own project and approved media. Video generation, encoding and browser inspection require the appropriate tools in your environment. These files do not include a model subscription, credentials, paid credits or those tools.

## Workflow

1. Decide the start and finish of the scene and what the visitor controls.
2. Produce or select the video and get the imagery right.
3. Use exact decoded video frames for the website's still states.
4. Wire native scroll to the film timeline and coordinate any separate object animation.
5. Check the joins, backwards scrolling, phone layout, access to content and media fallback.

The exact timeline distances, crop, colours, objects and model are project inputs. The skills do not require a bar, a margarita, a particular model or an animation framework.

## Status and scope

The techniques were exercised on the original portfolio in desktop and phone browser layouts. These packaged instructions have passed structural validation and a scenario walkthrough; they have not yet been tested by rebuilding a separate site from scratch. Physical iPhone Safari and constrained-network performance still need project-specific testing.

Claude installation instructions have been checked against its official documentation. A fresh end-to-end run of these packaged skills in Claude has not yet been tested.

The repository contains the workflows only. Source photographs, generated clips, reference images, private project notes and paid-service job data are not included. No third-party skill implementation has been copied into the package.

MIT licence applies to the original text in this repository. It does not license any third-party tools, models or media.
