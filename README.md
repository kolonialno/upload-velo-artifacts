<h1 align="center">
  🚲 <br>
  Upload Velo artifacts
</h1>

<p align="center">
  A GitHub Action to upload Velo deployment artifacts
</p>

This GitHub actions is part of the Velo deploy system at Oda.

## Usage


```yaml
name: Upload deploy artifacts

on: push

jobs:
  upload-deploy-artifacts:
    runs-on: ubuntu-latest
    steps:
      - uses: kolonialno/upload-velo-artifacts@v1
        with:
          google_service_account_credentials_json: ${{ secrets.<secret name> }}
          google_cloud_storage_bucket_name: <bucket name>
```
