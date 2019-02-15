   Create/update the codepipeline stack by executing the following command (using your own AWS profile):
   
   ```
   aws cloudformation create-stack \
   --stack-name sls-codepipeline \
   --template-body file://./codepipeline/sls-codepipeline-codecommit-cf.yml \
   --capabilities CAPABILITY_NAMED_IAM
   ```
   
   ```
   aws cloudformation update-stack \
      --stack-name sls-codepipeline \
      --template-body file://./codepipeline/sls-codepipeline-codecommit-cf.yml \
      --capabilities CAPABILITY_NAMED_IAM
   ```
   
   Delete stack:
   ```
   aws cloudformation delete-stack \
   --stack-name sls-codepipeline
   ```
