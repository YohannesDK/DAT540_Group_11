# DAT540_Group_11
Repo for group project in DAT540


## Python Environment


**To get up and running, run the first two commands (create venv/activate and install)**

From -> **DAT540_Group_11 folder** (check cmd / terminal)
- create venv and activate, (vs code should not be open when you do this)
- After this its **important** to select the create venv as Python Interpreter (look lower left in vs code)
````
Windows:
    py -3 -m venv venv
    .\venv\Scripts\activate

Mac OS / Linux:
    python3 -m venv venv
    . venv/bin/activate
````

- Install packages we use
- **Make sure**:
    - You have venv activated
```
    pip install -r requirements.txt
```
- To deactivate venv
```
    deactivate
```
- If you add a package to our project run: (to save the package in requirements.txt)
```
    pip freeze > requirements.txt
```

## Github

**Branching**

From -> **DAT540_Group_11 folder** (check cmd / terminal)
- Should be in **main branch** when you create a new branch
```
    git checkout main
```
- Pull the latest and then create a new branch
```
    git pull
    git checkout -b "yourNewBranchName"
```
- After you have created new branch, you would do you work and then update repo (see below)

**Updating repository with new code**

From -> **DAT540_Group_11 folder** (check cmd / terminal)
```
    git add .
    git commit -m "finished working on ..."
    git push
```

- If you have a new branch then **git push** wont work, you have to write:
```
    git push --set-upstream origin "yourNewBranchName"
```

**Merging / updating main branch**
- You should create a pull request on github when you are done with your work in your branch.
- Go to the repo, and click on the **pull request tab**
- then click on **New Pull Request**
- choose you branch in the dropdown where it says: **branch main <- compare:<choose your branch>**
- then finally, click **create pull request**, and if there are no merge conflicts you can merge it into main
