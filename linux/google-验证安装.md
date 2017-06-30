# Google身份验证器二次验证Ubuntu
* 在Ubuntu安装google-authenticator：运行“sudo apt-get install libpam-google-authenticator”。

* 手机安装google-authenticator，二维码扫描验证设置。

* 设置Ubuntu登陆时加载google-authenticator：运行“sudo vi /etc/pam.d/sshd”，在最后加一行“auth required pam_google_authenticator.so”；运行“sudo vi /etc/ssh/sshd_config”，找到“ChallengeResponseAuthentication”这行，改成“ChallengeResponseAuthentication yes”。

* 重启SSH：“sudo service ssh restart”。

* 再次登陆时，输入帐号密码登陆之外，还要输入google-authenticator的6位验证码。
