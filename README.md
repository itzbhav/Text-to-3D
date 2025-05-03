# Text-to-3D Model Generator (Prototype)

## 📌 Overview

This prototype accepts a **short text prompt** (e.g., “a small toy car”) and generates a **basic 3D model** (.obj and .ply formats) using **OpenAI’s Shap-E model**. It also visualizes the rendered model in the browser UI.

---

## 🎯 Features

- ✅ Accepts text prompts to generate 3D models
- ✅ Uses a pretrained open-source model (Shap-E)
- ✅ Outputs a 3D `.obj` and `.ply` file
- ✅ Displays a basic 3D image preview
- ✅ Clean Gradio UI for user input/output
- ✅ Compatible with CPU and GPU

---

## 🏗️ Architecture

```text
User Prompt ──> Shap-E (text300M model)
                ↓
         Latent 3D Representation
                ↓
    Transmitter Model + Virtual Cameras
                ↓
      Rendered Image + Mesh (.obj/.ply)
## Output
![3D-OUTPUT](3D-OUTPUT.png)

