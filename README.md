## How to run it locally
- Create a virtual environment with `py -m venv env`
- Activate it with `.\env\Scripts\activate`
- Install requirements.txt with `pip install -r requirements.txt`
- Run the project with `mkdocs serve`
- You can see it on `http://127.0.0.1:8000`
- You can create new docs by adding a new file for your doc in the `docs` folder and create it inside one of the sub-folders there or create a new folder, this sub-folders are used as topics or categories
- The file should be markdown, so for example `my-doc.md`
- A path to access the page of your new doc will be created automatically and you can access it by the folder path like `http://127.0.0.1:8000/sub-folder/my-doc` because the `docs` folder acts as the home path `/`
- You can directly make and commit your new changes in this branch `mkdocs-material`, this is the production branch and Netlify will deploy your changes as soon as you push your new commits.
