# Memory Mesh: Decentralized 4D Spatial Reconstruction
**Built for the AIDP GPU Competition (2026)**

## 🚀 The Vision
3D Gaussian Splatting (3DGS) is the breakthrough technology that allows us to turn 2D videos into fully interactive, photorealistic 3D environments. However, the hardware requirements are extreme: it requires high-end NVIDIA GPUs with at least 24GB of VRAM to process. Benchmark Focus: For this competition, we are utilizing the industry-standard Yellowhouse-12 (2GB) research dataset. This large-scale spatial data serves as the perfect benchmark to demonstrate how the AIDP Network handles massive parallel workloads that would otherwise crash consumer-grade hardware.

**Memory Mesh** democratizes 3D capture by using the **AIDP Decentralized GPU Network** to handle the heavy compute. Instead of needing a $3,000 workstation, users can offload the reconstruction to AIDP nodes for a fraction of the cost.

## 🛠 Technical Architecture (AIDP Integration)
Memory Mesh acts as the bridge between raw spatial data and AIDP’s high-performance compute:

1.  **Data Ingestion:** User captures 2D video frames.
2.  **GPU Request:** The system requests an **NVIDIA RTX 4090 or H100 node** via the AIDP marketplace based on VRAM requirements.
3.  **Decentralized Compute:**
    * **Phase 1 (COLMAP):** Extracts camera poses (High CPU/RAM).
    * **Phase 2 (Training):** Optimizes the Gaussian Splat (High GPU/VRAM).
4.  **Delivery:** The final `.ply` 3D file is served back to the user for AR/VR viewing.

## 📦 GPU Usage Depth
This project is designed to maximize AIDP’s infrastructure:
* **Target Chain:** Solana (SOL)
* **Compute Type:** Heavy Parallel Processing / CUDA
* **Recommended Hardware:** RTX 3090, 4090, A100, H100.
* **Depth:** This is not a simple API call. It involves full-scale model training that utilizes 90%+ of GPU capacity during the reconstruction phase.

## 📂 Repository Structure
* `engine.py`: The integration script for requesting AIDP nodes.
* `submission.txt`: Full project details and vision.

## 🔗 Links
* **AIDP Marketplace:** [Link to your project page]
* **Demo Video:** [Link to your X/Twitter or YouTube video]
* **Official Website:** [https://aidp.store](https://aidp.store)