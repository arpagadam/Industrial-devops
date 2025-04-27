# DevSecOps
DevSecOps zero to hero: A comprehensive guide

📋 DevOps Tools and Commands Mastery Checklist

🖥️ 1. Linux Essentials
Tool	           Must-Know Commands
bash	           if, for, while, functions, arrays
systemctl	       systemctl status, restart, enable, logs
journalctl	       journalctl -xe, journalctl -u service-name
network tools	   netstat, ss, tcpdump, ping, traceroute, curl, wget, iptables, rsync
file tools	       lsof, fuser, find, grep, awk, sed, cut, which, whereis
strace	           strace -p PID, strace -e openat <command>, top, htop
disk tools         smartctl, watch
ssh


☁️ 2. Cloud (AWS/GCP/Azure)
Tool	        Must-Know Skills
AWS CLI	        aws ec2 describe-instances, aws s3 cp, aws iam list-users
VPC	            Create Subnets, NAT Gateways, Route Tables
IAM	            Create Roles, Policies, AssumeRole
EC2	            Launch/Terminate instances, EBS snapshots
S3	            Versioning, Lifecycle policies, Static website hosting
CloudWatch	    Alarms, Log Groups, Metric Insights

⚙️ 3. Infrastructure as Code (Terraform)
Tool	             Must-Know Commands/Skills
terraform init	     Initialize a project
terraform plan	     Preview changes
terraform apply	     Apply infrastructure changes
terraform destroy	 Destroy resources
modules	Create reusable modules (e.g., VPC module, EC2 module)
remote backend	Use S3/dynamoDB locking for Terraform state


🐳 4. Containers (Docker & Kubernetes)
Tool	              Must-Know Commands/Skills
docker build	      Build Docker images
docker-compose	    Multi-container applications
docker logs, docker exec	Debug containers
kubectl get, describe, logs, exec	Managing pods and debugging
Helm	Install and configure apps via Helm charts
K8s Ingress	Setup NGINX ingress controller and configure routing

🔁 5. CI/CD Pipelines (Jenkins, GitHub Actions, GitLab)
Tool	                 Must-Know Concepts
Jenkins pipelines	     Write Jenkinsfile with stages (build, test, deploy)
GitHub Actions	         Write .github/workflows/*.yml for CI/CD
artifacts	             Save and retrieve artifacts between stages
Secrets management	     Store secrets in CI tools securely
Build triggers	         Webhooks, schedule-based triggers, manual approvals
📈 6. Monitoring, Logging, Alerting

Tool	          Must-Know Setup
Prometheus	      Install, add targets, setup basic alerts
Grafana	          Create dashboards from Prometheus or Loki
Alertmanager	  Configure alert rules, route to Slack/email
ELK Stack	      Logstash, Elasticsearch, Kibana basics


🔒 7. Security Tools
Tool	              Must-Know Skills
Vault (HashiCorp)	  Store, read, and inject secrets
AWS Secrets Manager	  Store/rotate secrets automatically
SSL/TLS	              Generate certs using OpenSSL, configure nginx/apache with SSL
IAM fine-grained	  Restrict S3, EC2 access properly


🛡️ 8. Backup, Disaster Recovery
Tool	                 Must-Know Concepts
AWS Backup	             Schedule backup plans
EBS Snapshots	         Automate volume snapshots
RDS Snapshots	         Backup and restore databases
Multi-AZ Deployments	 High availability across availability zones


📦 9. Version Control (Git)
Git Commands	Skills
git init, clone, pull, push, fetch	Basic repo management
git branch, merge, rebase	Branch management
git revert, cherry-pick	Handling mistakes and patches
git stash	Managing uncommitted changes

=============================================================================================================

🚀 Pro Mode:
Create a GitHub portfolio where you showcase:

A Kubernetes cluster setup

CI/CD pipelines

Terraform modules for cloud resources

Monitoring setup with Prometheus & Grafana

Bash and Python automation scripts

===============================================================================================================

Keep notes (for revision during interviews)

🎯 Final Tip:
"Be someone who can not just operate systems, but can design, debug, and scale them confidently under pressure."

That's real Senior DevOps material! 🔥
