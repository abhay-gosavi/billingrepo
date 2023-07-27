# billingrepo

This Python script uses Boto3 (the AWS SDK for Python) to retrieve billing details using the AWS Cost Explorer API. It fetches the unblended cost for a specified date range and granularity.

## Prerequisites

Before running the script, ensure you have the following:
- Python installed on your machine.
- Boto3 library installed. If not, you can install it using:


## Getting Started

1. Replace `YOUR_ACCESS_KEY` and `YOUR_SECRET_KEY` in the script with your actual AWS access key and secret key. These are necessary to authenticate with AWS services.

2. Customize the date range in the `TimePeriod` dictionary within the `get_billing_details` function to fetch billing details for the desired period.

## Usage

To run the script:
1. Save the script to a local file (e.g., `billing_details.py`).
2. Open a terminal or command prompt and navigate to the directory where the script is saved.
3. Execute the script using the following command:
4. The script will use the provided AWS credentials to fetch the billing details for the specified date range.

## Important Note

- Ensure that the AWS IAM user associated with the provided access key and secret key has appropriate permissions to access AWS Cost Explorer (ce:GetCostAndUsage) and S3 (s3:GetBucketAcl).

## License

This project is licensed under the [MIT License](LICENSE).
