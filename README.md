# k8s_auto_install
## 目標
* 減少安裝k8s複製貼上的次數

## 系統環境需求
* master branch
  * ubuntu 18.04.5 + k8s 1.22.0
* ub18.04_k8s1.22
  * ubuntu 18.04.5 + k8s 1.22.0

## 更新記錄
* 先SSH進要安裝的主機，因為.sh內很多操作都需要root權限，必須先sudo su
* 指令擇1： 
  * GitLab : wget http://192.168.168.131:8888/nine/k8s_auto_install/-/raw/master/install_k8s.sh
  * GitHub : wget https://raw.githubusercontent.com/CreatopNineWei/k8s_auto_install/78b89d28bc167eeb42d0bc9bf6b90b99d1e77191/install_k8s.sh
* 指令：/bin/bash install_k8s.sh
* 等待，收工