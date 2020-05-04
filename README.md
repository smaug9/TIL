# TIL

## 2020-05-04

### Powershell: convert array to arraylist

```
$resourceFiles = New-Object System.Collections.ArrayList(,$someArray)
```





## manually run powershell scheduled job

```
(Get-ScheduledJob -id 1).StartJob()
Receive-Job -id 1
```
  
  * ref: https://stackoverflow.com/questions/36691114/powershell-manually-trigger-a-scheduled-job
  
## install brave ubuntu

```
sudo su -
apt install curl
curl -s https://brave-browser-apt-release.s3.brave.com/brave-core.asc | sudo apt-key --keyring /etc/apt/trusted.gpg.d/brave-browser-release.gpg add -
sh -c 'echo "deb [arch=amd64] https://brave-browser-apt-release.s3.brave.com `lsb_release -sc` main" >> /etc/apt/sources.list.d/brave.list'
apt update && apt install brave-browser brave-keyring

```

  * ref: http://ubuntuhandbook.org/index.php/2018/12/how-to-install-brave-web-browser-in-ubuntu-linux-mint/
  
  
