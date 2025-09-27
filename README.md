🧬 Skin Cancer Lesion Segmentation with U-Net + ITTA-TLBO Optimization

Author: Boumediene Allaa Eddine



📖 Abstract

This project applies deep learning and hybrid metaheuristic optimization to the problem of skin cancer lesion segmentation.
We combine a U-Net convolutional neural network with a threshold optimization step powered by the hybrid Improved Tiki-Taka Algorithm (ITTA) and Teaching-Learning Based Optimization (TLBO).

Experimental evaluation on the Skin Cancer Lesions Segmentation dataset demonstrates that the proposed framework improves segmentation accuracy by adapting the probability threshold for binary mask generation.

🧾 Keywords

U-Net · ITTA · TLBO · Skin Cancer · Segmentation · Dice Score · Deep Learning · Optimization

📂 Dataset

Source: Skin Cancer Lesions Segmentation (Kaggle)

Size: 10,015 dermoscopic images with ground truth masks

License: CC-BY-NC-SA-4.0

⚙️ Methodology
🔹 Data Preparation

Images and masks resized to 128×128

Pixel values normalized

Dataset split into 80% training / 20% validation

🔹 Model Architecture: U-Net

Encoder–decoder CNN with skip connections

Loss: Binary Cross-Entropy

Optimizer: Adam

Trained for 10 epochs, batch size 16

🔹 Optimization with ITTA-TLBO

Instead of fixing the threshold at 0.5, we optimize the threshold using the ITTA-TLBO algorithm.

Objective: Maximize the Dice Similarity Coefficient (DSC)

Decision Variable: Probability threshold for binary mask generation

📊 Results

✅ Best Dice Score: 0.888

✅ Optimal Threshold: 0.4611

✅ Validation Accuracy: 93–94%

🏁 Conclusion

We presented a framework that combines U-Net segmentation with ITTA-TLBO threshold optimization for skin cancer lesion detection.
The optimized threshold significantly outperforms a fixed 0.5 threshold, demonstrating the potential of hybrid deep learning + optimization methods in medical image analysis.
