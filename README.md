## Varun Rajput

ML platform engineer. I make models fast, measurable and correct in production. Right now that means
**inference performance for computer vision**: PyTorch, ONNX and TensorRT, and the serving systems around them.

11 years in production infrastructure, the last 5 on ML and data platforms.

### Merged open-source PRs

- **Ultralytics** · [#26942](https://github.com/ultralytics/ultralytics/pull/26942): PyTorch's idle OpenMP threads were
  busy-waiting on the cores ONNX Runtime and OpenVINO need. Capping them at 2 made CPU prediction up to 2× faster on
  8 vCPUs, with identical outputs.
- **Ultralytics** · [#26897](https://github.com/ultralytics/ultralytics/pull/26897): YOLO loads the next image while
  OpenVINO runs inference on CPU, 7–8% faster at batch 1 on 2- and 4-core VMs, with identical outputs.

### How I work

- Measure first, change second, and quote the number from the code that ships.
- Open-loop load, percentiles rather than means, paired A/B runs, identical-output checks.

### Background

- Postgraduate studies in AI, University of Liverpool.
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
