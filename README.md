# ai-scrape
AI-powered document scraping and analysis.

## Setup

**1. Clone the repository.** This can be done either with GitHub Desktop using the repository link, or via Command Prompt:
```bash
cd C:/.../repos
git clone https://github.com/tnjfrerich/ai-scrape
```

**2. Create a virtual environment.** This will allow you to install packages uniquely to this project, thereby avoiding package version conflicts in other projects.  
Navigate to the directory in Command Prompt with
```bash
cd C:/.../repos/ai-scrape
```
Then, create a virtual environment with
```bash
python -m venv venv
```
Finally, activate it with
```bash
venv\Scripts\activate
```
If you chose to use a virtual environment, make sure to change your Python interpreter in VSCode. Open VSCode, open the Command Palette with "F1", type "Python: Select Interpreter", and select your virtual environment (i.e., venv)

**3. Install dependencies.** The dependencies have been added to `requirements.txt`. All you need to do is run the following command:
```bash
pip install .
```
This will refer to the project's dependencies and install them for you.

## Notes

1. This repository does not include many data dependencies (manuals, scraped data, etc.). These will have to be shared manually.
2. Much of the code refers to local data files. Make sure your code refers to these files in reference to your project's directory. For example, if you have a file which `__init__.py` refers to, you can place it in the same folder and refer to it simply with `filename.txt` in your code. If the file is in the folder above `__init__.py`, you can refer to the file with `../filename.txt`, where `../` moves up a directory from the directory which `__init__.py` is in. In general, try to store data files in `ai-scrape/docs`, such that files can be easily drag-and-dropped between authors.