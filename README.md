# helix-npm-template
Cookiecutter template for creating a new NPM Package using TypeScript

# Usage
1. Create a new github repo (choose to create a readme.md and license if appropriate)
2. Sync the github repo to your local machine.
3. `cd` into the folder
4. Run: ```docker run --rm -it -v $(pwd)/..:/app/ -w /app/ python:3.12 bash -c "mkdir -p cookiecutter; cd cookiecutter; pip install cookiecutter && cookiecutter https://github.com/icanbwell/helix-npm-template.git -v -f -o ../"```
5. This will ask you for the parameters.  Be sure to use your github repo name as the directory name
6. If you get a permission error running pre-commit then run: `chmod +x ./.git/hooks/pre-commit`
