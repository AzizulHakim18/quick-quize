# Getting Started with Create React App

Getting started
The first thing I did was find a good API resource for the questions. After a bit of Googling I found Open Trivia Database, which has thousands of questions and is moderated. If you take a look at the API config you can see that there are all the parameters you need to create a quiz platform: number of questions, category, difficulty, type & encoding options.

Using create-react-app, I set up using the default options, opting not to add redux initially (this is something that I reassess later). Start by running these commands in your terminal:
We import useEffect and useState from react, then we can declare a state variable for the options with an initial null value. This is where we will store the data from the API response using setOptions.
The final thing to consider before adding the JSX for the Question component is that we want an “unanswered” an “answered” state. Before the user has selected an answer, the main pieces of information that we need to show are the question and the answer options. When the user has made their selection, we should show whether they have selected the correct answer, and, if they haven’t, show them what the correct answer was.
