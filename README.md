sudo apt-get install python-pip
pip install --user git+git://github.com/Lokaltog/powerline
wget https://github.com/Lokaltog/powerline/raw/develop/font/PowerlineSymbols.otf https://github.com/Lokaltog/powerline/raw/develop/font/10-powerline-symbols.conf
mkdir ~/.fonts/
mv PowerlineSymbols.otf ~/.fonts/
fc-cache -vf ~/.fonts
mkdir -p ~/.config/fontconfig/conf.d/ && mv 10-powerline-symbols.conf ~/.config/fontconfig/conf.d/
git clone https://github.com/milkbikis/powerline-shell.git
cd powerline-shell
./install.py
ln -s  ~/powerline-shell.py
ll
cd ..
git clone https://github.com/powerline/fonts.git
cd fonts/
./install.sh
