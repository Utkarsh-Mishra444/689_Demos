# 🤖 Robotics Video Model Comparison - CSCE 689

A comprehensive comparison of AI video generation models for robotic manipulation tasks.

## 📊 Overview

This project evaluates the performance of various AI video generation models on standardized robotic manipulation tasks. Each model generates videos for 5 distinct robotics scenarios, allowing for side-by-side comparison of visual quality, motion realism, and task completion accuracy.

## 🎯 Tasks

The benchmark consists of 5 robotic manipulation tasks:

1. **T1: Pour water into mug** - Robot arm picks up bottle and pours into mug
2. **T2: Place spatula on pan** - Robot arm moves spatula into frying pan
3. **T3: Wipe crumbs off table** - Robot arm uses sponge to clean table surface
4. **T4: Lift lid from pot** - Robot arm removes lid from cooking pot
5. **T5: Push cube to target marker** - Robot arm pushes cube to marked location

## 🤖 Models Compared

### ✅ Completed Models
- **Grok** - xAI's video generation model
- **Veo2** - Google's video generation model
- **Veo3.1Fast** - Google's fast inference variant
- **Veo3.1Quality** - Google's high-quality variant
- **Wan** - [Model details pending]

### ⏳ Pending Models
- **Sora** - OpenAI's video generation model
- **Cosmos** - [Model details pending]

## 📁 Project Structure

```
├── Grok_Videos/
│   ├── Grok/           # Grok-generated videos (T1-T5_Grok.mp4)
│   ├── Veo2/           # Veo2-generated videos (T1-T5_Veo2.mp4)
│   ├── Veo3.1Fast/     # Veo3.1Fast videos (T1-T5_Veo3.1Fast.mp4)
│   ├── Veo3.1Quality/  # Veo3.1Quality videos (T1-T5_Veo3.1Quality.mp4)
│   ├── Base_Images/    # Base images for each task (T1-T5_Base.png)
│   └── For later/      # Additional content
├── index.html          # GitHub Pages comparison interface
├── README.md           # This file
└── CSCE 689 Video Prompts - Robotics.csv  # Task definitions and status tracking
```

## 🚀 Viewing the Comparison

The interactive comparison interface is available via GitHub Pages. Simply open `index.html` in a web browser to view all videos side-by-side.

## 📋 Task Details

Each task includes:
- **Video Prompt**: Detailed description for video generation
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
