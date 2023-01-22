# D365FO
```bash
➜  ~ curl -sL firebase.tools | bash
Password:
➜  ~ mkdir D365FO
➜  ~ cd D365FO
➜  D365FO ls
➜  D365FO firebase init hosting

echo "# D365FO" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/hajsf/D365FO.git
git push -u origin main

After modifying the files:
git commit -m "modify index.html"
git push -u origin main

➜  D365FO firebase init hosting

     ######## #### ########  ######## ########     ###     ######  ########
     ##        ##  ##     ## ##       ##     ##  ##   ##  ##       ##
     ######    ##  ########  ######   ########  #########  ######  ######
     ##        ##  ##    ##  ##       ##     ## ##     ##       ## ##
     ##       #### ##     ## ######## ########  ##     ##  ######  ########

You're about to initialize a Firebase project in this directory:

  /Users/hajsf/D365FO


=== Project Setup

First, let's associate this project directory with a Firebase project.
You can create multiple project aliases by running firebase use --add,
but for now we'll just set up a default project.

? Please select an option: Use an existing project
? Select a default Firebase project for this directory: d365fo-4a6e3 (D365FO)
i  Using project d365fo-4a6e3 (D365FO)

=== Hosting Setup

Your public directory is the folder (relative to your project directory) that
will contain Hosting assets to be uploaded with firebase deploy. If you
have a build process for your assets, use your build's output directory.

? What do you want to use as your public directory? public
? Configure as a single-page app (rewrite all urls to /index.html)? Yes
? Set up automatic builds and deploys with GitHub? Yes
✔  Wrote public/index.html

i  Didn't detect a .git folder. Assuming /Users/hajsf/D365FO is the project root.
i  Authorizing with GitHub to upload your service account to a GitHub repository's secrets store.

Visit this URL on this device to log in:
https://github.com/login/oauth/authorize?client_id=89cf50f02ac6aaed3484&state=478171168&redirect_uri=http%3A%2F%2Flocalhost%3A9005&scope=read%3Auser%20repo%20public_repo

Waiting for authentication...

✔  Success! Logged into GitHub as hajsf

? For which GitHub repository would you like to set up a GitHub workflow? (format: user/repository) hajsf/D365FO

✔  Created service account github-action-592039788 with Firebase Hosting admin permissions.
✔  Uploaded service account JSON to GitHub as secret FIREBASE_SERVICE_ACCOUNT_D365FO_4A6E3.
i  You can manage your secrets at https://github.com/hajsf/D365FO/settings/secrets.

? Set up the workflow to run a build script before every deploy? No

✔  Created workflow file /Users/hajsf/D365FO/.github/workflows/firebase-hosting-pull-request.yml
? Set up automatic deployment to your site's live channel when a PR is merged? Yes
? What is the name of the GitHub branch associated with your site's live channel? main

✔  Created workflow file /Users/hajsf/D365FO/.github/workflows/firebase-hosting-merge.yml

i  Action required: Visit this URL to revoke authorization for the Firebase CLI GitHub OAuth App:
https://github.com/settings/connections/applications/89cf50f02ac6aaed3484
i  Action required: Push any new workflow file(s) to your repo

i  Writing configuration info to firebase.json...
i  Writing project information to .firebaserc...
i  Writing gitignore file to .gitignore...

✔  Firebase initialization complete!
➜  D365FO echo "# D365FO" >> README.md
➜  D365FO git init
hint: Using 'master' as the name for the initial branch. This default branch name
hint: is subject to change. To configure the initial branch name to use in all
hint: of your new repositories, which will suppress this warning, call:
hint:
hint: 	git config --global init.defaultBranch <name>
hint:
hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
hint: 'development'. The just-created branch can be renamed via this command:
hint:
hint: 	git branch -m <name>
Initialized empty Git repository in /Users/hajsf/D365FO/.git/
➜  D365FO git:(master) ✗ git add .
➜  D365FO git:(master) ✗ git commit -m "first commit"
[master (root-commit) a31c69f] first commit
 7 files changed, 212 insertions(+)
 create mode 100644 .firebaserc
 create mode 100644 .github/workflows/firebase-hosting-merge.yml
 create mode 100644 .github/workflows/firebase-hosting-pull-request.yml
 create mode 100644 .gitignore
 create mode 100644 README.md
 create mode 100644 firebase.json
 create mode 100644 public/index.html
➜  D365FO git:(master) git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'origin'
➜  D365FO git:(master) git branch -M main
➜  D365FO git:(main) git push -u origin main
fatal: 'origin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
➜  D365FO git:(main) git remote add origin https://github.com/hajsf/D365FO.git
➜  D365FO git:(main) git push -u origin main
Enumerating objects: 12, done.
Counting objects: 100% (12/12), done.
Delta compression using up to 4 threads
Compressing objects: 100% (9/9), done.
Writing objects: 100% (12/12), 3.40 KiB | 1.70 MiB/s, done.
Total 12 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/hajsf/D365FO.git
 * [new branch]      main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.
➜  D365FO git:(main) git commit -m "modify index.html"
[main 79e8fb1] modify index.html
 3 files changed, 47 insertions(+), 91 deletions(-)
 rewrite public/index.html (61%)
➜  D365FO git:(main) git push -u origin main
Enumerating objects: 11, done.
Counting objects: 100% (11/11), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (6/6), 712 bytes | 712.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/hajsf/D365FO.git
   a31c69f..79e8fb1  main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.
➜  D365FO git:(main) cd ..
➜  ~ ls
```
