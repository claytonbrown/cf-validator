# cf-validator
Cloud Formation Validator


Usage python cf-validator.py 
Parameters:

--cf_path [Required]: is the location of CloudFormation template in JSON format. Supported location:
	File system – path to CF template on file sytem
	Web – you can point to the file on web e.g. http(s)://my-file.com/my_cf.json
	S3 – also, you can point directly to AWS S3 bucket e.g. s3://my_bucket/my_cf.json

--cf_rules [Required]: is the location of JSON file with validation rules. Supporting the same locations like above. More about rules in next section.

--cf_res [Optional]: is the location of JSON file with define AWS resources that existence need to be confirm before launch CF template. More about resource in Resource section.

--allow_cap [Optional][yes/no]: this parameter control if you allow create IAM resources such as: policy, rules, IAM user by CF template. Default value is no

--region [Optional]: AWS region where existing resources were created. Default value: us-east-1
