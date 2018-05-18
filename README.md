# pull-request-from-console
## install go
git clone https://go.googlesource.com/go
cd go
git checkout go1.10.2
cd src
./all.bash
### add path variables
export GOROOT=$HOME/go
export PATH=$PATH:$GOROOT/bin
## install hub
git clone https://github.com/github/hub.git && cd hub
script/build -o ~/bin/hub
### add alias
alias git=hub
## usage: git pull-request [-f] [-m `MESSAGE`|-F `FILE`|-i `ISSUE`|`ISSUE-URL`] [-o] [-b `BASE`] [-h `HEAD`]
