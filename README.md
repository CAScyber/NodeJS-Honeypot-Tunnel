# NodeJS-Honeypot-Tunnel
NodeJS setup with a tunnel to host local honeypot via localhost.run service.

• Simple setup: install NodeJS. 
• Install ADBHoney Low interaction honeypot:
# git clone https://github.com/huuck/ADBHoney
• Then run: 
# python run.py
• This will start listening on port 5555 locally.
• Get your tunnel at localhost.run.
• Get your SSH key on command line: 
# ssh-keygen -t rsa
• Copy your key. Look for the rsa.pub file.
• And to finish off, after putting your SSH key into the site at localhost.run, we use the command: 
# ssh -R 80:localhost:5555 localhost.run 
• Or another port other than 5555; 8080 is default.
• It will ask us to sign in, then it will run and give us a link, with 
