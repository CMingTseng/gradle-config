### 1��compile,?provided,?apk
��`File��Project?Structure��Dependencies`������
http://stackoverflow.com/questions/28472785/compile-provided-apk-android-dependency-scope

#### compile?�������ʹ��
1.**compile**
???���е�*build_type*�Լ�*flavors*������벢�Ҵ����apk��ȥ������ʱ��Ҫ��
*?`compile?fileTree(include:?'*.jar',?dir:?'libs')`??������libs�����е�jar��
*?`compile?files('libs/picasso-2.4.0.jar')`?������picasso-2.4.0.jar��
*?`compile?project(':common')`?������common?module

1.?**debugCompile**
???����debug��flavors������벢�Ҵ����apk��ȥ


2.?**releaseCompile**
???����release��flavors������벢�Ҵ����apk��ȥ


3.?**testCompile**
???��������Ե�Ԫ���Դ���ı�������Լ����մ������apkʱ��Ч������������debug����release?apk���������á�


4.?**xxxCompile**
???����xxx��flavors������벢�Ҵ����apk��ȥ,��releaseLogCompile

####?provided?ֻ������벻������
Provided�Ƕ����е�build?type�Լ�favlorsֻ�ڱ���ʱʹ�ã�����eclipse�е�external-libs,ֻ������룬�����������apk��

####?apk?ֻ���������������
ֻ������apk�ļ��У�����������룬���Բ����ٴ�����ֱ�ӵ���jar�е���򷽷��������ڱ���ʱ�ᱨ��