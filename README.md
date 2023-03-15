# Coding Challenge

Hey there, thanks for taking the time. To get to know you and your working style a little bit better, we have prepared a take-home coding challenge for you covering some parts of our daily work. You will be guided through the process by following the tasks below.

### Setup

1. Please visit XXXX and clone the repository to your local machine.
2. You will find a starter Django project containing a single app (keywords) and all the traditional Django files and folders. 
3. Set up a virtual environment and install the required dependencies. 
4. Run the development server to check everything runs as expected.

<aside>
💡 If you experience some problems during the setup or your tasks, feel free to shoot an e-mail to developer@syntinels.com

</aside>

### Tasks

1. Take a look at the `job_postings.csv` file provided at the root of the project. This is a random excerpt from our job posting database. It contains a reference to the company, as well as the title, link, content, and some additional metadata.
2. Please design an appropriate data model using the Django ORM in the `models.py` of the `keywords` app. Migrate your database (you should be able to use the basic one) and upload the data in your database.
3. The goal of this project is to derive keywords from job postings. The keywords are e.g. a list of skills like `Python, Git, Web Development, Tailwind, Docker`, or `Javascript.` The user should be able to modify this list once in a while (out of scope for this project) and we want to identify the keywords in the job postings and display them. Job postings may have multiple keywords. Extend the database models you have designed in ******2.****** to cover these needs.
4. Next, design a background script that has access to the keyword list and looks for them within the job postings (.csv or database, if you uploaded them). Feel free to do some research or to start right away, if you have a viable solution. How efficient is your implementation? Does it scale well with millions of job postings? What happens if the list of keywords is changed? What implications does that have on your data model? Be prepared to answer questions like these.
5. Execute the script so that your results are persisted somehow.
6. At Syntinels, we believe in test-driven development. In this case, we did not start with the tests, but how would you test your code so far? You don’t have to write something down, but it would be great to hear about your suggestions.
7. What approach and tools would you choose to automate the process of finding keywords in the job postings?
8. Now, that we have job postings matched with keywords, please visualize the results in the front end. It does not have to be fancy, you can use basic HTML if you want to. Just display the results somehow so that the user can see what keywords were identified for each job posting.
