# How to connect to EC Instance without SSH on AWS
## Use EC2 instance connect through AWS

- Enter venv with:
```bash
source /var/app/venv/staging-LQM1lest/bin/activate
```

- Access project with:
```bash
cd /var/app/current
```

- You can load the environment variables required by running the following commands
```bash
sudo yum install -y jq
```
```bash
/opt/elasticbeanstalk/bin/get-config environment | jq -r 'to_entries|map("export\(.key)=\(.value|tostring)")|.[]' > ~/env_vars.sh
```
```bash
source ~/env_vars.sh
```

- To install postgres, run:
```bash
sudo dnf install postgresql15
```

## You can obtain the username and password of a database with the following command:
```bash
/opt/elasticbeanstalk/bin/get-config environment
```
