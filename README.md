Deploy an ACT Lab using the YAML file found in the [latest release](https://github.com/nathanmusser/act-inband-ztp-demo/releases/latest). 

SSH to the automation device in your deployed lab using the credentials arista / arista123! 

Run the following: 

```
sudo dnf install -y python3.11 git
curl -sSL https://github.com/nathanmusser/avd-bootstrap/releases/download/v4.8.0/avd-bootstrap.sh | sh -s -- -p /usr/bin/python3.11 --install
cd ./avd; source venv_avd/bin/activate
git clone https://github.com/nathanmusser/act-inband-ztp-demo.git
cd act-inband-ztp-demo/
```

Login to CVP and watch the devices onboard. This process will take a while.
