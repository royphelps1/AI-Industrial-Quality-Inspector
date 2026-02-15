
1) Project Title
AI Industrial Quality Inspector
Multi-class surface defect classification + explainable AI (Grad-CAM)
2) One-line Pitch (VC style)
A computer-vision tool that automatically classifies surface defects in manufacturing images and highlights where the defect is, reducing inspection time and inconsistency.
3) Problem + Market Gap
Manual inspection is slow, subjective, and expensive. Existing inspection tools often require heavy tuning, don’t generalize well across defect types, and can be hard to trust without visual explanations.
4) Proposed Solution
Fine-tune a pretrained CNN to classify defect type from an image and generate Grad-CAM heatmaps to show the image regions driving the prediction.
5) Technical Approach (CS-614 option)
Option B: Fine-tune an existing model on a new dataset. 
CS 614 Applications of Machine …
Model: pretrained ResNet18
Task: multi-class classification (defect categories)
Explainability: Grad-CAM overlays
6) Dataset Plan
Primary: NEU Surface Defect Dataset (steel surface defect images; multiple defect classes).
Data stored locally under: data/raw/ (not committed to Git).
7) Success Metrics
Overall accuracy on held-out test set
Confusion matrix (per-class performance)
Qualitative demo examples (correct and incorrect predictions)
Grad-CAM overlays that plausibly focus on defect regions
8) Proof-of-Concept Demo (what we will show)
Input image → predicted defect class + confidence → Grad-CAM heatmap overlay.
Include 2–3 demo images in slides/video.
9) Deliverables
Slide deck + recorded video with: problem statement, technical approach, dataset stats, results, and demo 
CS 614 Applications of Machine …
Code + run instructions zipped for submission 
CS 614 Applications of Machine …
10) Risks + Mitigations
Class imbalance → weighted sampler / class weights
Overfitting on small dataset → augmentation + early stopping
Grad-CAM complexity → use a known minimal implementation; validate on a few images
11) Team Roles (3 people)
Roy: model training pipeline + evaluation + Grad-CAM integration
Teammate 2: dataset prep + experiments/augmentation comparisons + dataset stats
Teammate 3: pitch narrative + slides + video assembly + demo flow
12) Project Timeline (simple)
Week 1: dataset + baseline ResNet18 fine-tune + metrics
Week 2: Grad-CAM + demo images + slide draft
Week 3: polish + final recording + submission zip