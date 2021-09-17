# k8s_auto_install
## 目標
* 減少安裝k8s複製貼上的次數

## 指定安裝版本
* master branch
  * ubuntu 18.04.5 + k8s 1.22.1 + crio 1.21

## 注意事項
* cat /etc/hostname 得到的name，要與cat /etc/hosts 中的127.0.1.1的name一致
* 先SSH進要安裝的主機，因為.sh內很多操作都需要root權限，必須先sudo su

## 操作流程
* 於SSH內下載；下載來源指令擇1： 
  * GitLab : wget http://192.168.168.131:8888/nine/k8s_auto_install/-/raw/master/install_k8s.sh
  * GitHub : wget https://raw.githubusercontent.com/CreatopNineWei/k8s_auto_install/78b89d28bc167eeb42d0bc9bf6b90b99d1e77191/install_k8s.sh
* 指令：/bin/bash install_k8s.sh
* 等待，收工