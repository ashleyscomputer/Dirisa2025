# Driver Behaviour Detection --- YOLOv12 + Risk Scoring + XAI

This project implements a **driver-behavior detection system** using
**Ultralytics YOLOv11**, extended with:

-   Model persistence no need to re-train on every run
-   Full evaluation pipeline, including confusion matrices, precision/recall, accuracy, and metric charts
-   Training & validation loss curves
-   A risk scoring layer on top of YOLO detections
-   Integrated Explainable AI (XAI) visualizations
-   Video inference with user-uploaded inputs

## Table of Contents

1.  Project Overview
2.  Model Architecture
3.  Methodology
4.  Model Saving
5.  Video Inference
6.  Project Structure
8.  Future Work

## Project Overview

The goal is to automatically detect risky driver behaviour using computer
vision, assigning a risk score per frame and providing model
explainability visualizations.

## Model Architecture

Uses YOLOv11 with a CSPDarknet-style backbone, PAN-FPN neck, and
decoupled detection head. Custom training based on driver-behaviour
datasets.

## Methodology

### Dataset

COCO-format dataset with preprocessing, balancing, and augmentation.

### Training Workflow

Training YOLOv11 with metrics tracking, loss curves, and model
checkpointing.

### Risk Scoring Layer

Adds a post-processing score based on detection class, confidence, and
bounding box impact.

### Explainable AI

Per-frame explanation reports.

### Evaluation

Outputs mAP50, mAP50-95, precision, recall, confusion matrix, bar
charts, and loss curves.

## Model Saving

Supports YOLO `.pt` weight saving plus serialized risk/XAI layers via
`joblib`.

## Video Inference

Allows user to upload videos and generate annotated outputs with risk
scoring and XAI overlays.
