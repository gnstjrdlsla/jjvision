# 전주비전대 Project

## Install DHT11 sensor
```
git clone https://github.com/adafruit/Adafruit_Python_DHT.git
cd Adafruit_Python_DHT
sudo Python setup.py install
cd Adafruit_Python_DHT/examples
```
  - run
  ```
  python AdafruitDHT.py 11 4
  ``` 
  
# InflusDB Installation

## 1. Repository의 GPG KEY를 더하기
```
curl -sL https://repos.influxdata.com/influxdb.key | sudo apt-key add -
```
## 2. Repository를 더하기
```
echo "deb https://repos.influxdata.com/debian stretch stable" | sudo tee /etc/apt/sources.list.d/influxdb.list
```
## 3. 프로그램 설치
```
sudo apt update
sudo apt install influxdb
```
## 4. 프로그램 실행
```
sudo service influxdb start
```
## 5. 데이터베이스 만들기
```
>create database<데이터베이스이름>
```
```
확인: show databases
```
# Grafana Installation

## 1. Repository의 GPG key를 더하기
```
curl https://bintray.com/user/downloadSubjectPublicKey?username=bintray | sudo apt-key add -
```
## 2. Repository를 더하기
```
echo "deb https://dl.bintray.com/fg2it/deb stretch main" | sudo tee -a /etc/apt/sources.list.d/grafana.list
```
## 3. 프로그램 설치
```
sudo apt update
sudo apt install grafana
```
## 4. 프로그램 실행
```
sudo service grafana-server start
```
## influxdb import with python
```
sudo pip install influxdb
```
### Git Hub 사용방법
  -Repository down load
```
git clone https://github.com/<username>/<repository name>
```
### Vim 설정
```
set nu = 글자 앞에 번호 출력
set cindent = C언어 사용할때
set ts=<숫자> = Tap키를 누르면 숫자만큼 띄어쓰기
if has("syntax")
    syntax on
endif = syntax를 가진 파일이면 syntax 기능을 사용(컬러를 준다)
```
