#sed����

###��ʽ:sed ѡ�� ���� filename

###ѡ��

	 -n (ʹ�ð���(silent)ģʽ����������вŻ��������д�ӡ)

###����

- a ����һ������
![TIM��ͼ20181022191629.png](https://upload-images.jianshu.io/upload_images/14465950-8d3310f411f2a7fb.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
- i	����һ������
	�÷���a����
- c �滻(1,5c�Ὣ��һ�����������滻������ÿ�ж��滻) 

![TIM��ͼ20181022192711.png](https://upload-images.jianshu.io/upload_images/14465950-64c6ea4e8813ff98.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

- d ɾ��

![TIM��ͼ20181022110522.png](https://upload-images.jianshu.io/upload_images/14465950-18293410c4bd731a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

- p ��� (��� -n һ��ʹ��)
- w д�� sed 'w Ҫ��д����ļ�(Ŀ���ļ�)' ��ȡ���ݵ��ļ�(Դ�ļ�)ֻҪ��w���ļ�
	�н���д��ͻὫĿ���ļ�֮ǰ������ȫ���ɵ�
- r ��ȡ sed '2r Ҫ��ȡ���ļ�' �������ݵ��ļ�(Ŀ���ļ�)

- s �滻�������������в���

![TIM��ͼ20181022111819.png](https://upload-images.jianshu.io/upload_images/14465950-602a09a2072d7c33.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

- �߼�����
	 | �ܵ���,ʹ�ø÷��������������
	 {} ������sedִ�ж������,ֻ�Ƕ���֮��Ҫ��";"�ֺŸ���
	 &�滻 
 	 &�൱��ռλ�������� �������� s/��ѯ����/��ѯ��������
	 ������s/��ѯ����/Ҫ�滻�ɵ������н���ʹ��,ʵ��׷�ӵ�Ч��
	 \uת�ɴ�д����������ǵ�&��ʵ�ֽ�ƥ������ת���ɴ�д�Ĳ���
	 
![TIM��ͼ20181022114542.png](https://upload-images.jianshu.io/upload_images/14465950-fac7da2c2f3adebd.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
	 
	 ()���鹦��
	 ��ȡ���������
	 ���ȷ��������Ǵ�1��ʼ�Ĳ��Ұ��մ����ҵ�˳���ŵ�
	 Ҫ��ȡʹ��\������������ȡ,����\1����ռλ��
	 
![TIM��ͼ20181022141939.png](https://upload-images.jianshu.io/upload_images/14465950-0307d235885b9e42.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

