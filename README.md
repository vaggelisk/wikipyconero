# wikipyconero

1. install mysql 


2. install `nvm`


3. Go to WebstormProjects folder and write the command


    git clone https://github.com/vaggelisk/wikipyconero && cd wikipyconero

4. Choose node version


    nvm use 18

    export NODE_OPTIONS=--openssl-legacy-provider && npx yarn build

5. For developing wikipyconero, especially client-part, it's needed 
   
   1. to develop in wikiDevGit. See the app at
   > http://localhost:3090
   2. to build the code, so generating files in `assets folder`. From folder `wikiDevGit`
   > npx yarn build
   3. to copy all files of `wikiDevGit/assets` to `wikipyconero/assets`. Means from folder `wikipyconero` 
to have this command
   > cp -R ../wikiDevGit/assets/*  ./assets/




## Deploy on Server

   >  cd /var/www/pyconero.gr/node

   >  sudo -u www-data git pull

   >   systemctl restart  wiki.service

For finding configuration of the service of the wiki, you have to go to

   > sudo vi /etc/systemd/system/wiki.service

## IMPORTANT 

The translation staff is getting cached in the browser, so you could not see the changes
you implement except if you close and open your window. And it's better something like
this take place in private browser
