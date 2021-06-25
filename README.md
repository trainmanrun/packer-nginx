# packer-nginx

 Packer build for nginx that's on top of the base Ubuntu version which is located at: trainmanrun/bionic64

## How to use this
- Clone this repo
```
git clone https://github.com/trainmanrun/packer-nginx.git
cd packer-nginx
```
- Build box
```
packer build template.json
```
- Add the box locally
```
vagrant box add --force --name nginx64 output-nginx64-vbox/package.box
```
- Test it 
```
bundle exec kitchen test
```
