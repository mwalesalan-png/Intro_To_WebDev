#COMPLETE LESSON PLAN

##1. Lesson Information

**Course:** Introduction to Website Development

**Duration:** 60 Minutes

**Target Audience:** Begginers

**Teaching Method:** Demonstration and Practical Learning

**Instructor:** Mwale Allan

##2. Lesson Description

This lesson introduces learners to the fundamentals of Website development. 

Learners will understand what websites are, how to make an API call, how to read requests and identify the basic technologies used to build websites and create their first simple webpage.
Have you wondered how Websites are created and how they work.

## 3. Learning Objectives

By the end of this lesson, learners should ba able to:

1.Explain what website development is.
2.Make first APi request
3.Learned on how to handle Errors.
4.Create a basic HTML webpage.
5.Opened and view a webpage in a browser.

## 4. Teaching and Learning Materials
The following materials will be required:

1. Computer
2. Visual Studio Code for writing HTML code.
3. Internet connection
4. Lesson Handout and practical sheets.

## 5. Teaching Plan
### Time             Teaching Activity
0-5 min              Introduction and opening question
5-10 min             Explain website Development
10-20 min            Introduce HTML, JSON, CSS and JavaScript
20-30 min            Demonstrate creating a weather HTML page
30-45 min            Learners create their own webpage
45-50 min            Learners present their work
55-60                Assesment and lesson recap

## 6. Concept:
Website development is the process of creating and mintaining websites thatb people acess through the internet.
The main technologies:
   A. HTML - Structure: Provides the structure and contect of a webpage, such as headings, paragraphs and images.
   B. CSS - Design: Controls the appearance of a webpage, including colours, fonts, spacing and layout.
   C. JavaScript: Makes webpages interactive for example when someone clicks a button.
   D. API: Application Programming Interface. This is how your code talks to other services, other databases and other systems. Today you learn what they are and make your first API request.

## 7. How APi Call works
1. You send a Request: Your code sends an HTTP request to a URL. The URL is the adress of the API. Like visiting a website but instead of a browser making the request your python code does.
2. The API processes it: The server receives your request checks if you are allowed to make it run whatever logic it needs to and prepares a response.
3. You receive a Response: The API sends data, usually in JSON format. Json is astructured way to send data that both humans and computers can read. you parse and use what you need.

HTTP has different request types. The most common ones you will use are Get(fetch) and POST(send data). Today we use GET.


## Instructions for learners:
Installing the requests Library: Python can make HTTP request using a library called (requests). You install it once with pip
Open your terminal in VS code run:
(pip install requests)

##First API call
We will use REST countries API. It is free, needs no sign_up and returns live data about every country in the world.
Open Vs Code write day1_api.py type this exactly:

import requests
url = "https://restcountries.com/v3.1/name/kenya"
response = requests.get(url)

print("Status code:", response.status_code)
print("Data received:", response.json[])


status of 200 means Ok
status of 404 means not found
401 means not authorized
429 means too many requests
500 means something broke on the server side.

How do you know you got it? -"Learners runs code and output matches expected result."

## 8. Questions
1. Why does my funcion return none?
"You have no return statement Add return result on the last line of the fuction."
2. What is the difference between print and return?
Print shows it on screen return sendsthe value back to wherever the fuction was called, "use return when you need to use the value later"
Can I call a fuction inside another function?
"Yes. That is exactly how good code is built. Try it."