> ��֧��dubbo2.7��汾
## �����ܵ�����
���Զ������У����dubbo�ӿڽ���mock�Ŀ��

## ԭ��
����dubbo����չ���Զ���װ��ͨ��EasyMockClusterWrapper��ԭ����rpc�����дΪhttp����ת����mock�������������Ƕ�Ӧmock���

![](img/principle.jpg)

## ʹ��
1. �������
mvn clean package install -Dmaven.test.skip=true
```xml
<dependency>
        <groupId>io.github.shengchaojie</groupId>
        <artifactId>dubbo-easy-mock</artifactId>
        <version>1.0.0-SNAPSHOT</version>
    </dependency>
```

2. classpath����mock.properties
```
## �Ƿ�����mock
easymock.enable=true
## mock��������ַ
easymock.server.url=https://easy-mock.com/mock/5c77afd53ecfbb573cba5df8/test
## �ӿڼ���mock���� 
easymock.tests.HelloService=true
## ��������mock����,���ȼ����ڽӿڼ���
easymock.tests.HelloService.hello=true
```

3. mock����-����Լ��
