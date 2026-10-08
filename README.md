```
git clone https://github.com/atulkamble/cloudformation.git
cd cloudformation
touch template.yaml
aws cloudformation validate-template --template-body file://template.yaml
aws cloudformation deploy --template-file template.yaml --stack-name myEC2stack
aws cloudformation delete-stack --stack-name myEC2stack

cd ..

cd s3
aws cloudformation validate-template --template-body file://template.yaml
aws cloudformation deploy --template-file template.yaml --stack-name mybucketstack
aws cloudformation delete-stack --stack-name mybucketstack

cd ..
```

