# wsl2 docker start script
Script to add wsl2 and winhost to the windows hosts file the ```windows/System32/drivers/etc/hosts``` file must be writable by the user running WSL2;
1. Open File Explorer: 
    <img src="https://winaero.com/blog/wp-content/uploads/2018/12/file-explorer-folder-libraries-icon-18298.png" alt="alt text" title="image Title" width="50"/>
2.  Go to ```C:\Windows\System32\drivers\etc``` address;
3.  hosts _(Type: File)_ properties => Security => Edit => Allow Full control for users;

# Install

1. Clone the repository :
``` git clone https://github.com/AleksiDu/wsl2-docker-phpstorm.git ```

2. Create links to the directory ``` /usr/local/bin/ ```
``` 
sudo ln -s $(pwd)/prepare-hosts /usr/local/bin/ 
sudo ln -s $(pwd)/docker-start/usr/local/bin/
 ```
3. Creating permission for commands:
```
sudo chmod u=rwx docker-start
sudo chmod u=rwx prepare-hosts
```
### docker server will be available at ```tcp://wsl2:2375```

## Enjoy!!!