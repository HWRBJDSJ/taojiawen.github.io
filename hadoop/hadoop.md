# ����hadoop�ֲ�ʽ

### ׼������

����� hadoop �û� visudo

yum install -y (vim net-tools)

/home/hadoop ���� hadoop.gz jdk.gz

systemctl stop firewalld

��Ϊnamenode

��¡������Ϊdatanode

### ��ʼ����

����namenodeΪα�ֲ�ʽ������һƪ
[�����](http://taojiawen.github.io/hadoop/config)

vim ~/hadoop-2.7.3/etc/hadoop/slaves
����datanode ip��ַ

datanodeͬ������Ϊ���ڵ�hadoop
ֻҪ datanode ·���� namenode һ�� ����
scp -r �봫���ļ� �û���@ip��ַ:Ŀ���ַ
��namenode�����ô���DataNode

sudo vim /etc/hosts ��ip namenode ip datanode(datanode������Ҫ��ͬ) д��

��ʱ�Ϳ�����namenode����datanode��dfs��yarn ������Ҫ������������

so
ssh-keygen������Կ(���̻س�����)
ssh-copy-id �û���@IP��ַ �ѹ�Կ����datanode
ssh-copy-id localhost ���ñ�������
�������Ѿ����ɲ�׷�����

ps
authorized_keys:���Զ�����ܵ�¼�Ĺ�Կ,��Ҫͨ������ļ���¼��̨�����Ĺ�Կ
id_rsa : ���ɵ�˽Կ�ļ�
id_rsa.pub �� ���ɵĹ�Կ�ļ�
know_hosts : ��֪��������Կ�嵥

![1.jpg](https://upload-images.jianshu.io/upload_images/14465950-db7a7be76e591951.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

 




