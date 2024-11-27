# AI Video Generator for Rare-Human Actions

This project is part of the assignment to set up and generate rare-human actions using an AI video generator. It integrates **Gradio** as the user interface and leverages AI models for captioning and generating new videos. Below is a comprehensive breakdown of the work, steps, and outputs.

---

## Objectives
1. **Input Video Workflow**: Create a workflow to upload videos via drag/drop or file selection using **Gradio**.
2. **Video Captioning**: Automatically caption the input video to describe the actions depicted.
3. **AI Video Generation**: Use the generated captions to create AI-based videos depicting rare-human actions.
4. **Side-by-Side Comparison**: Display the original input video and AI-generated video side-by-side for comparison.
5. **Documentation**: Provide clear instructions for setup, usage, and outputs.
6. **Demo**: Share an unlisted YouTube video demo and upload outputs to the GitHub repository.

---

## Implementation Breakdown

### Step 1: Video Input via Gradio
- **Task**: Allow users to upload videos through a drag-and-drop interface.
- **Implementation**: 
  - Used **Gradio Blocks** to create an intuitive interface.
  - Supported video formats include `.mp4`, `.avi`, and `.mov`.

---

### Step 2: Video Captioning
- **Task**: Generate concise descriptions of the uploaded video.
- **Implementation**:
  - Extracted frames using **OpenCV**.
  - Provided a basic captioning mechanism for demonstration purposes:
    - Each frame is summarized as part of the overall video context.
    - Descriptions are combined into a single meaningful caption.
  - Future Extension: Use advanced captioning models (e.g., **BLIP**, **LLaVA**) for richer descriptions.

---

### Step 3: AI Video Generation
- **Task**: Use the generated captions to create new AI-based videos.
- **Implementation**:
  - Suggested model: **OPS AI Generator** (currently being integrated).
  - Used **Stable Diffusion** to prototype generation:
    - Generated multiple frames based on the caption.
    - Combined frames into an AI-rendered video.

---

### Step 4: Side-by-Side Comparison
- **Task**: Display both the input video and the AI-generated video for easy comparison.
- **Implementation**:
  - Used Gradio’s layout tools to render both videos in parallel columns.

---

### Step 5: Documentation and Outputs
- **Demo Video**: Uploaded to YouTube as an unlisted video. [Watch here](https://youtu.be/unlisted-demo-link).
- **Sample Outputs**: 
  - Input videos sourced from **Charades Dataset** and sample synthetic videos provided by the TA.
  - AI-generated videos available in the GitHub repository.

---

## How to Set Up

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-repo/ai-video-generator.git
   cd ai-video-generator

