# myonlinebook

git clone https://github.com/dragonleopardpig/myonlinebook

jupyter-book clean mylocalbook/ --all

jupyter-book build mylocalbook/ --all

rm -rf myonlinebook/_build

rsync -avP --delete mylocalbook/ myonlinebook/

cd myonlinebook

git add .

git commit -m "message"

git push

ghp-import -n -p -f _build/html
