# ♻️ Recycling-AI: Basic Artificial Garbage Sorter (B.A.G.S)

> “You don’t have to feel like a waste of space for trying to recycle.”

Welcome to **Recycling-AI**, where we blend tech with sustainability!  
We know the recycling system isn’t perfect, but we’re doing our part to make it better — one plastic bag at a time.

## 🎯 What is B.A.G.S?

**B.A.G.S** stands for **Basic Artificial Garbage Sorter** — a computer vision tool that detects plastic bags and helps sort recycling more accurately, preventing contamination and preserving valuable recyclables.

- 🔍 Uses **YOLOv5** for object detection  
- 🧠 Custom-trained model with **70–90% confidence** detecting various plastic bag types  
- 🧪 Built with **OpenCV** and **Python** for backend processing  
- 🚀 Room to grow — detection for bubble wrap, plastic straws, and more coming soon!

---

## 🖥️ Run the Web App

Clone the repo, make sure Python dependencies are installed, then run the app using the options below:

### ⚙️ Command Line Options

| Option             | Description                                           | Default           |
|--------------------|-------------------------------------------------------|--------------------|
| `-i`, `--ip`       | IP address of the device (**required**)              | N/A                |
| `-o`, `--port`     | Port number of the server (**required**)             | N/A                |
| `-f`, `--frame_count` | # of frames to build background model             | `32`               |
| `-m`, `--model`    | Model to use (`katy_perry.pt`, `paty_kerry.pt`)     | `katy_perry.pt`    |
| `-b`, `--backend`  | Backend: `cuda` or `cpu`                             | `cuda` (if available) |

### ▶️ Example:
```bash
python app.py --ip 0.0.0.0 --port 8000 -m paty_kerry.pt
