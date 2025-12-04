# 🤖 CSCE 689 Video Benchmarks

A comprehensive comparison of AI video generation models across two benchmark suites:
- **Robotics manipulation tasks** (index.html)
- **Classical physics experiments** (physics.html)

## 📊 Overview

This project evaluates the performance of various AI video generation models on standardized robotic manipulation tasks. Each model generates videos for 5 distinct robotics scenarios, allowing for side-by-side comparison of visual quality, motion realism, and task completion accuracy.

## 🎯 Robotics Tasks

The robotics benchmark consists of 5 manipulation tasks:

1. **T1: Pour water into mug** - Robot arm picks up bottle and pours into mug
2. **T2: Place spatula on pan** - Robot arm moves spatula into frying pan
3. **T3: Wipe crumbs off table** - Robot arm uses sponge to clean table surface
4. **T4: Lift lid from pot** - Robot arm removes lid from cooking pot
5. **T5: Push cube to target marker** - Robot arm pushes cube to marked location

### Models Compared
**Grok**, **Sora**, **Veo2**, **Veo3.1Fast**, **Veo3.1Quality**, **Wan2.1**

## ⚛️ Physics Tasks

11 analytical physics prompts grouped into buoyancy (B), collisions (C), and gravity (G):
- **B1 Heavy Sink** – Steel ball sinks in tank
- **B2 Light Float** – Hollow ball floats to surface
- **B3 Pop-up** – Submerged block shoots upward
- **C1 Elastic Head-On** – Perfectly elastic billiard collision
- **C2 Glancing Blow** – Off-center billiard collision
- **C3 Tower Topple** – Sliding block knocks over tower
- **C4 Springs** – Cart compresses spring against wall
- **G1 Earth Fall** – Ball dropping under Earth gravity
- **G2 Moon Fall** – Ball drop with lunar gravity
- **G3 Vacuum Drop** – Hammer & feather fall equally
- **G4 Projectile Arc** – Launcher fires projectile trajectory

### Models Compared
**Grok**, **Sora2**, **Veo2**, **Veo3**, **Wan2.1**

## 📁 Project Structure

```
├── Grok_Videos/
│   ├── Grok/           # Grok-generated videos (T1-T5_Grok.mp4)
│   ├── Veo2/           # Veo2-generated videos (T1-T5_Veo2.mp4)
│   ├── Veo3.1Fast/     # Veo3.1Fast videos (T1-T5_Veo3.1Fast.mp4)
│   ├── Veo3.1Quality/  # Veo3.1Quality videos (T1-T5_Veo3.1Quality.mp4)
│   ├── Base_Images/    # Base images for each task (T1-T5_Base.png)
│   └── For later/      # Additional content
├── Physics/            # Physics videos, base images, prompts
├── physics.html        # Physics comparison interface
├── index.html          # Robotics comparison interface
├── README.md           # This file
└── CSCE 689 Video Prompts - Robotics.csv  # Task definitions and status tracking
```

## 🚀 Viewing the Comparisons

- `index.html` → Robotics manipulator benchmark
- `physics.html` → Physics experiment benchmark
Host both via GitHub Pages or open locally with `python3 -m http.server`.

## 📋 Task Details

Each benchmark task includes:
- **Video Prompt**: Detailed description for video generation (CSV files)
- **Image Prompt**: Base image generation instructions
- **Base Images**: Starting visual context for video generation

## 🛠️ Technical Notes

- All videos use consistent naming: `T{task_number}_{Model}.mp4`
- Base images follow pattern: `T{task_number}_Base.png`
- Franka Emika Panda robot arm used in all scenarios
- Fixed camera perspectives (side view for manipulation tasks, top-down for planar tasks)

## 📊 Evaluation Criteria

Videos can be evaluated on:
- **Motion Realism**: Natural, physics-accurate movements
- **Task Completion**: Successful execution of intended action
- **Visual Quality**: Sharpness, lighting, and detail
- **Temporal Consistency**: Smooth, coherent motion over time

## 🤝 Contributing

This is a research project for CSCE 689. Additional model implementations and evaluation metrics are welcome.

## 📄 License

[Add appropriate license information]
