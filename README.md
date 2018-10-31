# jrdevleague-installfest
Setting up Environment for start of the school year

## Github
  1. Go to github.com
  2. Click on sign up
  3. Type username
  4. Type Email
  5. Password **REMEMBER YOUR PASSWORD**
  6. Choose Unlimited Plan

## Set Up SSH Keys
  ### Generating SSH Keys
  1. Open Terminal
  2. Paste the text below, substituting in your GitHub email address.
  ```
  ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
  ```
  3. When you're prompted to "Enter a file in which to save the key," press Enter. This accepts the default file location.
  ```
  Enter a file in which to save the key (/Users/you/.ssh/id_rsa): [Press enter]
  ```
  4. At the prompt, type a secure passphrase. For more information, see "Working with SSH key passphrases".
  ```
  Enter passphrase (empty for no passphrase): [Type a passphrase]
  Enter same passphrase again: [Type passphrase again]
  ```
  ** YOUR PASSPHRASE WILL BE HIDDEN WHILE TYPING **
  
  ### Adding your SSH key to ssh-agent
  1. Start the ssh-agent in the background.
  ```
  eval $(ssh-agent -s)
  ```
  - On Mac
  ```
  ssh-add -K ~/.ssh/id_rsa
  ```
  - On Windows
  ```
  ssh-add ~/.ssh/id_rsa
  ```
  
  ### Add SSH key to your Github account
  https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/

## Git
  1. Install Git https://git-scm.com/downloads
  2. $ git config --global user.name "Mona Lisa"
  3. $ git config --global user.email "email@example.com" 

## VSCode
  - Install Windows or Mac https://code.visualstudio.com/
  - **Open VScode from terminal**
    1. Command + shift + p
    2. Install code command path
  - **Set up git-bash with integrated terminal in VScode**
    - Go into settings and search for "terminal.integrated.shell.windows"
    - "terminal.integrated.shell.windows": "C:\\Program Files\\Git\\bin\\bash.exe"
    OR
    - Type `bash` in your vs terminal window
    - A pop-up will ask if you'd like to customize your intergrated terminal
    - Select `git bash` terminal
    
## Node
  1. Install node https://nodejs.org/en/download/
  2. Npm install -g live-server 
