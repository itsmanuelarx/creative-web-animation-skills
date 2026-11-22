---
name: seamless-video-entrance
description: Create or refine a short photographic video entrance that joins cleanly to a website's opening and final scene. Use when subject identity, materials or reflections, colour continuity, camera movement or temporal repairs need to remain believable across video and still states.
---

# Seamless video entrance

Build a continuous visual entrance that settles naturally into the website. Treat the image, video, browser decoding and page composition as one visual sequence. Adapt the subject and action to the project: products, interiors, artwork or other scenes. Drink, splash and counter examples below are conditional examples, not required elements. Choose a motion the available video or animation tools can support; this workflow does not supply character rigs or a 3D scene engine.

## Recover the approved direction

Locate the actual approved image, clip, crop and feedback. Distinguish approval of a visual from approval to publish it. Preserve originals and working snapshots; do not let a new experiment silently become the baseline.

Identify the intended camera position, subject scale, lighting, materials, motion and final framing. Separate fixed details from experimental ones. The newest explicit user correction overrides an older prompt or manifest.

Inspect the source video directly before editing. If no approved source exists, locate supplied references and prepare a reviewable first candidate. Ask only for inputs that cannot be recovered from the project or connected sources.

## Start from an image or an existing clip

This skill supplies a workflow, not a video model, subscription or generation runtime. Starting from a still image requires access to an image-to-video service or model. Higgsfield is optional; use the user's chosen tool if it supports the required inputs and action. Starting from a suitable existing clip can skip generation.

1. Inspect the supplied image and identify the intended movement, camera path and settled endpoint. Recover these choices from project context before asking for missing inputs.
2. Check which generation tools the assistant can actually access, their supported references and the user's authorisation for any paid request. Do not promise automatic generation without a usable tool.
3. With a connected generator, submit the concrete request through the available tool. Without one, give the user a ready-to-use prompt, the exact reference roles and suggested settings supported by their selected app. Ask them to generate and supply the resulting video; keep that dependency explicit.
4. Preserve the returned clip, record its provenance and inspect it before wiring it into the website. Judge the result against the approved image and motion, not merely the generation tool's success response.

Do not claim that writing a prompt or creating this skill generated a video. Continue with media preparation and website integration only when the actual output is available.

## Choose the smallest useful intervention

- Use a new generation when the scene or camera movement is fundamentally wrong.
- Use a targeted edit when a specific defect needs changing but the shot is otherwise approved.
- Use deterministic finishing when colour, timing, decoding or a local temporal defect can be corrected while preserving the shot.

Use the user's selected model and currently available tools. Record the model as displayed by the service, the request, settings, output and review result. Do not infer a model's identity from a filename or treat a tool/model as an agent skill. Check current availability and cost before a new paid request; project-specific approvals do not become a standing retry budget.

## Design a continuous shot

Assign each image reference a purpose: composition, subject identity, materials, lighting or endpoint. Avoid mixing several references with incompatible geometry and asking the model to infer the priority.

When start/end references are supported, anchor both endpoints. Describe the physical action and camera path separately. Define cause and effect for the chosen action. A product turn should preserve its shape and surface details; a camera moving through a doorway should preserve room geometry. For a liquid-impact shot, the object touches the liquid before a splash appears; a visible droplet should persist or become plausibly occluded.

Keep the subject, supporting surface, contact shadow and reflection moving coherently. Transparent materials need plausible refraction and occlusion; a submerged object is one example. When the desired effect is a physical camera move, preserve coherent foreground/background perspective instead of shrinking an isolated subject over an unrelated scene.

Ask for one continuous shot and a settled ending when that is the selected direction. Avoid extra cuts, a second pullback, invented text, exposure shifts or a different object appearing at the end. Make these constraints specific to the scene rather than accumulating a generic negative-prompt list.

## Match the website to the actual film

Capture the opening and settled endpoint from the exact selected video through the target browser's decoded output where possible. Use the same frames for the page poster and settled foreground. An approximately similar still can expose differences in shape, colour or detail placement.

Compare subject colour, contour, recognisable details, supporting-surface texture, reflections and background exposure at the seams. For a drink, also inspect the rim and garnish; for a product, inspect its silhouette and markings. Keep source colour metadata and avoid blind re-encoding or relabelling colour spaces. Validate the rendered browser result rather than trusting matching file metadata alone.

If the final film has a soft background but the approved destination photograph is sharp, preserve the film's complete foreground plane and blend into that background across a broad, suitable region. Check the join at every viewport crop. Do not outline the subject as a cutout or paint a flat patch over a textured surface to disguise a mismatch.

Use the same approved source across desktop and phone when that composition works, with deliberate crop and framing adjustments. Separate generated variants can drift in subject identity and colour; use them only when the composition requires them and review their continuity explicitly.

## Repair temporal defects without creating new ones

Inspect the defect in motion and frame sequences, not only in a still. Decide whether it is part of a real impact, an existing surface mark or a generated inconsistency.

A repair on a moving surface must follow that surface's perspective. Use a stable repair region in tracked surface coordinates, temporally consistent texture, smooth illumination changes and appropriate foreground occlusion. Unrelated texture sampled independently each frame can flicker even when each still looks acceptable.

Keep changes local and preserve approved subject geometry, colour, camera movement and timing. Compare the opening, key action, camera move, occlusion and final hold at normal speed and in close-up. Numerical difference or stability measures can help locate problems; they do not prove perceptual realism. If a repair changes more than the requested defect, show it as a separate candidate rather than quietly replacing the approved shot.

## Prepare delivery and interaction

Save the source and finished clip under distinct names, exact endpoint stills, a short manifest and a review view. Record which output was accepted, rejected or merely generated. Keep prompts and receipts available in the project's private working files, without bundling account details into a shareable workflow.

Select playback control separately from camera direction. A camera turn can be timed, triggered or scroll-controlled. If scrolling must control the action from frame zero, the website must seek the entire clip without requiring a click first. Use a separate delivery derivative if frequent seeking needs different encoding; preserve the approved master.

## Verify and hand over

Review the first frame, key action timing, camera transitions and final frame in the browser. Check still-to-video and video-to-still handovers, colour continuity, subject and reflection integrity, and every repaired area in motion. Repeat at desktop and phone crops. Confirm the last frame remains stable without an unintended extra zoom.

Deliver a concrete preview, named approved and alternative versions, source/finished provenance, and any remaining limits. Separate successful encoding, perceptual approval and physical-device testing. Creating a local preview does not authorise publishing it.
