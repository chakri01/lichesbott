- 👋 Hi, I’m @chakri01
- 👀 I’m interested in making games
- 🌱 I’m currently learning java
- 💞️ I’m looking to collaborate on java challenges
- 📫 How to reach me kachamchakri.80968.kc@gmail.com

<!---
chakri01/chakri01 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

lichess-bot
A bridge between Lichess API and bots.

How to Install
Mac/Linux:
NOTE: Only Python 3.7 or later is supported!
Download the repo into lichess-bot directory
Navigate to the directory in cmd/Terminal: cd lichess-bot
Install pip: apt install python3-pip
Install virtualenv: pip install virtualenv
Setup virtualenv: apt install python3-venv
python3 -m venv venv #if this fails you probably need to add Python3 to your PATH
virtualenv .venv -p python3 #if this fails you probably need to add Python3 to your PATH
source ./venv/bin/activate
python3 -m pip install -r requirements.txt
Copy config.yml.default to config.yml
Edit the variants: supported_variants and time controls: supported_tc from the config.yml as necessary
Windows:
Here is a video on how to install the bot: (https://youtu.be/w-aJFk00POQ). Or you may proceed to the next steps.
NOTE: Only Python 3.7 or later is supported!
If you don't have Python, you may download it here: (https://www.python.org/downloads/). When installing it, enable "add Python to PATH", then go to custom installation (this may be not necessary, but on some computers it won't work otherwise) and enable all options (especially "install for all users"), except the last . It's better to install Python in a path without spaces, like "C:\Python".
To type commands it's better to use PowerShell. Go to Start menu and type "PowerShell" (you may use cmd too, but sometimes it may not work).
Then you may need to upgrade pip. Execute "python -m pip install --upgrade pip" in PowerShell.
Download the repo into lichess-bot directory.
Navigate to the directory in PowerShell: cd [folder's adress] (like "cd C:\chess\lichess-bot").
Install virtualenv: pip install virtualenv.
Setup virtualenv:
virtualenv .venv -p python (if this fails you probably need to add Python to your PATH)
./.venv/Scripts/activate (.\.venv\Scripts\activate should work in cmd in administator mode) (This may not work on Windows, and in this case you need to execute "Set-ExecutionPolicy RemoteSigned" first and choose "Y" there [you may need to run Powershell as administrator]. After you executed the script, change execution policy back with "Set-ExecutionPolicy Restricted" and pressing "Y")
pip install -r requirements.txt
Copy config.yml.default to config.yml
Edit the variants: supported_variants and time controls: supported_tc from the config.yml as necessary (use # to disable certain ones)
Lichess OAuth
Create an account for your bot on Lichess.org
NOTE: If you have previously played games on an existing account, you will not be able to use it as a bot account
Once your account has been created and you are logged in, create a personal OAuth2 token with the "Play as a bot" selected and add a description
A token e.g. Xb0ddNrLabc0lGK2 will be displayed. Store this in config.yml as the token field
NOTE: You won't see this token again on Lichess.
Setup Engine
Place your engine(s) in the engine.dir directory
In config.yml, enter the binary name as the engine.name field (In Windows you may need to type a name with ".exe", like "lczero.exe")
