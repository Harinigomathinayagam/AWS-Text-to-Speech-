# AWS-Text-to-Speech-
This project demonstrates the power of serverless computing and AI-driven voice synthesis using AWS Cloud services.
We can build Text to Speech solution using AWS Serverless services like AWS Lambda, Amazon Polly and Amazon S3.
#Steps 
#Step-1:
  Create an S3 bucket — A place in S3 to store audio files
#step-2:
  Create the Lambda function — Using AWS Lambda console:choose runtime , link the IAM role, and write code that will do the conversion (text → speech) and store results.
#step-3:
  Define IAM role — Set up a role that gives your Lambda function rights to read from S3,write to S3, and use other AWS services securely.
#step-4:
  expose an API — Use something like an API call (maybe via Postman) to send text input, trigger Lambda, and retrieve resulting audio.
#step-5:
  Invoke AWS Polly inside Lambda — Within the Lambda code, pass the input text to Polly service, Polly generates audio from the text.
#step-6:
  Save the generated audio to S3 — Once Polly returns the audio, Lambda uploads/stores that audio file into the S3 bucket.
#Conclusion:
  Use S3 + Lambda + Polly as serverless workflow — This combination lets you convert text to speech on demand, store results, all without managing servers
