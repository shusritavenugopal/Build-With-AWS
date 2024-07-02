# Build With AWS - [PartyRock Hackathon Project Link](https://community.aws/content/2etY00T8tlf3NHsQxnDSSjmXjHH/exploring-partyrock-app-development-with-amazon-bedrock)

![883BDA7E-67B8-42CC-A353-94699285F166-JPG](https://github.com/shusritavenugopal/Build-With-AWS/assets/63789652/73c8a3c9-4ee5-4bf0-a399-6796ebf376cf)

With over 200 AWS services available, finding the right services can be tough. Build With AWS promotes AWS cloud by analyzing your project requirements and recommending the most suitable AWS services.

[Project Featured on AWS Vice President & Chief Evangelist LinkedIn](https://www.linkedin.com/posts/jeffbarr_aws-activity-7184227585332068353-Ni01?utm_source=share&utm_medium=member_desktop)

[Project Featured on AWS Q VP LinkedIn](https://www.linkedin.com/posts/themza_exploring-partyrock-app-development-with-activity-7183927823793840128-bpKt?utm_source=share&utm_medium=member_desktop)

[PartyRock App](https://community.aws/content/2etY00T8tlf3NHsQxnDSSjmXjHH/exploring-partyrock-app-development-with-amazon-bedrock)

[AWS Community Blog - Coding perspective of PartyRock App](https://community.aws/content/2etY00T8tlf3NHsQxnDSSjmXjHH)

[AWS Community Blog - Build With AWS](https://community.aws/content/2dUK1A3E8iaozHjSP41yLyu4pYi/build-with-aws)

[Snapshot of PartyRock App Usage](https://partyrock.aws/u/shusrita/MJ-8wHfGU/Build-With-AWS/snapshot/er3462ONM)

# Inspiration
The inspiration behind building this project stemmed from recognizing that the most effective way to learn cloud computing is through hands-on projects. Many aspiring cloud users may have projects but haven't yet implemented them on the cloud. This app aims to bridge that gap by promoting the use of cloud services and products offered by AWS.

# What it does
The Build with AWS app serves as a comprehensive guide for navigating the vast array of services offered by Amazon Web Services (AWS). With over 200 fully featured services available globally, AWS is the leading cloud provider, but selecting the right services for a project can be overwhelming.

To address this challenge, the app allows users to input details about their project, including descriptions, libraries, and algorithms they plan to use. Using this information, the app analyzes the project's requirements and objectives. It then generates a curated list of AWS services and products that best align with the project's needs.

The app offers step-by-step guidance on how to integrate these recommended AWS services into the project. This includes instructions on setup, configuration, and usage, making it easier for users to implement AWS solutions effectively.

Additionally, the app provides useful AWS blogs and resources to help you build the project. The app also features a built-in chatbot that serves as virtual AWS support. Users can ask questions and seek assistance regarding AWS services and configurations in real-time.

## Getting started

### Choose a notebook environment on AWS

- For a fully-managed environment with rich AI/ML features, used [SageMaker Studio](https://aws.amazon.com/sagemaker/studio/).

### Enable AWS IAM permissions for Bedrock

The AWS identity you assume from your notebook environment (which is the [*Studio/notebook Execution Role*](https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-roles.html) from SageMaker, or could be a role or IAM User for self-managed notebooks), must have sufficient [AWS IAM permissions](https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html) to call the Amazon Bedrock service.

### Configure IAM Policy for Amazon Bedrock Access

This notebook requires an IAM role that has access to Amazon Bedrock. Below is an example IAM policy that grants access to Bedrock APIs:

### Example IAM Policy

```json
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "Statement1",
            "Effect": "Allow",
            "Action": "bedrock:*",
            "Resource": "*"
        }
    ]
}
```

### AWS Configuration for Amazon Bedrock

To work with Amazon Bedrock, I used the following AWS configurations:

#### AWS Account and Region
- **AWS Account**: Used my AWS Account
- **Region**: `us-west-2` (Oregon)

#### SageMaker Studio Setup
- **SageMaker Studio Account**: Utilized my SageMaker Studio Account

#### Kernel Configuration
- **Image**: Data Science 3.0 (or greater)
- **Instance Type**: `ml.t3.medium`

### Instructions

1. **Access the Amazon Bedrock Console**
   - Open the Amazon Bedrock console.

2. **Navigate to Model Access**
   - In the left menu, go to **Model access**.
   - Select **Manage model access**.

3. **Request Access to Models**
   - On the **Manage model access** page, request access to the following models:
     1. **Amazon - Titan Embeddings G1 - Text**
     2. **Anthropic - Claude**

4. **Confirm Access**
   - Wait for approval and confirmation of access to the requested models.





