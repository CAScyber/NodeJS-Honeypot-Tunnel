# NodeJS-Honeypot-Tunnel
NodeJS setup with a tunnel to host local honeypot via localhost.run service.

• Simple setup: install NodeJS. 
<br>
• Install ADBHoney Low interaction honeypot: git clone https://github.com/huuck/ADBHoney
<br>
• Then run: python run.py
<br>
• This will start listening on port 5555 locally.
<br>
• Get your tunnel at localhost.run.
<br>
• Get your SSH key on command line: ssh-keygen -t rsa
<br>
• Copy your key. Look for the rsa.pub file.
<br>
• And to finish off, after putting your SSH key into the site at localhost.run, we use the command: ssh -R 80:localhost:5555 localhost.run 
<br>
• Or another port other than 5555; 8080 is default.
<br>
• It will ask us to sign in, then it will run and give us a link to the honeypot we are running.
