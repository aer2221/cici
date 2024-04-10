# CiCi: Columbia CS Advising Chatbot
### CS classes are hard. CS advising shouldn’t be. Get answers to all your Columbia computer science questions from CiCi!

Note: this project is an extension of a hackathon project I began with Kylie Berg, Charles Liu, and Eris Gao. Please feel free to check out this [original repository](https://github.com/kynsity/DivHacks2023_project) for an idea of what that project looked like.

## Inspiration
One of the hardest parts of being a CS major at Columbia is not the classes: it’s advising. The current system is overwhelming and unsustainable for CS advisors and students alike; students often wait hours to meet with advisors who often cannot properly answer their questions, and this reality motivated me to improve and extend CiCi.

## What CiCi does

CiCi is an AI chatbot trained on Columbia CS advising data. It uses this history along with its broader chatbot capability to answer any questions you have about the CS major, coursework, or career options at Columbia. Generally, CiCi is better at answering broader questions about the major, such as questions that a first- or second-year CS student may have. Unless you provide it extensive proper context, CiCi is not as well equipped to answer specfic questions about your experience in the major (i.e. am I on track to graduate, etc.).

*For a lovely pitch video that encapsulates all that CiCi does, including a demo, in 2 minutes, click [here!](https://youtu.be/Ww39W1hPjcs)*

## How CiCi was built

Backend: Created embeddings using Columbia CS Advising documents and stored them in a vector database. Then, use the OpenAI API to make a chatbot that answers CS advising questions by searching through the vector database for the most relevant text and compiling them into a single concise answer.

Frontend: HTML/CSS/JavaScript

## How I improved CiCi from the original hackathon version
- backend improvements: upgrading to GPT-4, prompt engineering, adding additional Columbia CS documentation to better train CiCi
- frontend improvements: bug fixes (text going outside the page, items shifting once text appears, etc), adding sample questions for users to test, making UI more intuitive and responsive
- I also, through my own user research and testing, discovered what I believe is best use case for CiCi, which as I mentioned earlier is answering broader questions about the CS major at Columbia that tend to come from underclassmen, prospective students, and those who are new to the CS program. 
  
## How to use CiCi
NOTE: To use CiCi you need to have access to an OpenAI API key and an Active Loop Deep Lake API key. Please add these within the code yourself. 
Type "flask run" in your terminal and navigate to local host to use CiCi. 
