> Use multiple SSH keys on one client

Save from hassles not re-entering username/passwd mutiple times with *HTTPS*

### Generate/Upload `private`/`public` key pairs

1. Generete SSH key

    `ssh-keygen -t rsa -f ~/.ssh/nux.github.id_rsa -C "nuxlee92@gmail.com"`

2. Create/Update `vi ~/.ssh/config`

    ```
    Host personal/company # alias of HostName
    HostName github.com
    User git
    IdentityFile ~/.ssh/nux.github.is_rsa
    ```

3. Add generated public key to Github (remote server)

    `pbcopy < ~/.ssh/nux.github.id_rsa.pub`

### Link to git repo    

1. Clone the repo with *configured* Host

    `git clone git@personal:n-u-x/testssh.git`

2. Set the right author if necessary

    `git config user.name <username>`
    `git config user.email <email>`
