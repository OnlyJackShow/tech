# 常用命令
## 防火墙和端口系列
* 查看防火墙状态
   
   ```systemctl status firewalld```
   
 * 开启防火墙命令
   
   ``` systemctl start firewalld  ```

 * 关闭防火墙命令
   
   ``` systemctl stop firewalld  ```
  
  * 重启防火墙命令
   
    ``` systemctl restart firewalld  ```
  
  * 查询已开放端口
 
    ``` firewall-cmd --list-all ```
  
  * 开放端口
  
     ```firewall-cmd --zone=public --add-port=5672/tcp --permanent```
  
  * 移除端口
  
     ``` firewall-cmd --permanent --remove-port=5672/tcp ```
  
  * 立即生效
  
    ```firewall-cmd --reload```
   
   * 安装网络工具
      
      ```yum -y install net-tools```
     
   * 查看端口被哪个应用占用
      
      ```netstat -lnp | grep 5672```
    
   
   * 创建文件夹
   
     ``` mkdir test1 ```
   
   * 创建文件 例如hello.txt
   
      ``` vi hello.txt ```
   
   * 拷贝文件
   
     ``` cp hello.txt test1```
     
   * 移动文件
   
     ```mv hello.txt test1``` 
     
   
