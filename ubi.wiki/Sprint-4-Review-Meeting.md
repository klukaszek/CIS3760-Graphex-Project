*Fri. March 17/23*  11:30-12:15
- **Review completed user stories**
  - Sentiment Analysis:
    - Go thorough the twitter posts and view the sentiment analysis
  - About Page:
    - As a viewer I want to view information about the website. The about page displays      information about UBI and contains team member information
  - Q&A Page powered by OpenAI:
    - Only answers question related to UBI
  - For each twitter post, there is a link to the post on twitter's website
  - All Page:
    - Loads all twitter posts that are contained in the database. Judi asked if we are planning on using sentiment analysis for the entire database. Yes we will be doing so.

- **Open and view User Story (About Page)**
  -  Turn the definition of done and acceptance criteria into a checklist. It will make it easier for us to keep track. We can tick off each individual task. 
  - Make a template for issues, we can write a template so that every issue we make fills up with a pre-generated template.

- **Testing**
  - **Backend**
    - We have both unit and integration test. We use an in memory database for testing using MongoMock.
    - Integration testing for reddit, twitter, and plots
    - We have unit tests for database connectivity
    - We can create a connection class that runs off an environment variable, that creates pretend backend, and a pretend database that can be used for testing. This is what we have done.
  - **Frontend**
    - Two sets of tests working for showposts page. When trying to test showplot, we get importing errors through the testing harness. npm issues.
    - When using node frontend. Jest can create a mock for the backend, but this might be a react only feature
    - Any plans for UI testing? We can grab components through vitetest and check the screen for specific text. If the text exists in the DOM then it passes the test. Automated UI testing is painful, try using human readable scripts to go through UI testing. 

- **Environment Variables**
  - For docker compose you only need the port. For Kubernetes it adds its own uri, as it runs in separate containers. It can’t resolve to localhost since it has its own uri. 

- **Code Review Process**
  - When someone is merging code, the person who answers the merge request goes through the checklist that is available in our wiki.
  - Are we doing merge review process through calls? No, we are in contact through slack and ask questions/comments through slack

- **Commit Conventions**
  - Do we have commit conventions? Yes, we have proper commit messages, with documentation for feat, chore, fix, style, etc.

  - Go through merge request code review Iss75-86  nltk sentiment analysis:
    - Feedback: Nice commit messages, compare old and new commit message conventions. 


- **Refactoring**
  - Wrappers around the api. If reddit changes the api for accessing it, how many files would we have to change? We only have to change one file. We previously had api call to twitter in different files, but we refactored so that twitter wrapper api is only 
Wiki Page
  - Look through our meeting minutes, coding conventions, sprint contribution reports, wrapper api documentation

Did we setup a sprint 4 goal? Yes, it is in our sprint 4 sprint planning meeting. Originally, we planned on creating a term-frequency histogram. But we made a sentiment analysis plot instead.

- **Feedback**
  - **Next Sprint** 
    - Staging server
    - Visualization that overlays that two data sources in some way
    - Two new user stories
    - Tidy it up refactor




