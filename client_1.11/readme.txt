1. ��� ������ ������ ����������, ����� ���� �����������:
 - JDK1.7_05;
 - Maven 3.*;
 - CryptoPro JCP 1.0.5*.

2.	������ ������ ������� ����

������ ��������� ��� ������ � �������������:
  a) ������� � ����� crypto 
  b) ��������� mvn install

������ �������:
  a) ������� � ����� client
  b) ��������� mvn install


������ �������������� ����������� ������� �mvn install� � ����� code_new
� ���������� � ����� code_new\modules\smev-client\target\ � ��������� maven-����������� �������� ���� smev-client-*.jar

3.	����������� ������ ������� � maven-������

��� ����������� ������ ������� ��������� � pom.xml �����������
<dependency>
	<groupId>ru.it.smev</groupId>
	<artifactId>smev-client</artifactId>
	<version>${project.version}</version>
</dependency>

4.	������ �������������
��� ��������/��������� ��������� ���������� �������� ������ ������ MessageExchangeEndpoint, ��������:
MessageExchangeEndpoint.getInstance().sendRequest(messageID, content, personalSignature, null, attachmentList);

����� sendRequest() ���������� ��������� � ����, ���
messageID � ID ���������, 
content � ������ �� ���� ���������
personalSignature � ������� ��������� ��-��
attachmentList � ��������

� ����� example ����� ����� ����������, ��������������� ����� ������� ������. ���� ��� ��������� � ����� Example.java. �� ���� ���� ���������� �����������.
����� �������� ���������� ���������� ��������� � ������ ���� � ����� ����, ��� ���������, ��������� ������.
��������� ����� ������ ���� ����������� � CryptoPro JCP.

