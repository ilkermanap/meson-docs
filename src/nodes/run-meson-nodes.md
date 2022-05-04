# Run Nodes

## Commands Reference

<CodeGroup>
  <CodeGroupItem title="Linux x64" active>

```bash
wget 'https://coldcdn.com/api/cdn/f2cobx/terminal/v2.5.2/meson-linux-amd64.tar.gz'    # download the terminal package
tar -zxf meson-linux-amd64.tar.gz         # unzip the package
cd ./meson-linux-amd64                    # install the app as service
sudo ./meson service-install              # input your token, port and space provide
sudo ./meson service-start                # start the app
sudo ./meson service-status               # wait about 1 minutes and check status
sudo ./meson service-stop                 # to stop meson network service
sudo ./meson service-remove               # to remove meson network application
```

  </CodeGroupItem>

  <CodeGroupItem title="Linux x86">

```bash
wget 'https://coldcdn.com/api/cdn/f2cobx/terminal/v2.5.2/meson-linux-386.tar.gz'    # download the terminal package
tar -zxf meson-linux-386.tar.gz           # unzip the package
cd ./meson-linux-386                      # install the app as service
sudo ./meson service-install              # input your token, port and space provide
sudo ./meson service-start                # start the app
sudo ./meson service-status               # wait about 1 minutes and check status
sudo ./meson service-stop                 # to stop meson network service
sudo ./meson service-remove               # to remove meson network application
```

  </CodeGroupItem>

  <CodeGroupItem title="Mac">

```bash
wget 'https://coldcdn.com/api/cdn/f2cobx/terminal/v2.5.2/meson-darwin-amd64.tar.gz'    # download the terminal package
tar -zxf meson-darwin-amd64.tar.gz        # unzip the package
cd ./meson-darwin-amd64                   # install the app as service
./meson service-install                   # input your token, port and space provide
./meson service-start                     # start the app
./meson service-status                    # wait about 1 minutes and check status
./meson service-stop                      # to stop meson network service
./meson service-remove                    # to remove meson network application
```

  </CodeGroupItem>

  <CodeGroupItem title="Win x64">

```bash
wget 'https://coldcdn.com/api/cdn/f2cobx/terminal/v2.5.2/meson-windows-amd64.zip'    # download the terminal package
unzip meson-windows-amd64.zip             # unzip the package
cd ./meson-windows-amd64 && ./meson.exe   # run the app
```

  </CodeGroupItem>

  <CodeGroupItem title="Win x86">

```bash
wget 'https://coldcdn.com/api/cdn/f2cobx/terminal/v2.5.2/meson-windows-386.zip'    # download the terminal package
unzip meson-windows-386.zip              # unzip the package
cd ./meson-windows-386 && ./meson.exe    # run the app
```

  </CodeGroupItem>
  
</CodeGroup>

## Tutorial

### Download and Install

(Currently [12/29/2021], the version is 2.5.2, please check and download the latest version) (You can always find the latest command here)

```bash
wget 'https://coldcdn.com/api/cdn/f2cobx/terminal/v2.5.2/meson-linux-amd64.tar.gz'
```

If you get notifications like "-bash: wget: command not found" telling that you can't use this command, please install wget by using "sudo apt-get install wget" first. If the above link is abnormal, please try the backup link

```bash
wget 'https://assets.meson.network:10443/static/terminal/v2.5.2/meson-linux-amd64.tar.gz'
```

### Unzip this package

```bash
tar -zxf meson-linux-amd64.tar.gz
```

### Install Meson as a service

```bash
./meson-linux-amd64 && sudo ./meson service-install
```

Token, Port, and Space are parameter you need to input here:

- Token —— from https://meson.network/terminals
- Port —— Please open a port (default:19091) from the firewall
- Space —— At least please offer 40+GB space for Meson.

High Space and Bandwidth for High Earning. please check [miningrules](https://meson.network/miningrules) for details.

### Start the service of Meson

```bash
sudo ./meson service-start
```

### Please remember to check if it runs well

Please wait about 1 minute after the above one.

```bash
sudo ./meson service-status
```

After 2-3 minutes, you will have a new terminal record at [terminals](https://meson.network/terminals). Other Commands For Your Information

If the above commands(4 - 5) fail, you could just use

```bash
./meson
```

or " nohup ./meson & " to run it in the background.

Also, there are these commands to try

```bash
sudo ./meson service-stop                #To Stop Meson Network Service
sudo ./meson service-remove              #To Remove Meson Network Application
```
You could just move the folder of Meson to change the install position.

## Common Attentions

How to Change the Port? Please modify config.txt at the folder of Meson.

How to Change the Space? Please modify config.txt at the folder of Meson. And then restart Meson by using "sudo ./meson service-stop" and "sudo ./meson service-start".

If you want to try personal computers... It's much recommended to use servers rather than personal computers which are easier and more stable. But if you still want to try to mine on your own PC at home with the network router...

## Please make sure that

You truly have an unshared bandwidth and a direct public IP.

You have set up the Port-Forwarding rules.

For public IP, you could check the IP address on the dashboard of your router, and compare it with the one you searched "My IP" from the website. If they are different, it means you don't own a public IP, and you have to get help from your network service provider or use Intranet penetration to deploy Meson then.