# ��ν����� git �ֿ�ͬ�����͵�Զ�̵� gitee �� github �ֿ�

Windows 10 �½����زֿ����͵����Զ�ֿ̲ⷽ���ܶ࣬���γ������Ƽ�2�ַ�����
�����ڱ��γ̵�ʵ����Ϸֱ���������ַ�����������Ӧ��ʵ�����д��ʵ�鱨�档

�ڽ��������ʵ��֮ǰ����Ҫ���� gitee �� github �Ϸֱ𴴽�һ���ֿ���ͬ���㱾�زֿ��е����ݡ�
��Ϊ�������ֿ���Ӻ���Կ��������ͬ���μ�[ʹ�� ssh-key](ssh_gitee.md)�����Ա㽨�� SSH ������������Ӧ��Զ�ֿ̲⡣
�������Ǽ������������õ������ֿ�ֱ�Ϊ��
1. https://gitee.com/someone/some_repo.git
2. https://github.com/someone/some_repo.git

## 1 ʹ�������й���

�����ʹ�� Win10 �Դ��� Windows PowerShell ���� Visual Studio �Դ��� Developer PowerShell.
�� Developer PowerShell �����ַ�ʽ��
1. ����˵��� View��Ȼ���� Terminal
2. ����˵��� Tools��Ȼ���� Command Line�����ŵ�� Developer PowerShell

���������½���Ҫ���͵ı��زֿ����ڵ��ļ���
(�����ʹ�� Developer PowerShell �ҵ�ǰ VS ���򿪵��ļ��о��Ǳ��زֿ����ڵ�λ��, ���������µ�·���Զ�����Ҫ���͵ı��زֿ�)��
�������� git status �鿴һ�µ�ǰ��״̬��

���� gitee �� github Զ�ֿ̲⣨��Ҫ�����زֿ����͵��������ֿ⣩
```shell
git remote add origin_gitee https://gitee.com/someone/some_repo.git
git remote add origin_github https://github.com/someone/some_repo.git
```
��������Ϊ���زֿⴴ����������Զ�ֿ̲�����ӣ����ֱַ�Ϊ origin_gitee �� origin_github 
(��Ҳ����ȡΪ��������, ��ͨ��ȱʡ������Ϊ origin)��

������ɱ��ص� commit ����Ϳ�����Զ�ֿ̲� push �ˡ������ص�ǰ��֧���͵� gitee �ϵ� master ��֧:
```shell
git push -u origin_gitee master
```

�����ص�ǰ��֧���͵� github �ϵ� master ��֧:
```shell
git push -u origin_github master
```
���ҽ�����ʵ����̷ֱ��ͼ��������ͼ��ӵ����ʵ�鱨���С�


## 2 ʹ�� VS �е� Team Explorer ���湤��

��ʹ�� VS �� Open Folder ���㱾�زֿ����ڵ�Ŀ¼��Ȼ��� Team Explorer �������(��� View ���ٵ�� Team Explorer)��
��� Home ���ٵ�� Setting, ���� git ��ǩ�µ�� Repository Settings ������������µĽ��棺

![repository settings](images/repo_settings.PNG)

����·�����ɫ�� Add Ϊ���زֿⴴ����Զ�ֿ̲�����ӣ������ҷֱ𴴽��� origin �� gitee��origin_github �� github����
�����ͨ�� Edit ���޸�, ͨ�� Remove ��ɾ����Զ�ֿ̲�����ӡ�

���ӽ����ú����ǾͿ���ѡ�񽫵�ǰ�ύ���͵���ͬ��Զ�ֿ̲⡣��� Home ���� Sync ���������½��棺

![repository sync](images/home_sync.PNG)

�ٵ�� Push �ұߵ����������Σ���ʱ����Զ�ֿ̲����ӵ�ѡ����棬����ѡ��ͬ��Զ�ֿ̲����Ӽ���֧:

![push to remote](images/push_remote.PNG)

��ͼ��ѡ����� origin_github���ٵ�� Push �Ϳ��Խ������ύ���͵���ѡ���Զ�����Ӽ���ѡ��֧��
���Ҫ�ύ��������ͬ��Զ�ֿ̲⣬�����ѡ��� Push ��Ҫ�ֱ������Σ�

���ˡ�Զ�ֿ̲�ͬ��ʵ��͵�����������������κ����⣬�뽫�����ͼ����������Ľ������һ��д�����ʵ�鱨�档


