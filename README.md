# HOG + SVM Face Detection

A legacy Python face-detection code repository using Histogram of Oriented Gradients (HOG), a support vector machine (SVM), multi-scale sliding windows and non-maximum suppression.

## Source attribution

The existing commit history credits [azowilson](https://github.com/azowilson) and references the [original repository](https://github.com/azowilson/Final-year-project-face-detection-). That authorship and history are preserved. This repository should not be read as a claim of sole original authorship by its current owner.

## Code overview

| File / directory | Role |
| --- | --- |
| `face_detector_scratch.py` | Main training/loading and image detection workflow |
| `SVM.py` | SVM implementation used by the detector |
| `CV2HOG.py`, `get_hog.py` | HOG feature extraction utilities |
| `non_max_suppression.py` | Filters overlapping candidate detections |
| `model/` | Stored model files |
| `testimg/` | Example test-image directory |
| `Final Report.pdf` | Existing project report |
| `requirements.txt` | Historical package/version table |

## Running the historical code

The actual entry filename is **`face_detector_scratch.py`**.

1. Review the source and dependency versions in an isolated Python environment.
2. Reconstruct and test a compatible dependency environment. The existing `requirements.txt` is a package/version table, not a directly usable pip requirements file.
3. Check `model_path` and `testPath` in the entry script. The model path uses a Windows-style separator.
4. If training is needed, replace the hard-coded `trainPath` with the path to your own labelled training data.
5. Once the environment and paths are valid, run:

```bash
python face_detector_scratch.py
```

The script displays detection windows through OpenCV, so a desktop/GUI environment is required for that display path.

## Results & maintenance status

The original README reported approximately 80% average detection accuracy. That historical figure has not been independently reproduced in this documentation update, and the dataset, metric definition and evaluation protocol should be checked before relying on it.

This update improves documentation only. The source code and original commit history are retained; runtime compatibility has not been revalidated.

---

[Current IT & Networking portfolio](https://hmahadi810.github.io/) · [LinkedIn](https://www.linkedin.com/in/hmahadi810/)
