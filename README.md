### ubuntu
---

http://ftp.riken.jp/Linux/ubuntu/

https://github.com/chef/bento

```
```

```
```


```
// Settings
//　キーボードレイアウト
// 日本語英語切り替え
// Ctrl+Space




// Window Snipping
sudo apt-get install unity-tweak-tool -y

```
---



###### ubuntu rbenv,rails s 
```
// ubuntu setup
sudo apt install git
sudo apt install g++
sudo apt-get install -y libreadline6-dev
sudo apt-get install -y git curl curl g++ make
sudo apt-get install -y zlib1g-dev libssl-dev libreadline-dev
sudo apt-get install -y libyaml-dev libxml2-dev libxslt-dev
sudo apt-get install -y sqlite3 libsqlite3-dev nodejs

git clone https://github.com/rbenv/rbenv.git ~/.rbenv
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(rbenv init -)"' >> ~/.bashrc
exec $SHELL

git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
exec $SHELL

rbenv install -l
rbenv install 2.7.1
rbenv rehash
rbenv global 2.7.1
ruby -v

gem install bundler
mkdir dev1 && cd dev1
bundle init 
vi Gemfile
# gem "rails"
bundle install

sudo apt-get upgrade
exec $SHELL // source ~/.bash_profile

rails new apptky1 && cd apptky1
bundle install

sudo sh -c 'echo "deb http://packages.dotdeb.org wheezy all" > /etc/apt/sources.list.d/dotdeb.list'
sudo sh -c 'echo "deb-src http://packages.dotdeb.org wheezy all" >> /etc/apt/sources.list.d/dotdeb.list'
cd /tmp
wget http://www.dotdeb.org/dotdeb.gpg
sudo apt-key add dotdeb.gpg

curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
sudo apt-get update && sudo apt-get install yarn

exec $SHELL
yarn -v
yarn install

rails webpacker:install
rails s
curl https://127.0.0.1:3000/

vi ~/.gemrc
/* .gemrc
install: --no-ri --no-rdoc
update: --no-ri --no-rdoc
*/
cd aptky1
vi Gemfile
# gem "rails", '6.0.3.2'


sudo apt install -y nodejs npm
sudo npm install n -g
sudo n stable
sudo apt purge -y nodejs npm
sudo apt autoremove
exec $SHELL -l
node -v

sudo n 12.18.3
node -v
sudo n lts
node -v

yarn install --check-files
rails -b.0.0.0.

```
