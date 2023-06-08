# Use AI in DevOps

## Create ChatGPT account

- go to https://chat.openai.com/auth/login
- Login if you have an account or sign up or a new account using your google account


## Create content using prompts

- Provide me ideas for a sample web application that I can use in my CI/CD project
>> some ideas will be listed..

- Continue with the same prompt and ask: 
regenerate a simple application for beginners

- Make the liste wider so ask:
generate 5 more ideas for a beginner

- Now make the prompt finer to ask:
generate the python code for simple calculator application
>> python code is generated for the application

- the program works on command line, but we need it on the web. enter the prompts to ask to convert this to a web application
>> convert this application to a web application

- change the code to fit for mobile devices.
>> make this web application responsive to mobile devices

- ask AI to Dockerize the application
>> Dockerize the application

- There's the requirements file used in the Dockerfile. let's find out the contents of the requirements.txt file.
>> What are the contents of requirements.txt file

- Now let's automate deployment
>> generate a sample Jenkins CI/CD pipeline for the .... application

- if code is not generated refine the prompt to generate the pipeline code ..

- you may have noticed that we ask follow up questions but we do not refer to the context, it assumes that way, understands it

- now lets convert this pipeline so that we can use in Kubernetes
>> convert this pipeline to Kubernetes manifest

- try the pipeline code again
>> regenerate the pipeline code for this Kubernetes


- It is now time to provision Infrastructure (by default aws is selected)
>> generate Terraform files to provision the infrastructure to host this application

- ask to use variables in file 
>> generate variables file and use variables in main.tf

- now the most boring but a very vital part to produce, the documentation
>> generate a readme file for the Jenkins pipeline, application code and terraform.

====
**Other Use Cases**

## Use AI for a Blog

ask the AI about
- best practices of ansible

then ask to 
- write a technical blog using the above details


## Describe a Topic

ask to describe a topic
- Explain me Docker as if I am 10


## Write a Resume/CV or a Cover Letter

- include some requirements of a job description and then ask to 
>> write a cover letter for the described job

- you can refine it 
>> rewrite in less than 500 words and use bullet points

## Understand/explain some piece of code

- explain below code

```js
// Importing the built-in 'readline' module for user input
const readline = require('readline');

// Creating an interface for user input/output
const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout
});

// Function to generate a random number between min and max
function generateRandomNumber(min, max) {
  return Math.floor(Math.random() * (max - min + 1)) + min;
}

// Prompting the user to enter the minimum and maximum values
rl.question('Enter the minimum value: ', (minValue) => {
  rl.question('Enter the maximum value: ', (maxValue) => {
    // Parsing the input values as integers
    const min = parseInt(minValue);
    const max = parseInt(maxValue);

    // Checking if the input values are valid
    if (isNaN(min) || isNaN(max) || min >= max) {
      console.log('Invalid input. Please enter valid minimum and maximum values.');
      rl.close();
    } else {
      // Generating a random number and displaying the result
      const randomNumber = generateRandomNumber(min, max);
      console.log(`Random number between ${min} and ${max}: ${randomNumber}`);
      rl.close();
    }
  });
});
```



## Understand logs

- explain below logs
2023-06-07 09:15:23 [INFO] Server started on port 8080.
2023-06-07 09:17:45 [DEBUG] Received GET request for /api/users.
2023-06-07 09:17:45 [INFO] Executing query to retrieve user data from the database.
2023-06-07 09:17:46 [DEBUG] Query executed successfully. Returned 25 users.
2023-06-07 09:17:46 [INFO] Sending response with user data to client.
2023-06-07 09:18:02 [DEBUG] Received POST request for /api/users.
2023-06-07 09:18:02 [INFO] Validating user input.
2023-06-07 09:18:02 [WARNING] Invalid email format in the request body.
2023-06-07 09:18:02 [INFO] Sending 400 Bad Request response to client.
2023-06-07 09:18:15 [DEBUG] Received GET request for /api/posts.
2023-06-07 09:18:15 [INFO] Exec



## Automate tasks

- create a bash script to take mysql database backup daily and save it on s3
