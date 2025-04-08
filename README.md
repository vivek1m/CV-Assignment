# 🔍 Feature Detection Parameter Tuning
This project explores how tweaking key parameters affects feature detection and matching accuracy using:

🧠 SIFT Feature Matching

🏔️ Harris Corner Detection

🎯 Shi-Tomasi Corner Detection

📋 Experiment Summary
I tuned important parameters and observed their effects on accuracy, noise, and false matches.

🧠 SIFT Feature Matching
Initial Ratio Threshold: 0.75

Changes:

🔼 0.80 ➔ More matches, but more false matches.

🔽 0.70 ➔ Fewer false matches, missed valid points.

🏔️ Harris Corner Detection
Initial Sensitivity Factor (k): 0.04

Changes:

🔼 0.05 ➔ Fewer corners, missed edges.

🔽 0.03 ➔ More corners, but with noise.

Initial Block Size: 3

Changes:

🔼 4 ➔ More robust detection, missed fine details.

🔽 2 ➔ More corners detected, but noisy.

🎯 Shi-Tomasi Corner Detection
Initial Quality Level: 0.01

Changes:

🔼 0.015 ➔ Stronger corners, fewer detections.

🔽 0.005 ➔ More corners, but some false ones.

Initial Minimum Distance: 10

Changes:

🔽 8 ➔ Clustered detections, redundancy.

🔼 12 ➔ Spaced detections, missed key points.
🛠️ Requirements
Python 3.x 🐍

OpenCV 📸

NumPy 📊

✨ Final Insight
Tuning parameters greatly impacts feature detection results. ⚡
Fine-tuning is necessary based on your application to balance between accuracy, robustness, and noise! 🎯

