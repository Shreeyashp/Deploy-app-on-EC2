# How to Deploy Streamlit app on EC2 instance

## 1. Login with your AWS console and launch an EC2 instance

## 2. Run the following commands

### Note: Do the port mapping to this port:- 8501

```bash
sudo apt update
```

```bash
sudo apt-get update
```

```bash
sudo apt upgrade -y
```

```bash
sudo apt install git curl unzip tar make sudo vim wget -y
```

```bash
sudo apt install git curl unzip tar make sudo vim wget -y
```

```bash
git clone "Your-repository"
```

```bash
after cloning go into your repository by cd and use ls, after that u will see that there is no .env file
so create .env file by command touch .env , but .env file is hidden file so cant see that, so to check .env file use ls -al to check it
now open it by command vim .env, now whatever credential is present in .env file in vscode copy all that & paste it.
now press esc button and then shift clone afterthat at bottom there will be one white tab blinking so type :wq or ZZ (Shift + ZZ)
to check .env use commant cat .env
```

```bash
sudo apt install python3-pip
```

```bash
pip3 install -r requirements.txt
```

```bash
#Temporary running
python3 -m streamlit run app.py
```

```bash
#Permanent running
nohup python3 -m streamlit run app.py
```

```bash
after running all these commands u will get url but after accessing it will not run 
so go in ec2--> security-->click security group-->edit inbound rules--> add 8501 port
now add 8501 in ur url and then trigger 
```
Note: Streamlit runs on this port: 8501



