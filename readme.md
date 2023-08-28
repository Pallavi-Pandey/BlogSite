# Local Setup
- Clone the project
- Run `setup.sh`

# Local Development Run
- `local_run.sh` It will start the flask app in `development`. Suited for local development

# Folder Structure

- `db_directory` has the sqlite DB. It can be anywhere on the machine. Adjust the path in ``application/config.py`. Repo ships with one required for testing.
- `application` is where our application code is
- `setup.sh` set up the virtualenv inside a local `.env` folder. Uses `pyproject.toml` and `poetry` to setup the project
- `local_run.sh`  Used to run the flask application in development mode
- `static` - default `static` files folder. It serves at '/static' path. More about it is [here](https://flask.palletsprojects.com/en/2.0.x/tutorial/static/).
- `static/bootstrap` We have already added the bootstrap files so it can be used
- `static/style.css` Custom CSS. You can edit it. Its empty currently
- `templates` - Default flask templates folder


'''
.
|   Blog Lite Documentation.pdf
|   BlogLite_API.yaml
|   local_run.sh
|   local_setup.sh
|   main.py
|   readme.md
|   requirements.txt
|   tree.txt
|   
+---application
|   |   api.py
|   |   config.py
|   |   controllers.py
|   |   database.py
|   |   models.py
|   |   myfunctions.py
|   |   validation.py
|   |   __init__.py
|   |   
|   \---__pycache__
|           api.cpython-38.pyc
|           config.cpython-38.pyc
|           controllers.cpython-38.pyc
|           database.cpython-38.pyc
|           models.cpython-38.pyc
|           myfunctions.cpython-38.pyc
|           validation.cpython-38.pyc
|           __init__.cpython-38.pyc
|           
+---db_directory
|       bloglitedb.sqlite3
|       
+---static
|   |   add_edit_post.css
|   |   followers-following.css
|   |   header.css
|   |   home.css
|   |   profile.css
|   |   search.css
|   |   signup.css
|   |   style.css
|   |   
|   +---bootstrap
|   |   +---css
|   |   |       bootstrap-grid.css
|   |   |       bootstrap-grid.css.map
|   |   |       bootstrap-grid.min.css
|   |   |       bootstrap-grid.min.css.map
|   |   |       bootstrap-grid.rtl.css
|   |   |       bootstrap-grid.rtl.css.map
|   |   |       bootstrap-grid.rtl.min.css
|   |   |       bootstrap-grid.rtl.min.css.map
|   |   |       bootstrap-reboot.css
|   |   |       bootstrap-reboot.css.map
|   |   |       bootstrap-reboot.min.css
|   |   |       bootstrap-reboot.min.css.map
|   |   |       bootstrap-reboot.rtl.css
|   |   |       bootstrap-reboot.rtl.css.map
|   |   |       bootstrap-reboot.rtl.min.css
|   |   |       bootstrap-reboot.rtl.min.css.map
|   |   |       bootstrap-utilities.css
|   |   |       bootstrap-utilities.css.map
|   |   |       bootstrap-utilities.min.css
|   |   |       bootstrap-utilities.min.css.map
|   |   |       bootstrap-utilities.rtl.css
|   |   |       bootstrap-utilities.rtl.css.map
|   |   |       bootstrap-utilities.rtl.min.css
|   |   |       bootstrap-utilities.rtl.min.css.map
|   |   |       bootstrap.css
|   |   |       bootstrap.css.map
|   |   |       bootstrap.min.css
|   |   |       bootstrap.min.css.map
|   |   |       bootstrap.rtl.css
|   |   |       bootstrap.rtl.css.map
|   |   |       bootstrap.rtl.min.css
|   |   |       bootstrap.rtl.min.css.map
|   |   |       
|   |   \---js
|   |           bootstrap.bundle.js
|   |           bootstrap.bundle.js.map
|   |           bootstrap.bundle.min.js
|   |           bootstrap.bundle.min.js.map
|   |           bootstrap.esm.js
|   |           bootstrap.esm.js.map
|   |           bootstrap.esm.min.js
|   |           bootstrap.esm.min.js.map
|   |           bootstrap.js
|   |           bootstrap.js.map
|   |           bootstrap.min.js
|   |           bootstrap.min.js.map
|   |           
|   +---images
|   |       blank-profile-picture.png
|   |       blogliteimg.png
|   |       no-image-selected.jpg
|   |       
|   \---js
|           custom_validations.js
|           signup_validations.js
|           
\---templates
        addpost.html
        archived_posts.html
        base.html
        edit_post.html
        edit_profile.html
        error.html
        home.html
        index.html
        profile.html
        search.html
        search_response.html
        session_expired.html
        signup.html
        test.html
        view_followers.html
        view_following.html
        view_post.html
        view_profile.html

'''