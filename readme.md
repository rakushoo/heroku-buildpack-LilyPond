# Heroku Buildpack: LilyPond

Use LilyPond-Buildpack if you need Heroku to execute the LilyPond application.

## Usage

NOTE: The C app being deployed with this buildpack needs a makefile that will specify the build rules of the project.

<br>$> heroku create myapp_name -s cedar
<br>$> heroku config:add BUILDPACK_URL=https://github.com/atris/heroku-buildpack-LilyPond.git

# create your app, see test-app for an example

$> git push heroku master

<br>-----> Heroku receiving push
<br>-----> Fetching custom git buildpack... done
<br>-----> LilyPond app detected
<br>-----> makefile found
<br>gcc -o greesc1 greesc1.c
<br>-----> Compilation done
<br>-----> Discovering process types
       <br>Procfile declares types -> (none)
<br>-----> Compiled slug size: 4K
<br>-----> Launching... done, v9


