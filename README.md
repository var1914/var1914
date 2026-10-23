## Varun Rajput

ML platform engineer. I make models fast, measurable and correct in production. Right now that means
**inference performance for computer vision**: PyTorch, ONNX and TensorRT, and the serving systems around them.

11 years in production infrastructure, the last 5 on ML and data platforms.

### What I'm working on (October 2026)

**Open-source fixes, measured before and after**

- **torchmetrics** · [#3584](https://github.com/Lightning-AI/torchmetrics/pull/3584): multiclass stat scores built a
  `num_classes × num_classes` matrix, so memory grew with the square of the class count. One sample at 16k classes:
  1,956 MiB → 2.5 MiB. The 1M-class case from the issue: an 8 TB request → 134.5 MiB.
- **Ultralytics** · [#26850](https://github.com/ultralytics/ultralytics/pull/26850): on Apple GPUs, YOLO's per-stage
  timer didn't wait for the GPU, so most inference time showed up as postprocess (inference reported up to 14× too
  low at batch 16). Fix with before/after numbers on an M4 and an M5 Pro.

**[The Payload Is the Workload](https://github.com/var1914/image-serving-bench)**: a benchmark harness for image
inference. Per-request cost follows the payload (megapixels, format), not the model, and the usual autoscaling
signals can't see a shift in the payload mix. Testing a header-only cost signal as the fix.

**Postgraduate studies in AI**, University of Liverpool (currently the Deep Learning module).

### How I work

- Measure first, change second, and quote the number from the code that ships.
- Open-loop load, percentiles rather than means, paired A/B runs, identical-output checks.

### Background

- ML platforms on Kubernetes and AWS: training and serving pipelines with Airflow, Kubeflow and MLflow, across
  100+ EKS clusters and a 100+ GPU fleet.
- LLM serving: vLLM workers behind a job queue, which took document translation turnaround from ~20 min to ~5 s.
- Edge computer vision: ONNX → TensorRT engines for Jetson devices.

### Stack

PyTorch · ONNX / ONNX Runtime · TensorRT · vLLM · Kubernetes (EKS) · AWS · Terraform · Airflow · Kubeflow · MLflow ·
Prometheus / Grafana · Docker · Python

### Contact

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/varun-rajput-4096115a/)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:therajputvarun@gmail.com)

![Profile Views](https://komarev.com/ghpvc/?username=var1914&color=6366f1&style=for-the-badge&label=PROFILE+VIEWS)
