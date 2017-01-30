# testssh
Empty repo test ssh set up only

> Use multiple SSH private keys on one client

1. Generete SSH key
    `ssh-keygen -t rsa -f ~/.ssh/nux.github.id_rsa -C "nuxlee92@gmail.com"`
2. Create/Update `~/.ssh/config`
    `vi ~/.ssh/config`
    ```
    Host github.com
    HostName github.com
    User git
    IdentityFile ~/.ssh/nux.github.is_rsa
    ```
3. Add generated public key to Github
    `pbcopy < ~/.ssh/nux.github.id_rsa.pub`
    
