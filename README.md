# Memory Mesh: Decentralized 4D Spatial Reconstruction
**Official Submission for the AIDP GPU Competition (2026)**

## 🚀 Project Vision
3D Gaussian Splatting (3DGS) is the future of digital twins, but the hardware barrier is too high for the average user. Processing high-resolution research datasets requires enterprise-grade GPUs with 24GB+ VRAM.

**Memory Mesh** democratizes this by using the **AIDP Decentralized GPU Network**. Our platform offloads the heavy "Splat Training" phase to remote AIDP nodes on the Solana chain, turning hours of local processing into minutes of high-performance compute.

## 📊 Dataset 
Waterlily House (Insta360 Spatial Capture) Processing: 30,000 training iterations simulated via AIDP GPU nodes. Result: High-fidelity 4D reconstruction of complex organic environments.
## 🛠 Technical Architecture (AIDP Integration)
Memory Mesh acts as the bridge between raw spatial data and AIDP’s high-performance compute:
## 🛠 Technical Architecture (AIDP Integration)
Memory Mesh acts as the bridge between raw spatial data and AIDP’s high-performance compute:

1.  **Ingestion:** User uploads 2GB+ of spatial data (Images/Video).
2.  **GPU Orchestration:** The system requests a high-VRAM node via the AIDP marketplace.
3.  **Distributed Training:** * **Phase 1:** Structure from Motion (SfM) via COLMAP.
    * **Phase 2:** Neural Rendering Optimization (30,000 iterations).
4.  **Delivery:** The final `.ply` spatial file is delivered to the user for VR/AR viewing.

## 📦 How to Run the Benchmark
To see the AIDP integration in action, run our performance simulator:
```bash
python run_benchmark.py

