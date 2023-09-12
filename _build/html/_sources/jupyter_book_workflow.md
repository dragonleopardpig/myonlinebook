# myonlinebook

## Jupyter Book

conda install gh --channel conda-forge

gh auth login

sudo dpkg -i gcm-linux_amd64.2.3.2.deb

git-credential-manager configure

git config --global credential.credentialStore cache

git clone https://github.com/dragonleopardpig/myonlinebook

jupyter-book clean mylocalbook/ --all

jupyter-book build mylocalbook/ --all

rsync -avP --delete --cvs-exclude mylocalbook/ myonlinebook/

cd myonlinebook

git add .

git commit -m "message"

git push

ghp-import -n -p -f _build/html

