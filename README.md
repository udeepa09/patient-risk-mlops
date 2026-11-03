# CardioTwin: Digital Twin Patient Risk MLOps Pipeline



## 🌐 Live Cloud Deployment
* **Live Web Dashboard:** [http://cardiotwin-deepa-2026.s3-website-ap-southeast-2.amazonaws.com](http://cardiotwin-deepa-2026.s3-website-ap-southeast-2.amazonaws.com)
* **API Gateway Endpoint:** `https://hahdp4mz63.execute-api.ap-southeast-2.amazonaws.com`

---

## 🛠️ Architecture & Tech Stack
* **Model:** XGBoost Classifier compiled to ONNX Runtime (`model.onnx`, 0.35 MB, Opset 15)
* **Training & Tracking:** Amazon SageMaker (`ml.t3.medium`) & MLflow
* **Serverless Compute:** AWS Lambda (`patient-risk-inference`) with ~0.203 ms warm latency
* **API Ingress:** Amazon API Gateway (HTTP API v2)
* **Data Lake:** Amazon S3 (`patient-risk-mlops`) with Object Versioning enabled
* **Frontend:** Responsive HTML5, TailwindCSS, SVG Avatar, and HTML5 Canvas ECG Monitor# patient-risk-mlops
