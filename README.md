# PortfolioWebsite
This website will be a place for me to showcase my projects and create blog posts

The goal for the landing page:
    The landing page should include an about me section.
    The landing page should show a skills table including current skills, description, project application.
    The landing page should show a featured projects table including up to 4 projects.
    The landing page should be changeable in the admin dashboard, only acceptable to me, the admin of the site.

The goal to showcase projects page: 
    Project tiles that users can click on to show more information about a project. Tiles should include a screenshot of an example of the project. Tiles should also include the main languages (or libraries) used in the project, but only up to 2. 
    The project tiles will be added/changed through the admin dashboard, only acceptable to me, the admin of the site.

The goal for blog posts page:
    The blog posts page should have an area where the admin can post blogs and see posted blogs but users can only see posted blogs.

The goal for the contact me page:
    This page will contain a section including ways the user may contact me.
    This page will contain an area for users to input their information and send me a message via email.

The goal for user interaction:
    Users should be able to view the site without authenticating but need to login for liking or commenting.
    Users should be able to register for an account.
    Users should be able to reset their password.
    Users should be able to like blog posts and comment on blog posts.
    Users should be able to navigate to all pages of the site except for admin.
    Users should be able to click on projects in the showcase to view more information and be able to like the project.

The goal for the stack: 
    I would like to use Next.js, Django, and PostgreSQL for the frontend, backend, and database.
    I will use mailgun for emails.
    I am unsure of how to currently implement blog posts.

The goal for hosting the site:
    I will use a Linode Nanode server to host the frontend server, backend server, and PostgreSQL database.

Basic design outline:
    User goes to domain.
    User is directed to landing page.
    User can interact with the site without logging in unless they wish to like or comment
    User is directed to login page for authentication.
    User may click Register Here
    User may click forgot password
    User logs in.
    User may like and comment.

    Landing page talks to backend to recieve skills table and featured projects table, shown also is the likes from each of the projects.
    Projects page talks to backend to recieve projects listed in order of being added to the page.
    Blog posts page allows admin user to post blogs and allows all other users to only read the posts, they should not see the create post button or prompt.
    Contact me page will allow users to send an email to me by completing the prompt fields of Name, Email, Subject, Message and clicking send. 