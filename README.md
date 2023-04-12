# Lambda-function-

DIY Activitiy for Serveless Function on Cloud Quest. 
Serverless Foundation 

Modify the lab's AWS Lamda function code to display differnt feeling values based on the emoji_type value in the JSON element. 

![image](https://user-images.githubusercontent.com/55962550/231575864-1d80aedc-ad4d-49ff-8e79-a349964bce32.png)


Validation Process 
Our test servers will transmit a JSON object to your Lambda function containing the emoji_type identification element and a random message. Example:
{
"emoji_type": 0,
"message": "I love the park"
}

Update the lambda function using the following rules:

 emoji_type = 0, returns feeling: "positive"
 emoji_type = 1, returns feeling: "neutral"
 emoji_type = any other value than 0 and 1, returns feeling: "negative"
  
After the above updates, your Lambda function must return the interpreted sentiment in the following JSON format (just like it already does):
{
	"feeling": "positive",
	"message": "I love the park"
}
The validation code will look for a similar output as displayed above.  Any extra characters in the output will fail the validation.
 
 Hints:
 Based on the sample code provided (the sample_code.py file you downloaded eariler): 
 - Update the if-else block to add a variable for the feeling attribute (positive, neutral, negative).
 - Change the response section of the code to add the feeling attribute instead of custom_message.
 - Look at step 11 from earlier if needed.
