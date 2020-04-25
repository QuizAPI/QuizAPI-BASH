# QuizAPI-BASH
This is a BASH wrapper for the quizapi.io API

![QuizAPI Demo](https://dev-to-uploads.s3.amazonaws.com/i/ckb8sug0y9rs4ha6toeb.gif)

## Prerequisites

* An API Key for the Quiz API, you can get it totally for **free for developers** (here)[https://quizapi.io/register]

* jq installed, if you try to run the script without having `jq` installed you will get the following message:

```
The jq command is required! Please install it and then try again
```

## Installation

Download the script:

```
https://raw.githubusercontent.com/QuizApi/QuizAPI-BASH/master/quiz.sh
```

Make the script executable:

```command
chmod +x quiz.sh
```

Set your **QuizAPI** key as an env variable:

```command
export API_KEY=your_api_key_here
```

## Usage

To run the script just run the following:

```
./quiz.sh -a ${API_KEY}
```

You will get to an interactive quiz menu where you can select multiple answers.

The output will look like this:

```
There is only 1 correct answer!

"Following Docker command: docker commit -m \"My first update\" container_ID user_name/repository_name  is used to:"
  1 ) "Activate default VM machine"
  2+) "Commit changes done in a Docker image"
  3 ) "Build an image"
  4 ) "Access a running container"
"Commit changes done in a Docker image" was checked
Check an option (again to uncheck, ENTER when done):

Selected was:  "Commit changes done in a Docker image"
Correct: is:  "Commit changes done in a Docker image"
Correct Answer
```

## Arguments

The script accepts the following arguments:

```
quiz.sh -a API_KEY [-c Category] [-d Difficulty] [-t Tags]
```

* `-c` - get questions only for a specific category
* `-d` - get questions only for a specific difficulty (Easy, Medium and Hard)
* `-t` - get questions for a specific topic/tag, this lets you combine multiple topics

## Documentation

For more information, checout the official **QuizAPI Documentation** here:

(QuizAPI Documentation)[http://quizapi.bobbyiliev.com/docs/1.0/overview]
