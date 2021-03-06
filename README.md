# Recipes

## Developer setup

To activate your virtual environment:

```powershell
# for powershell
./venv/Scripts/activate.ps1
```

```batch
::for batch
venv\Scripts\activate
```

Then, you can run any python command such as running jupyter notebooks or pelican or pip.

## How to install packages from a file.

You can manually install packages or save them in a requirements file. This is helpful to make your environments more portable.

If you want, you can specify which python packages you want to install in your environment

```batch
:: install whatever is in your requirements
pip install -r requirements.txt

- show what's currently installed.
pip freeze
``` 

Generally, you can just pick the top-level packages and just list those instead of all their dependencies.

### ToDo: Figure out how to store passwords in a .env file so I don't have to type them over and over...

``` Powershell Prompt
To change the Powershell prompt to only display the current working directory copy and paste this into your powershell:

function prompt {
$(($pwd -split '\\')[-1] -join '\') + '> '
}
```
function prompt {'<recipes> '+$(($pwd -split '\\')[-1] -join '\') + '> '}

``` Turning off Git warning message
With Git, when using the autocrlf = true flag, a warning is still given when line-endings are changed. Here's how to turn off the annoying message:

git config --global core.safecrlf false
```

