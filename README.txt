git ʹ�÷���

1 ע��github�˺�

2 ����git�ͻ��� gitbash

3 mkdir /d/opt/repository�������زֿ�   git init����git�����ļ�

4 git��github֮��Ĵ�����ͨ��SSH���ܵģ����Ե�һ�����ڱ�������һ.ssh   cd ~/.ssh  �Ȳ鿴�����Ƿ���.ssh�ļ����еĻ�ɾ��

5 �����������.ssh��д���Լ�������   ssh-keygen -t rsa -C "your email@.com"

6 Ϊ�˱�����github��������ʱ���������½�һ��config�ļ��������´��븴�ƽ�ȥ   Host github.com
    User git
    Hostname ssh.github.com
    PreferredAuthentications publickey
    IdentityFile ~/.ssh/id_rsa
    Port 443


7 ��id_rsa.pug�����ݸ��Ƶ�ָ��λ��  ͷ��  setting  ssh and gpg keys 

8 ���������Ƿ�ɹ�����ͼ��ʾ���ʳɹ�	ssh -t git@github.com

9 �ϴ���Ŀ git add <�ļ���>   git commit -m "first commit" 

   git remote add origin git@github.com:zhengyp/Myproject.git

   �������  git remote rm origin �������һ��

10 git push -u origin master

11 �����ļ� git add readme.txt  git commit -m "�Ż�������"   git push -u origin master 

12 ��ʼѧϰ��֧��ز���