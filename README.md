# mkproject_script
shell script for creating files and folders for basic web development projects

## Structure
The following structure is created in the current directory upon executing the command.

./projectdir <br />
  | <br />
  +--- index.html <br />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| <br />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+--- ./html <br />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| <br />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+--- ./css <br />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+-- style.css <br />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| <br />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+--- ./js <br />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+-- index.js <br />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| <br />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+--- ./resources <br />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+-- ./images <br />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+-- ./audio <br />
               
## How to use the script

### Method 1: Locally

You can clone or copy the script mkproject.sh in the directory in which you need to create the project into, and the execute it as:

```sh
./mkproject.sh
```

Note: For this method you would have to copy the script into the project directory for each new project.

### Method 2: Globally (Not recommended if you have no experience with PATH and/or environment variables in general)

Follow these steps, if you would like to execute the mkproject.sh from any path you are into

#### Step 1: Create $HOME/bin

```sh
mkdir $HOME/bin
````

### Step 2: Copy the script into $HOME/bin

To open the route
```sh
cd
cd $HOME/bin
````

Use nano to create and modify the script file
```sh
nano mkproject.sh
````

Copy the script content into your newly created mkproject.sh file, and follow the instructions to save and exit.

Use chmod to give execution permissions to the script
```sh
chmod +x mkproject.sh
```

Add the following to your PATH PATH="$HOME/bin:$PATH (go to ~/.zshrc in mac or ~/.bashrc in linux)
restart your .bashrc/.zshrc
```sh
source ~/.zshrc
```

After adding the script globally you might execute it as any other command just by calling its name without the extension .sh

```sh
mkproject
```

## Support & Troubleshooting

You might inform me of any bug or problem at luisca246@gmail.com
