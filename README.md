# Polly-Powered-Audio-Narrator
Text to Audio Converter

<a href="https://viewer.diagrams.net/?tags=%7B%7D&lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1&title=TextToSpeech&dark=0#Uhttps%3A%2F%2Fdrive.google.com%2Fuc%3Fid%3D1elLvNFNEUweHbse9Ay57DAEZIalIS4Jb%26export%3Ddownload">Design</a>

This project leverages AWS services to convert text files into audio files. This is useful for creating audio versions of written content, making it accessible to a wider audience, including those who prefer listening over reading.

Stage 1: Created two S3 Buckets( Source Bucket and Destination Bucket)

Stage 2: Created an IAM policy for Lambda
![Image](https://github.com/user-attachments/assets/94ca66b1-2bea-4dc9-8a7d-f3f7589483ba)

The policy gives read/write access to both the source and destination bucket. The policy gives read access to all resources. 

Stage 3: Created an IAM Role and attach amc-polly-lambda-policy and AWSLambdaBasicExecutionRole Policies

Stage 4: Created and Configured the Lambda Function

Stage 5: Configure S3 Event Notification

Stage 6:Lambda Code
