<p align="center">
<img height="200" src="static/aws-threathunting.png">
<br>AWS CloudTrail Threat Hunting 
</p>

Welcome to the CloudTrail AWS Threat Hunting Repository! This repository serves as a comprehensive resource for enhancing your threat detection and hunting capabilities within your AWS environment using AWS CloudTrail and other AWS services. Whether you are new to threat hunting or a seasoned pro, this repository offers valuable insights and tools to supercharge your security efforts.

## Abstract

CloudTrail is the central logging source for each AWS account. It provides a perfect foundation for creating threat hunting queries, which can be used for offline analysis or integrated into a SIEM based on Athena, (H)ELK, Splunk, or a custom solution.

The CloudTrail dataset can be enriched with information such as geoIP, threat data, access level, and MITRE ATT&CK TTPs.

Other AWS offerings that can provide deeper insights into your AWS environment include S3 bucket access logs, VPC FlowLogs, VPC DNS queries (collected over Route 53 Resolver Query Logs), CloudWatch Logs, load balancer access logs, and traffic mirroring (one of the most awesome features of Nitro Instances).

All or even a subset of these log sources can be used to build a mature threat hunting and alerting system for your AWS cloud.

More ideas for hunting queries can be found in my [Blog](https://benjitrapp.github.io/defenses/2023-06-30-AWS-cloudtrail-ir/)

**Happy hunting!**

## Contents

This repository includes the following resources:

1. [Jupyter Notebook](http://localhost:8888/notebooks/hunting-cloudtrail-flaws-cloud.ipynb): A comprehensive Jupyter Notebook with insightful plots and examples of Threat Hunting Queries based on CloudTrail.
2. [Cloud Trail Logs](https://github.com/BenjiTrapp/aws-threat-hunting/tree/main/cloudtrail/flaws_cloudtrail_logs): These logs were released by Scott Piper anonymized CloudTrail logs from [flaws.cloud](https://flaws.cloud) which contain real malicious events, to practice some Threat Hunting capabilities

## Threat Hunting Playbook meets Jupyter Notebook

Explore and leverage the power of threat hunting within your AWS environment using our Jupyter Notebook. This notebook provides detailed examples, visualizations, and step-by-step guides to help you get started with CloudTrail-based threat hunting.

### Getting Started

To get started with the Jupyter Notebook, follow these steps:

1. Clone this repository to your local machine or AWS environment.
2. Open the Jupyter Notebook and follow the instructions provided within the notebook.
3. You want at least the following pip dependencies:
   ```python
   pandas
   matplotlib
   tabulate
   seaborn
   ```

### Note

Make sure you have the necessary permissions and credentials to access your AWS environment and CloudTrail logs before running any queries in the notebook against your real data. The data used within the demo are real malicious provided by Scott Piper 

## How to Contribute

We welcome contributions from the community to improve and expand the capabilities of this repository. If you have ideas, improvements, or additional resources to share, please feel free to submit a pull request.

## License

This repository is licensed under the [MIT License](LICENSE).

---

Thank you for visiting the CloudTrail Threat Hunting Repository. I hope this resource enhances your AWS security efforts and helps you better protect your cloud environment. Happy hunting! 🌟

[![Follow Me on GitHub](https://img.shields.io/github/followers/yourgithubusername.svg?style=social&label=Follow)](https://github.com/BenjiTrapp)

**Maintained with ❤️ by [BenjiTrapp](https://github.com/BenjiTrapp)**
