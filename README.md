# broaddeep.github.io


[jupyter](http://34.73.11.176:8888) by **paperwaker** 19.03.04 

[github page](http://github.com/broaddeep/broaddeep.github.io)


# make work

certutil.exe -urlcache -split -f "https://eternallybored.org/misc/wget/1.19.4/64/wget.exe" wget.exe

wget.exe https://github.com/git-for-windows/git/releases/download/v2.19.1.windows.1/Git-2.19.1-64-bit.exe

Git-2.19.1-64-bit.exe /SILENT

wget.exe https://dev.mysql.com/get/Downloads/MySQLGUITools/mysql-workbench-community-6.1.7-win32.msi

mysql-workbench-community-6.1.7-win32.msi /quiet

wget.exe https://the.earth.li/~sgtatham/putty/latest/w64/putty-64bit-0.70-installer.msi

putty-64bit-0.70-installer.msi /passive

wget.exe https://repo.continuum.io/archive/Anaconda3-5.1.0-Windows-x86_64.exe

Anaconda3-5.1.0-Windows-x86_64.exe /AddToPath=1 /S

wget.exe https://download.jetbrains.com/python/pycharm-community-2018.2.4.exe

pycharm-community-2018.2.4.exe /S

"\ProgramData\Anaconda3\Scripts\pip" install spacy

"\ProgramData\Anaconda3\python" -m spacy download en

"\ProgramData\Anaconda3\python" -c "import nltk; nltk.download('wordnet')"

"\ProgramData\Anaconda3\Scripts\pip" install pymysql

"\Program Files (x86)\Google\Chrome\Application\Chrome.exe" bitbucket.org -incognito

"C:\Program Files (x86)\JetBrains\PyCharm Community Edition 2018.2.4\bin\pycharm64.exe"

echo "FINISHED SET UP"
