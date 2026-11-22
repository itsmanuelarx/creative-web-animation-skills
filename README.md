# Creative web animation skills

Two reusable AI-agent workflows extracted from building an interactive portfolio with a cocktail entrance, a camera turn, and a photographic vinyl record that moves into a project menu.

| Skill / readable SOP | Use it for |
| --- | --- |
| [Seamless video entrance](skills/seamless-video-entrance/SKILL.md) | Creating and refining a short video that joins cleanly to a website's opening and final scene. |
| [Scroll video website](skills/scroll-video-website/SKILL.md) | Making scrolling control a video from its first frame and coordinating object motion, responsive layouts and project navigation. |

## What these are

These are instructions an AI coding assistant can follow, and SOPs a person can read. They are not video models, pre-rendered animations or a complete website template.

They were written **after** the original build to capture the process. General frontend-design and development workflow skills supported that build; the entrance, frame handover and scroll behaviour were custom work. The generated film supplies the photographed motion; website code controls its playback or scroll position. A photographic texture and CSS transforms supply the record's apparent 3D flip.

## Can this turn an image into a video?

Yes, as a guided workflow with a video generator. **The skill itself is not the video model.**

- **Starting with an image:** bring your image and access to an image-to-video model or app. Higgsfield is one option, not a requirement. Your chosen tool needs to support the motion and references you want; availability and pricing vary.
- **With a connected, authorised generator:** the assistant can use the available tools to prepare references, submit a generation and review the result. Automatic operation depends on what your assistant can actually access.
- **Without a connected generator:** the assistant prepares the prompt, reference roles and review checklist. You generate the clip in your chosen app, then provide the downloaded video so the assistant can continue.
- **With an existing clip:** start with that video. You do not need another generation unless it needs changes that require one.

The website's scroll control is a separate coding step. It does not require Higgsfield. You need a coding assistant with access to your website files and suitable media and browser tools. Subscriptions, API access and generation credits are your own. These instructions do not guarantee a finished animation in one attempt.

## Use a skill

Download a skill folder and add it to your assistant's supported skills directory. For a Codex setup using the standard user directory, the two folders go under `~/.codex/skills/`. Keep each `SKILL.md` and its `agents/` folder together. Reload skill discovery or start a new session if the assistant does not see it yet. Other assistants have their own installation locations; these Markdown instructions can also be supplied directly.

Example requests:

- `Use $seamless-video-entrance to turn this image into a short entrance. First check which video tools you can access. If none are connected, prepare the prompt and references for me to generate the clip in my own app.`
- `Use $seamless-video-entrance to make the approved clip join seamlessly to this website. Preserve its glass, lighting and camera movement.`
- `Use $scroll-video-website so scrolling lowers the object from the first frame, then reveals the room and continues into the project menu.`

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

The repository contains the workflows only. Source photographs, generated clips, reference images, private project notes and paid-service job data are not included. No third-party skill implementation has been copied into the package.

MIT licence applies to the original text in this repository. It does not license any third-party tools, models or media.
