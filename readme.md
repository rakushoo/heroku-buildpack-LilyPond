# Heroku Buildpack: LilyPond

Use LilyPond-Buildpack if you need Heroku to execute the LilyPond application.

## Usage

NOTE: There must be a .ly file in the root directory of the app to trigger the LilyPond installation.

<br>
Step 1: Heroku Dashboard -> <App Page> -> Settings -> Buildpacks の Add buildpack にリポジトリを追加
<br>
Step 2: コマンドラインから環境変数を追加
<br>$> heroku config:add BUILDPACK_URL=https://github.com/rakushoo/heroku-buildpack-LilyPond.git

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


