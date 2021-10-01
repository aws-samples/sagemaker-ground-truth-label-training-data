# Easily label training data for machine learning at scale (AIM-406) 
### Summary 
In this session you will learn how to create high-quality labels while also reducing your data labeling costs by up to 70 percent. This session walks through the different workflow options in Amazon SageMaker Ground Truth, such as automatic labeling and assistive labeling features like auto segmentation and Image label verification. We will walk you through how to build highly accurate training dataset for company brand/logo so you can build a ML model for company brand protection.

Table of Content 
<TODO>

Problem Definition
<TODO> 

Setup Env
<TBD EE or awslabs>


Workshop


### Step 0 : Login to event engine.
## AWS Instructor-Led lab
Go to: https://dashboard.eventengine.run/login. You will be redirected to the page
below
![Access Eventengine Dashboard](images/5_1.png)
Enter the event hash you have received from your instructor
![Enter the event hash](images/5_2.png)
Click on Email One-Time Password (OTP)
![Email One-Time Password](images/5_3.png)
You are redirected to the following page:
![](images/5_4.png)
Enter your email address and click on Send passcode
![Enter your email](images/5_5.png)
You are redirected to the following page
![Enter passcode](images/5_6.png)
Check your mailbox, copy-paste the one-time password and click on Sign in.
![Sign in](images/5_7.png)
You are redirected to the Team Dashboard. Click on AWS Console.
![Team Dashboard](images/5_8.png)
Click “Open AWS Console”
![Open AWS Console](images/5_9.png)

### Step 1 : Create Sagemaker Ground Truth Workforce

Amazon SageMaker Ground Truth gives you access to different workforce options:
* Amazon Mechanical Turk – You get access to an on-demand, 24/7 workforce of over 500,000 independent contractors worldwide. This option is recommended for non-sensitive data.
* Private – You can setup up access for a team of your own employees or contractors. This option is recommended for sensitive data or when domain expertise is required for the labeling job.
* Vendor managed – You can get access to a list of third-party vendors approved by Amazon, who specialize in providing data labeling services, available through AWS Marketplace.

For this tutorial, we use `Private` workforce with you as the labeling member to label our dataset label a dataset with images of brand logos. Let's get started.

1. Navigate to the Amazon SageMaker console by clicking typing SageMaker at the search bar as seen below. 

![Naviagte to Amazon SageMaker](./images/1_1.png)

2. Select the Ground Truth on the left pane.

![Click Ground Truth](./images/1_2.png)

3. Select Labeling Workforces.

![Click on Labeling Workforces](./images/1_3.png)

4. Select the tab that reads private and select 'Create Private Team'

![Click on Create Private Team](./images/1_4.png)

5. Select 'Create Private Team with AWS Cognito'. Enter details for 'Team Details' and 'Email Addresses' sections. Ensure that you have access to the email address you provide.

![Enter details to Create Private Team](./images/1_5.png)

6. Review the Summary

![Summary](./images/1_6.png)


### Step 2 : Navigate to the SageMaker Studio
Navigate to AWS Console and using service locator search for Sagemaker Studio.
Next, Click on Create Sagemaker Studio.
You should already see a user - "sagemakeruser" created for you.
Once you select this user, you will be directed to Launcher screen.
Within Notebook and Compute Resources section, select a python 3 Notebook as show below.
![Navigate to Sagemaker Studio](./images/4_1.png)

### Step 3 : Download the notebook code
TODO

### Step 4 : Upload images using notebook
TODO

### Step 5 : Create Labelling job using notebook
TODO

Verify from the UI : Labelling job is created.












1. Using Service Locator, search for S3.

![Locate S3](./images/2_1.png)

2. Create a bucket.

![Create a bucket](images/2_2.png)

3. Give the bucket a unique name and ensure that it is in the same region where the Ground Truth was created. 

![Assign a unique name to the bucket](images/2_3.png)

4. Select option to 'Upload'.

![Select option - Upload](images/2_4.png)

5. Select option to 'Add Folder'.

![Select option - Add Folder](images/2_5.png)

6. Review summary to ensure all images have been uploaded. Select 'Upload' at the bottom of the screen.

![Select Option - Upload Images](images/2_6.png)

### Step 3 : Create the Amazon SageMaker Ground Truth labeling job.








1. Create Sagemaker Ground Truth private workforce.
2. Upload images file which needs to be labeled to S3 for company brand detection use case, this is more on object detection use case. (We will pre-populate this files, to event engine account so that customers do not want to download the re-upload to s3)
3. Create the Amazon SageMaker Ground Truth labeling job.


4. Involve in the data labelling process as a worker.
5. Review labeling job results.
6. Enrich the labelling job with automatic labelling and reduce the cost.
7. Future Extensions (Example blogs, references etc)

Test
