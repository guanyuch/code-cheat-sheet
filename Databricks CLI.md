pip install databricks-cli
databricks configure --token --profile MCT
databricks clusters list --profile MCT
databricks secrets create-scope --scope <scope-name> --profile MCT
databricks secrets put --scope <scope-name> --key <secret-key> --profile MCT
