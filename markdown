# Oort DSS GitHub Integration

This repository provides a seamless integration between GitHub and Oort DSS, allowing you to easily upload files from your GitHub repository to Oort DSS for secure and scalable data storage.

## Usage

To use this GitHub Action, add the following step to your workflow:

```yaml
- name: Upload to Oort DSS
  uses: actions/oort-dss-upload-action@v1
  with:
    path: ./build
    oortEndpoint: ${{ secrets.OORT_ENDPOINT }}
    oortAccessKey: ${{ secrets.OORT_ACCESS_KEY }}
    oortSecretKey: ${{ secrets.OORT_SECRET_KEY }}
    oortBucket: 'my-bucket'
