# Create new Django / React project  `create-django-shell-func`
The `zsh`/`bash` shell function to create a django project from scratch. This function creates and starts a new django project in the `~/sites/test.python` folder. To be able to correctly use this function please follow the installation guide.

## Installation
To install this function you need to add the function to your bash/zsh/shell profile file and source the file.
### Prerequisites
- Have a proper version of Python installed on your machine.
- Have Python aliase or symlined to work with the command `python`, or change line `58` of the function to use the correct python command, in most cases it can be `python3`.
### Step-by-step
1. Copy and paste the contents of the file `shell-func.txt` into your `~/.zshrc` or `~/.bash_profile` file
3. Create the folder named `~/sites/test.python` or change line `48` of the function to point to the folder you want your project to be created.
2. Run `source ~/.zshrc` or `source ~/.bash_profile` accordingly.

## Usage
```
create [instance] [name] [-d --dev | -r --with-react]

Instance:
django  : currently the only project instance allower. Soon Yii2 instance to be implemented

Name:
The name of the project to be created. Have in mind the diferente django and react restriction to naming projects.

Options (and corresponding environment variables):
-d --dev        : starts the django development server with the --insecure flag to allow 
                  static files from being pulled from any STATICFILES_DIRS directories
-r --with-react : creates the project with a React.js front-end module to separate between
                  the django back-end logic
```
