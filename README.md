# Amazon-Rekognition - BUILDING AN IMAGE LABELS GENERATOR USING AMAZON REKOGNITION.

ABOUT AMZON REKOGNITION: 

Amazon Rekognition is a cloud-based computer vision platform that provides image and video analysis capabilities. It uses deep learning technology to detect objects, scenes, faces, and text in images and videos. 

Some key features of Amazon Rekognition include: 

1. Object and scene detection: Identifies objects, scenes, activities, landmarks, and dominant colors in images.

2. Facial analysis and recognition: Detects faces, analyzes facial attributes like emotions and facial hair, and enables face-based user verification.

3. Text detection: Extracts text from images and videos of signs, social media posts, product packaging, etc.

4. Custom labels: Allows training models to detect custom objects and scenes specific to a business using as few as 10 images

Amazon Rekognition includes a simple, easy-to-use API that can quickly analyze any image or video file that’s stored in Amazon S3.

Some notable use cases include detecting inappropriate content, verifying identities online, streamlining media analysis, and sending smart home alerts.

PROJECT OVERVIEW: 

The summary of this project is to process raw images downloaded from the internet and label them using Amazon Rekognition.

1. The images of a bustling city were downloaded from a website whose link will be provided down below.

2. Create an IAM user with permissions to access AWS S3 and Amazon Rekognition.

3. Create an S3 bucket and move the downloaded images into it.

4. Install the AWS CLI and install required Python libraries including Boto3 to facilitate AWS interaction and Matplotlib for visualization, using pip.

5. Use Boto3 to connect to your S3 bucket and list the images stored there. For each image, call the Rekognition service to find and label objects within the image.

6. Collect the positions (bounding boxes) of these objects along with their labels.

7. Read the image directly from S3 without saving it locally. Use Matplotlib to display the image with bounding boxes around detected objects.

8. Position the labels below the bounding boxes to make them easy to read.

9. Execute your Python script to see the images with labelled objects and bounding boxes.

CHALLENGES ENCOUNTERED: 

I encountered a minor issue after generating the analyzed images. The text boxes were stacked on top of each other making it slightly difficult to read.

However, after a few tweaks in the code, it was quickly rectified and the text boxes were adequately spaced out.

AWS RESOURCES UTILIZED: 

IAM - I wrote a JSON script to create the permissions required to ensure the access Rekognition needed to interact with S3, and attached it to an IAM user.
AWS S3 - Created an S3 bucket to contain the images that were to be processed by Rekognition.
Amazon Rekognition - Used Rekognition to analyze and label the individual components of the images.

TECHNOLOGIES EMPLOYED: 

AI tools came in very handy in the course of this project, specifically Perplexity and ChatGPT . 

I also resorted to YouTube to study the entirety of Amazon Rekognition.

LINKS:

1. Image Source: https://unsplash.com/s/photos/busy-city

2. ChatGPT: https://chatgpt.com/share/853ae3ae-75ed-476f-81dc-3227e2e21871

3. Perplexity AI: https://www.perplexity.ai/search/write-python-code-that-uses-de-E97WmmgVThecx91PhRm7mw

4. YouTube: https://www.youtube.com/watch?v=3PGPfs-ARdo&ab_channel=BeABetterDev

