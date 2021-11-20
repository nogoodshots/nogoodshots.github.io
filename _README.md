
```
bundle install
bundle exec jekyll serve
```

Now you should be able to see the content on http://localhost:4000

If nothing happens add --trace onto the end of the bundle exec command to get more information.

## Formatting the page
Pick a page background colour.

Check out the colours on https://www.w3schools.com/cssref/css_colors.asp . Note each one has a code under the name, for example Crimson has code #DC143C.

Pick a colour and then edit _sass/main.scss look for the primary-color variable
```
$primary-color: #DC143C;
```
Replace the value between : and ; with the chosen code.

Repeat the same for primary-text-color (apologies for the American spelling).



It is hard to get ssh working

On Mac

ssh-keygen -t ed25519 -C "nogoodshots@gmail.com"

eval "$(ssh-agent -s)"

touch ~/.ssh/config
vi ~/.ssh/config

Host *
  AddKeysToAgent yes
  UseKeychain yes
  IdentityFile ~/.ssh/id_ed25519

ssh-add -K ~/.ssh/id_ed25519

