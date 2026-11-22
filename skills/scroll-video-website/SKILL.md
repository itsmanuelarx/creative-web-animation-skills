---
name: scroll-video-website
description: Build or refine a website where native scrolling scrubs an approved video and coordinates object transitions into page content. Use for scroll-driven cinematic entrances and photographic object motion, rather than ordinary autoplay video embeds.
---

# Scroll video website

Turn an approved visual sequence into a responsive, reversible website interaction. Reuse the existing site's stack and approved assets; the technique does not require a particular animation library.

## Establish the interaction

Inspect the current implementation, approved version and latest user feedback before editing. Resolve from that context:

- Which motion is in the video, and which objects are separately animated in code?
- Does scrolling control the complete clip, or does a deliberate timed segment precede scrolling? Follow the selected behaviour. A scroll-from-the-start request must work on the first wheel or touch scroll without a click gate.
- Where does the final scene become ordinary page content? How can visitors reach projects directly?
- Which sizes and platforms matter, and which preview must remain available?

If only timing or control changes are requested, do not regenerate media. Save the current working version and create an isolated alternative when comparison is requested.

## Prepare the media

Use the exact video and corresponding decoded start/end stills. Preserve colour interpretation, aspect ratio and the source file. If the seam itself is wrong, fix the media handover before hiding it with interaction effects.

Inspect duration, frame rate, dimensions and seeking behaviour. Shorter keyframe intervals can help scrubbing; an all-keyframe copy can be useful for a local prototype but may become too large for deployment. Benchmark the derivative in the actual browser and optimise delivery separately. Do not prescribe one encoding setting for every clip.

Keep a poster while metadata and frames load. Retain the latest requested time and apply it when the video becomes ready. A missing or rejected video must leave a usable static route to content.

## Map scrolling to a timeline

1. Use a native scrolling track and a sticky visual stage when they fit the existing layout. Keep the document scrollable immediately if scrolling is the entrance control. Avoid wheel interception and touch capture merely to simulate a scrollbar.
2. Divide the story into intentional ranges: object descent, camera reveal, room hold, object transfer and content. Allocate enough distance to brief but important events. Map each range to its media or transform progress; the clip's seconds need not map uniformly to scroll pixels.
3. Update from one requestAnimationFrame scheduled by scroll events. Read layout when measuring, not repeatedly inside every animation update.
4. Keep the video paused for scrubbing. Coalesce seeks: store the latest target, do not start a competing seek while one is pending, and apply the latest target after `seeked`. Do not build a backlog of obsolete frames.
5. Clamp endpoints, with a small pixel tolerance for fractional viewport calculations. Test the first and final frames using actual browser scroll positions.
6. Make stopped scrolling hold the current state. Reverse each phase according to the chosen interaction, including the opening action when the entire clip is scroll-controlled.
7. Cancel programmatic travel when the visitor supplies wheel, touch or navigation-key input. Prevent resize and restored scroll positions from unexpectedly skipping the opening state.

For a hybrid entrance, explicitly define which segment is timed and where reverse scrolling stops. Do not silently introduce a timed segment into a fully scroll-controlled experience.

## Keep photographic objects continuous

Use one visible object through extraction, flight and landing, where practical. If reparenting it onto a destination, match its position and projection before and after that change.

A full end-over-end flip needs a 3D rotation that exposes the edge. A flat in-plane rotation is a different motion. A textured plane can give the required effect; do not describe it as a fully modelled 3D scene.

Keep source and destination measurements in a consistent coordinate system. Do not mix viewport and document coordinates when a stage is sticky. Re-measure on resize and preserve meaningful progress. For a turntable, keep the needle raised until the record lands, then lower it before the playing state begins.

Blend scene boundaries using matched lighting and scene geometry. Keep headings and project links readable instead of placing them over visually busy equipment. On a narrow viewport, let the project list sit beneath the object when there is insufficient space beside it.

## Preserve website access

Reveal navigation at the chosen point in the story, not only after a long film finishes. Keep direct category access, skip, replay and a route back to the scene. If category changes are meant to exchange the object, coordinate that with the needle and project list; rapid selections should settle on the latest request.

Do not focus a target while it or an ancestor is inert. Make it interactive first, then focus it without an extra scroll jump. Restore focus after project dialogs close.

A reduced-motion path should show usable static scenes without scrubbing or flipping, including when scrolling backwards. Keep failed-media state persistent so reverse scrolling cannot restore a broken overlay.

## Verify and hand over

Use the supported browser tools to test real input, not only calls to internal animation functions:

- From a fresh load, scroll without clicking. Stop partway, continue, then reverse to the opening.
- Inspect the video/still handover and the object-to-destination join visually.
- Reach the projects with one object in the correct place. Exercise category change, skip, replay and keyboard focus.
- Check desktop and phone layouts, resize mid-journey, reduced motion and a deliberately unavailable video.
- Check horizontal overflow, media loading and console errors. Distinguish browser emulation from a physical phone test.

Deliver the review URL, a useful screenshot, the preserved baseline, and any material performance or device-testing limits. Keep a concise manifest identifying the source media and timing. Implementing a local review does not by itself authorise publication.
