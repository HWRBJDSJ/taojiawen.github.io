# Linux �û�

## �����ļ�

- �����û���Ϣ���ļ���/etc/passwd	
- ����������ļ���/etc/shadow
- �����û�����ļ���/etc/group
- �����û���������ļ���/etc/gshadow
- �û������ļ���/etc/default/useradd

## �û���ϵͳ���Ƿ�Ϊ��ɫ�ģ�ͨ��UID��ʶ���ɫ

	root�û���ϵͳΨһ�����Բ���ϵͳ�κ��ļ������ӵ�����Ȩ�ޣ�UID=0 
	�����û�(ϵͳ�˻�)�������е�¼ϵͳ��������ȴ��ϵͳ���в���ȱ�ٵ��û����磺bin��daemon��ftp��mail�ȣ�UIDΪ1---499֮��
	��ͨ��ʵ�û������Ե�¼ϵͳ��Ȩ�����ޣ�������Ա������UIDΪ500��60000֮��

## ϵͳ�˻�

- 1 �C 99����distributions���д�����ϵͳ�˺�
- 100 �C 499�����û���ϵͳ�˺�����ʱ������ʹ�õ�UID

### Ϊ�˸��õĹ����û���������group�ĸ���

	�����飨˽���飩 ���û������ļ����ļ���ʱ��Ĭ������˽����
	�����飨�����飩

# �û�����

## �û����������ļ�

### �û��˺��ļ�--/etc/passwd

![TIM��ͼ20181018212652.png](https://upload-images.jianshu.io/upload_images/14465950-55fd4b1d6bd150af.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
	
### �û������ļ�--/etc/shadow

![TIM��ͼ20181018212830.png](https://upload-images.jianshu.io/upload_images/14465950-6b6c32df1a1ae3c2.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

## �û���������

### useradd ����û�����

- -u ָ����ID��uid��
- -g ָ��������������gid��
- -G ָ������飬�ö��š������ֿ���Groups��
- -c �û�������comment��
- -e ʧЧʱ�䣨expire date��

### passwd ��������

- -d������û������룬ʹ֮�������뼴�ɵ�¼
- -l�������û��ʺ�
- -S���鿴�û��ʺŵ�״̬���Ƿ�������
- -u�������û��ʺ�
- -x:    �������ʹ��ʱ�䣨�죩
- -n:    ��С����ʹ��ʱ�䣨�죩

### usermod �޸������û�����

- -l �޸��û��� ��login��usermod -l a b��b��Ϊa��
- -g ����� usermod -g sys tom
- -G��Ӷ���� usermod -G sys,root tom
- �CL �����û��˺����루Lock��
- �CU �����û��˺ţ�Unlock��

### userdel ɾ���û�����
 
- -r ɾ���˺�ʱͬʱɾ��Ŀ¼��remove��

# �����

## ����������ļ�

### �û����ļ���/etc/group

![TIM��ͼ20181018213530.png](https://upload-images.jianshu.io/upload_images/14465950-79f4784095090891.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

### �û��������ļ��� /etc/gshadow

![TIM��ͼ20181018213625.png](https://upload-images.jianshu.io/upload_images/14465950-ef96b6e3c26003df.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

## ���������

### groupadd ������˺�

-g ָ��gid
 
### groupmod �޸���

- -g��������Ҫʹ�õ�GID
- -o��ʹ���Ѿ����ڵ�GID
- -n��������Ҫʹ�õ�Ⱥ������

### gpasswd �������ʺ����루�����ã������/ɾ�����Ա

- -a�����������һ���û�
- -d��������ɾ��һ���û���Ա
- -M���������Ա�б��Զ��ŷָ�

### groupdel ɾ�����˺�

	 ע�⣺ֻ��ɾ����Щû�б��κ��û�ָ��Ϊ������顣
		   ��ʾ�û�������

### groups �鿴��ǰ��

		   