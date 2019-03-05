Starting in index.Bundle1
SPA for Web Developer Testing Project.
    Prepared by Allen Jones
    Uses Bootstrap Modals for login, register, and ckeditor forms
    Adds input data from registration into indexed database
    References database for password check, proceeds to profile page

    The database is persistant through browser close. No accounts exist at first
    Messages are displayed through html appendages, and removed and re-appended
    during each visit, post, and deletion.
    
    Tesing has only been done on Google Chrome. 

    html head:
        Resources

    html body:
        Welcome screen/header
            Login modal
            Register modal
            ckeditor modal
        Message area
            created elements for threads
                Created area for replies
        Error area

    Javascript Functions
    UserInput - Takes user input from the modals and calls the functions

    Register - Takes user input for username and password
    adds info to indexed database, handles errors

    login - Takes user input for username and password
    attempts to reference input password with database entry matching username
    this poses security risks, allowing password to be viewed in debugging.

    goToProfile - Enambles the messages element

    openEdit - Opens ckeditor for editing an existing post, passing id along
    to updatate the database

    openReply - opens ckeditor for a reply, passing the thread and title to
    create a new element for the purpose of collapsing

    addPost - Intakes username, ckeditor data, the current date, and the title
    and adds this info to the IDB. The database is counted to determine the next
    id number.

    postMessageButton - The function for the Post Message Button. Calls addPost
    to add the ckeditor data to the database. THen calls displayPost to reset
    the posts on screen

    deletePost - Intakes the post id from the delete post button and deletes the
    appropriate post. Then calls displayPost to reset the posts on screen

    displayPost - Removes all content in the postarea element, then appends all
    posts through the database using a cursor.

    initCascadePosts - takes the post's thread and title to collapse the thread 
    into a button to expand them again.'

I do not own the loading.gif image used. The Jimg.png is royalty free from pixabay.
