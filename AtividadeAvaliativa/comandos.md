**Git status** → status

**Gid add <filename ou .>** → Vai adicionar um arquivo para ser commitado

**Git Restore - -staged <filename ou .>** → remover esse arquivo para ele não ser commitado

**Git branch** <branchname> → criar uma nova branch

**Git checkout** <branchname> → vai trocar de branch

**Git checkout** -b <branchname> → vai criar uma nova e trocar

**Git commit -m “<description>”** → vai fazer o commit

**Git merge** <branchname> → vai mesclar as branches

**Git branch -D <branchname>** → deletar a branch

------Aqui configura o usuário:

git --version

git config --glbal user.name "Emanuele"

git config --global user.email "Emanuele@gmail.com"


------Configura o SSH:

ls -al ~/.ssh

ssh-keygen -t ed25519 -C "Emanuele@gmail.com"

eval "$(ssh-agent -s)"

ssh-add ~/.ssh/id_ed25519

clip < ~/.ssh/id_ed25519.pub

ssh -T git@github.com

Lista de configurações -> git config --list