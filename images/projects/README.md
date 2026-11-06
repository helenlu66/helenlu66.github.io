# Portfolio preview sources

Images are retained locally so project cards do not depend on third-party image hosting.
Titles, venues, and destination links were taken from HelenLu_RoboticsIntern_10222026.pdf.

| Preview | Source |
| --- | --- |
| hybrid-planning.jpg | https://helenlu66.github.io/hybridLLMguided/static/images/plan-learn-execute%20loop.png |
| vla-symbolic.jpg | Figure 1, page 3: https://hrilab.tufts.edu/publications/luetal25icad.pdf |
| price-not-right.jpg | https://price-is-not-right.github.io/static/images/overview.png |
| few-shot.jpg | Figure 1, page 2: https://hrilab.tufts.edu/publications/lorangetal25corl.pdf |
| curiosity.jpg | Figure 1, page 1: https://hrilab.tufts.edu/publications/lorangetal25icra.pdf |
| collaboration.jpg | Figure 1, page 2: https://hrilab.tufts.edu/publications/luetal24icsr.pdf |
| multinet-v2.jpg | https://multinet.ai/static/images/maze_figure.png |
| multinet-v1.jpg | https://multinet.ai/static/images/Multinet%20v1%20release%20visual%20final.png |
| texture-sort.jpg | https://raw.githubusercontent.com/helenlu66/texture_sort/main/demo/task_sequence.png |

Paper figures were cropped to exclude surrounding text. Previews were resized and converted to JPEG; transparent backgrounds were rendered on white.

## Animated previews

GIFs use real project footage; the JPEGs remain as static fallbacks. Reduced-motion preferences show stills by default. Animated cards retain matching stills for reduced-motion preferences.

| GIF | Source | Processing |
| --- | --- | --- |
| hybrid-planning.gif | https://helenlu66.github.io/hybridLLMguided/static/videos/pick-up-lid-from-pot.mp4 | Full 3.75-second clip, original speed, 360 px wide, 10 fps |
| price-not-right.gif | https://price-is-not-right.github.io/static/videos/nsm-hanoi.mp4 | Full demo at 8x speed, 360 px wide, 8 fps |
| multinet-v2.gif | https://multinet.ai/static/videos/r1_reels/r1_M3_8x8_corridor_kr_sg_1__opus48_FAIL.mp4 | Recorded failure episode at 3x speed, 480 px wide, 10 fps |
| texture-sort.gif | https://raw.githubusercontent.com/helenlu66/texture_sort/main/demo/tactile_classification_phase.webp | Source frames 220-320, with the GelSight tactile image and robot camera shown side by side; approximately 2x speed, 640 px wide. The static fallback shows tactile contact at source frame 280. |

### Co-creative dialogue and placement preview

`cake-dialogue-placement.gif` and its matching JPEG use 48.0–58.7 seconds of the original `cake_decoration_demo_iros.mp4` (Cake Decoration Files). The robot picks up the mint macaron and places it at a3 in response to the human's correction. The relevant robot suggestion and human reply are retained at full width above the robot view. The 800 × 450 GIF runs at 10 fps, with a short final-frame hold; the card disables hover zoom to preserve the dialogue edges. The JPEG is the reduced-motion fallback.

`vla-tug.jpg` uses the overview figure from https://vla-tug.github.io/assets/img/overview.png, resized to 1200 pixels wide. The full architecture and runtime failure-detection panels are retained.

`vla-tug.gif` uses the first 10 seconds of the agent and wrist videos at https://vla-tug.github.io/media/rollouts/ep2/ (640 × 360, 10 fps). The monitoring/alarm label follows the episode metadata: alarm step 11 × 0.4 seconds = 4.4 seconds, wrong-object failure. `vla-tug-demo.jpg` is its reduced-motion fallback.

`vla-tug-mushroom.gif` and its JPEG fallback use synchronized external (`/cameras/925622071555`) and wrist (`/cameras/onboard`) camera frames from the user-provided `mushroom_steer_probe.rrd`. The preview includes the failure prediction (93.2%, 1.317 s), all five logged corrective nudges (+Y 6.49 s, -Z 9.87 s, -Z 13.56 s, -X 16.94 s, +X 19.25 s), policy restart (25.65 s), and grasp/placement. Camera sampling is sparse while paused; recorded nudge frames are retained, waits between corrections are shortened and explicitly labeled, and recording timestamps remain visible. No missing motion is synthesized. Output: 800 × 450, 10 fps.

The mushroom preview displays the user-confirmed instruction “Task: Put the mushroom on the plate” throughout playback.

`hybrid-robot-montage.gif` and its JPEG fallback use the five task videos from https://helenlu66.github.io/hybridLLMguided/. Task labels are copied verbatim from the webpage captions, in order: “Pick up lid from pot”, “Pick up from open box”, “Pick up nut from peg”, “Open drawer”, and “Pick up from open drawer”.

`price-comparison.gif` and its JPEG fallback compare the complete `pi0-hanoi-end-to-end.mp4` and `nsm-hanoi.mp4` demos from https://price-is-not-right.github.io/static/videos/. Both play at 4× speed; the shorter neuro-symbolic demo holds its last frame. Method labels are copied from the webpage (“End-to-End VLA”, “Neuro-Symbolic Method”); “Play Towers of Hanoi” comes from the original `e2e-vla.en.vtt` subtitle. Output: 800 × 450 at 10 fps. No outcomes or energy figures are added to the footage.
