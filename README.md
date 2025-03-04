# site
This README is geared towards people who want to build a similar website with at least a basic knowledge of Markdown and basic understanding of the command line such as changing directories and runing commands.

## getting started
### Prerequisites.
* A GitHub account.
* An editor.
* Pelican downloded.
* Knowledge of Markdown.
* Basic knowledge of Git.

At the *Further Resources/Readings* there is tutorials to help with getting the prerequisite knowledge.

### Instructions.  
#### Setup
1. Setup a pelican project using 
        
        pelican-quickstart
    in the terminal
2. When it asks you to pick a URL prefix do something like this: 

        https://username.github.io/example
    where:
    * Username is the GitHub username
    * Example is the repository name

2. Create a Markdown file in the content folder that is automatically created when you create a pelican project  
3. Create a Title, Date, and Category for the file in the top 3 lines of the file like this:  

        Title: name  
        Date: yyyy-mm-dd hh:mm   
        Category: name  
#### Layout
1. Write your name with a # before it at line after the setup like this:  

        # FirstName LastName
2. Write your contact information underneath your name
3. Add a section heading underneath like this:

        ## Heading name

    According to Etter there should be a bias towards including headers as they make the writing more approachable.   

4. Write what you want in it. As a recommendations for something like a job postion you can write something like this:

        **Job Title -** _Company Name_, StartDate – EndDate  
        * Information about the job

    Using inline styles to offset offset different sections of the job description help with visual clearity and makes it easy to find inprted informaion.

5. Repeat step 3 and 4 until everything you wanted to include in the resume is there.

#### Hosting
1. Install ghp-import in the root of the folder using: 
        
        python -m pip install ghp-import
   May need to use python3 instead of python.

2. [Install Git](https://git-scm.com/)
3. Create a GitHub account.
4. Create a repository and make sure it is public.
5. Go to setting in the repository.
6. Go to the pages page under Code and automation.
7. Pick the source and save.
8. After waiting for a bit refresh the page.
9. Click on the **Visit site** button on the GitHub Pages page to visit the website.

#### Publishing
 1. pelican content -s publishconf.py
 2. ghp-import output -b gh-pages
 3. Use:

        git push origin gh-pages
    to push the changes made to the repository.

#### Running
Using a terminal (for testing purposes):
* To run use the following in the teminal while being in the root of the project:  

        pelican -r -l
Using GitHub:
1. Go to setting in the repository.
2. Go to the pages page under Code and automation.
5. Click on the **Visit site** button on the GitHub Pages page.

## Further Resources/Readings
* [GitHub Tutorial](https://docs.github.com/en/get-started)  
* [Git Tutorial](https://git-scm.com/docs/gittutorial)  
* [Pelican Tutorial](https://docs.getpelican.com/en/latest/)  
* [Markdown Tutorial](https://www.markdownguide.org/basic-syntax/)   

## FAQ
1. Q. Why is Markdown better than writing raw HTML?  
A. It has a clean syntax that makes it simple for peopel to understaned and use.  
2. Q. "I changed the Markdown version of my resume, so why don’t I see the changes when I refresh the website in my browser?”  
A. Just changing the Markdown doesn't change the repository the website is hosted on, you have to update the files in the repository to have your website proccess the changes.
3. Q. Why is markdown the most popular lightweight markup language?  
A. Markdown is popular because it has a very simple syntax which makes it easy to read and use. 
4. Q. How can you check how the Markdown is compiled?  
A. There are a lot of compilers that can read Markdown to bea able to review the compilation such as [markdownlivepreview](https://markdownlivepreview.com).
5. Q. Why does markdown produces different outputs depending on where you run it?  
A. 

## Credits
* Mohammad Adnan Malik
* Fawaz Saleem
* Andrew Etter's Modern Technical Writing [An Introduction to Software Documintation]

## things needed
* More than anything, they need reference materials, short tutorials, and code samples.
* Bias towards including headers, tables, lists, diagrams, and images. These additions make your writing more approachable and simpler to scan than paragraph after paragraph of prose.
* Use inline styles to offset important text.
