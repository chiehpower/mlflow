# MLFlow

### Usage

Launch the mlflow server.

```
mlflow ui
## Or
mlflow server 
```

 view it at [http://localhost:5000](http://localhost:5000/).

### Installation

```
pip3 install mlflow
```



### Troubleshooting

When we click the models on mlflow page, it shows this error:
```
[BUG] - INVALID_PARAMETER_VALUE: Model registry functionality is unavailable; got unsupported URI
```

### Solution:

Launch the mlflow server again.

```
mlflow server --backend-store-uri sqlite:///:memory --default-artifact-root ./mlruns
```

