# AI LLM Prompts


## To check email reply if ok
Set temp: 0
```
For the following email to my colleagues, please ensure that the tone is formal and profe
ssional. Ensure that the spelling and grammar are correct, and that the flow of the email is good.
Please use British English for the response.
```

## To summarise long meeting notes
Set temp: 0
```
I will provide you with the Original Text of some shortform notes taken of a work meeting with my colleagues.
As the Original Text is very long, I will be providing the Original Text in parts.
Begin by asking me for the first part of the Original Text.
Once I have given you the first part, ask me for the second part of the Original Text, the third part of the Original Text, so on and so forth.
Only after I inform you "End of Original Text", then you will reply to summarise all the parts of the given Original Text, in the Style specified, with the Audience in mind. Adhere to the requirements given under Response. 

Style: Formal for work purposes
Audience: For my colleagues and bosses
Response: 3 paragraphs, in British English

Take a deep breath, and let me know if you understand my requirements. If you understand my requirements, tell me "let's go" and I will begin to provide the Original Text.
```

## To generate proposed replies
Set temp: 0.5
```
I had sent the following email to my colleague:
"xxx"

My colleague has responded with the following email reply:
"xxx "

Based on my previous email to my colleague and my colleague's email reply, I would like to respond to my colleague's reply with an email consisting of the following points:
-
-
-

Please provide a draft email reply using the above points.  Ensure that the spelling and grammar are correct, and that the flow of the email is good. Please use British English for the response.
```

## To provide counselling chat
Set temp: 1.0
```
Imagine you are a Counsellor. Role-play with me and ask me questions and provide replies to simulate a counselling session for stress management.

When I say "Stop", you will immediately end the role-play and give me a detailed assessment of the conversation, and highlight areas of improvement I need to take note of.

When you are ready, say "Hi, how can I help you today?" and start your first question.
```


## COSTAR PROMPT
Set temp: 0.5
```
Context: <specify the background of your prompt, e.g. This is an email to my colleague who has helped me greatly at work>

Objective: <specify the task you want the AI to perform, e.g. write a poem about … | write an email to …>

Style: <specify the style you want the AI to use to write the response, e.g. humorous | casual>

Audience: <specify the people whom the response is intended for, e.g. my colleague | my family | my CEO>

Response: <specify the length of the response you want, e.g. short | long | 3 paragraphs | 200 words | in a tabular format | in a report format>

Do the Objective above based on the Context, in the Style specified, with the Audience in mind. Adhere to the requirements given under Response.
```



## Roleplay
Set temp: 0.5
```
Imagine you are a <specify the role of the AI, e.g. Career Coach | Counsellor>. Role-play with me and ask me up to <specify the number of questions you want to answer, e.g. 5> questions to <specify the purpose of the roleplay, e.g. simulate a job interview for a Personal Assistant job>

When I say "Stop", you will immediately end the role-play and give me a detailed assessment of my replies, rate me from 1 to 10 with 10 being the best, and highlight areas of improvement I need to take note of.

When you are ready, say "Begin" and start your first question.
```




## Summarise
Set temp: 0
```
Original Text : '''
<insert your text here>
'''

Style: <specify the style you want the AI to use to write the response, e.g. humorous | casual>

Audience: <specify the people whom the response is intended for, e.g. my colleague | my family | my CEO>

Response: <specify the length of the response you want, e.g. short | long | 3 paragraphs | 200 words>

Summarise the above Original Text denoted within the triple quotes, in the Style specified, with the Audience in mind. Adhere to the requirements given under Response.
```

## Correct
Set temp: 0
```
Original Text : '''
<insert your text here>
'''

Correct for errors (typos, grammatical and spelling mistakes) in the Original Text denoted within the triple quotes.

Then, provide a list of the changes as well as a rating of the Original Text from 1 to 10, with 1 being that it is full of errors and 10 being perfect.
```

## Brainstorm
Temp: 1
```
I am thinking of a problem, which is <specify the complex problem you are currently facing, e.g. how to explain the difficult concept of AI to a 6 year old>. Analyse the problem from multiple angles, and think through step-by-step what is the best approach to the problem.

Explain the thought process in detail before coming to your conclusion.
```

## Suggest
Temp: 0.5
```
Help to write a good prompt that when used with a Large Language Model, the AI will help me with <specify the task you want to complete, e.g. writing an email to my colleague to congratulate him>. Do not provide the prompt immediately, but instead ask me a series of up to <specify the number of questions you want the AI to clarify first before giving you the prompt e.g. 5> clarifying questions one at a time. Each time, wait for my response to help you better formulate the prompt.

If I say "Stop", immediately output the best prompt that you have at that point in time.
If I say "Execute", use the latest prompt you have and execute that prompt.
If ready, say "Let's begin" and start with your first clarifying question.
```


## Classify
Temp: 0
```
Category A : <specify what the contents in category A are like, e.g. Positive comments>

Category B : <specify what the contents in category A are like, e.g. Negative comments>

<add more categories if you need, e.g. Category C : Negative comments>

Original List : '''
<insert your list of data here, e.g. lines of feedback data>
'''

Classify the above Original List denoted within the triple quotes into the respective Categories A, B, etc. Look through the output step-by-step and make sure the counting is accurate.

For example, if there are 8 feedback, output as below:

Category A (3)
- Food is good
- Tastes good!
- Excellent service

Category B (2)
- Food is bad
- Terrible.

Category C (3)
- No comments
- Nil
- NA
```

