## Install notes ##

- Go get a coffee, make it a venti...
- Install python (if you don't have it installed on your system)
    -- https://docs.djangoproject.com/en/1.4/topics/install/#installing-official-release
    -- on Mac OSX (install Homebrew), `$ homebrew install python` (this installs pip as well)
- Install pip
    -- After installing Python, easy_install command in terminal should be available to you.
        -- `$ sudo easy_install pip`
- Install all dependencies
    -- `$ pip install -r requirements.txt`
- Sync the database (will create a sqlite3 db locally)
    -- `python manage.py syncdb`
    -- Fill out instructions by saying 'yes' and enter your credentials that you see fit.
- Update the MEDIA_ROOT in local_settings.py
    -- Line 20, should be an absoulte path to the 'geekdom/media' folder
    -- example: '/Users/iMac/Dropbox/Code/geekdom/media'
- Run the djanjo dev server
    -- `python manage.py runserver`
- Update local_settings.py to use Djano's web server
    -- `


====
API GET Request
====

http://members.geekdom.com/api/users/get/user_id/<username>/?api_key=RZSOY7O0FSAO65NZYF68W2OZ4BDBRBJY



Other notes about installation:    
-- If you're feeling lucky install all this in virtualenv, but I don't know how.


__________________
planned features

for users:

    - view all public forums
        - create thread
        - view thread
            - reply to thread

    - view my forums / classes / workshops
        - create thread
        - view thread
            - reply to thread
        - sign up for class / workshop


for admins:

    - create public forum / class / workshop
    
    - view my classes
        - enrollment stats
        - add new event to calendar
            - attach files to event