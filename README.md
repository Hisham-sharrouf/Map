# Map
test map in GEE

## start

cd
mkdir voila
cd voila
python -m venv venv
source venv/bin/activate
pip install voila
pip install jupyter numpy matplotlib
jupyter notebook

# Test Voila locally
voila app.ipynb

# Create Three Files
requirements.txt : pip freeze > requirements.txt
runtime.txt : python-3.7.6
Procfile  : web: voila --port=$PORT --no-browser app.ipynb

# Add, commit and push local files to GitHub

git init
git remote add origin https://github.com/<usename>/<reponame>
git add .
git commit -m "initial commit"
git pull origin master
git push origin master 
git push heroku master

# to add/edit 
git add .
git commit -m "change note"
git push origin master 
git push heroku master

# to open 
heroku open

