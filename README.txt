������������ �������� ������� Java ���� ����������������� ��������������.

� ������� ��� ������������ 11 ����������� ������.���� �� ������ ����� �� ����:
Plane.java , equipmentCompartment.java , planeComponent.java , cargoBay.java ,
privateCompartment.java , cleaningEmployee.java , maintenanceEmployee.java ,
securityEmployee.java , employee.java , passengerCompartment.java ����� ��� � main.java
��� ������������.
��� �� ������ ����� �� ��������� , ������ �������� ��� ������ �javac main.java� ��� ������
��� �� ��������� ��� ������� , �������� �java main� ��� ���������� �� ��������� ������������.

������ , �� ���� �� ������ , �� ��� ��������� ����� ��� �������� ������� ��� ���������� ��� , 
������ �� ��������� ��������� ��� ����������� ���� ���� ��� ��� ������� ��� ��� ���������� �� 
���� ��� ������.

�������� ������� :
������ , ��� �� ������ , ����� �� ����� ����� ��� ����� Object ��� ������� Java.
������ �� �� ��� , �������� ���� ������� ��� ����������� ��� Object �� ���� class "onomaclassis" extends Object
���� ������ ��� ������ ������� ��� ���� ��������� ����������.
������ ��� ����������� ���� ��� ��������.

��� ������ ��� abstract ����� planeComponent (���� �� ������� abstract �����������) ����� ���� ������
�� ����� , ���� ��� ���������� ��� ������������.
��� �������� ��� ������ ��� ����� �� ����� passengerCompartment � ����� ���������� ��� ����� planeComponet.
������ ���������� ��� ��������� ����� , ��� ������ ���� ������ ��� �� ���� extends planeComponent.
��� ���� ������� �� �� passengerCompartment ��������� ��� � ����� privateCompartment � ����� ����� ���������
��� ��� ������������ ���� ��� ���� ���.��� ����� privateCompartment ���������� , �� ��� ���� ������ � �����
cargoBay (extends privateCompartment) ��� � ����� equipmentCompartment(extends privateCompartment).

������ , ��� ������ ��� "�����" ��������� ����� employee ���� �� ��� ������ ��� ������� �����������.
��� ����� employee  ����������� , �� ������� securityEmployee(extends employee) , maintenanceEmployee(extends
employee) ����� ��� � ����� cleaningEmployee(extends employee).

������������ , ��� ������ ��� ��� ����� �����, �� ����� Plane � ����� , ���� ���������� ��� ����� Object ��� �������
Java ��� ����� ���� ��� ��� ��������������� ������� , ��� ���� �������� ��� ���� ������� ���� ��� ������ ��� 
������.

����� , ������� ��� � main ����� ��� ������������ , � ����� ��������� ����� ��� ���������� ��� ��������� ���
����� ��� ����������� ����������� ��� �� ���������� � �������� ��� �������� �����.


���� , �� ������� ��� ������ ��� ������� ��� �� ���������� ��� ����������� ��� ������� ���.

-������ planeComponent.java : ��� ������ ��� ����� planeComponent �� ��������� , ���� ����� ��������� ��� 
��� ��������.��� ������ �� ������� 1 �������� ������� ��������� , �� "�������" , ����� ��� 2 ���������� 
����������� ���� ��� ����� 2 �����������.
-������ passengerCompartment.java : � isSecured �������������� �� 0 ������ ��� ����� secured  � ��������� ����
 ��������� ��� ���� � ��������� ������� ���� �������� ���� ����������� �� �������� �� ����.�� ������� 
�����������,��� ��� ������� ���� �� ������������ , ���� ��� accessors ��� ����������� �� ������ ���� ��� 
����������.
-������ private Compartment.java : �� ���� �� ������ ��� ������ 3 ��������� ���������� ����� int ����� ��� 
6 ����������� ���� �� ��� ������,4 ����� & accessors 2 ����� �� ����������� ��� ������ � �������� �� 
������������ . ���� �� ����������� ��� ������� ����� ������� �� �������� ��� ���������� ��� ��������� ��� ������� 
������ ��� ������������.
-������ cargoBay.java Q: �� 3 ��������� ���������� ��� ��������� ��� �������������� �� ��� ����� privateCompartment ������ �����
 0 (��������������� ���� constructor), �������� (������ ��������� �� accessors ) ,���� ���� ��� workOn . ���� ���������� ,����� 
������� ��� �� ���������� accessors ��� ������ ��� ���������� ���������� �� ����� ��� ��� ������ �������� . ����� �������� 
��� � ��������� ready_check ,�  process � ����� ����� ��� workOn . ������ ������� ��� ��������� allOk � ����� ���������� ��� ���� �� �� 3
 �������� ���� ��� ���������� ����� ����� 1 (������ ���� ������ ��������� �� �������� �'����) .
-������ equipmentCompartment.java: ������ ������� �� ����� ����������� �� �� ������ cargoBay ���� ��� ���� �� ���� ������� �� ������
equipmentCompartment.

-������ employee.java: �� �������� ��� ����������� . ��� �������� ��������� �� �� ����� ��� ����� ��� 4 ����������� �� ��� ������ �� 3 
����� ���������� .
-������ cleaningEmployee.java : � ����������� ����������. �������� �� constructor � ������ ������� �� ������ ��� string ��� �� ��������� 
��� ����� name . ��� �������� ������� � ��������� report ��� ��������� ��� ���� ������ . ����� �������� �� ����������� workOn �� ������ 
��������� ��� �� 2 ���� ��� ���������� ��� ����� ��������� � ������������� �����������.
-������ maintenanceEmployee.java : � ����������� ����������. �������� �� constructor � ������ ������� �� ������ ��� string ��� �� ��������� 
��� ����� name . ��� �������� ������� � ��������� report ��� ��������� ��� ���� ������ . ����� �������� �� ����������� workOn �� ������ 
��������� ��� �� 2 ���� ��� ���������� ��� ����� ��������� � ������������� �����������.
-������ securityEmployee.java : � ����������� ���������. �������� �� constructor � ������ ������� �� ������ ��� string ��� �� ��������� 
��� ����� name . ��� �������� ������� � ��������� report ��� ��������� ��� ���� ������ . ����� �������� �� ����������� workOn �� ������ 
��������� ��� �� 3 ���� ��� ���������� ��� ����� ��������� � ������������� �����������.

-������ Plane.java : �� ���������. ����� ������� �� ������� private ���� ���� �� ����� , � ������������ ����� ������������ 
������ ��� �� ������� compartments.������ ��� ����� 2 ���������� �� ��������� �� ������ ���� ���� ��� ������� �������. � ������� passengerCompartmentNum
 ��� � ������� isReady � ����� ����������, �������������� �� 0 ��� ������� 1 ���� �������� � ��������� beready ��� ���������� ����������� �� �� ���������
 ����� ������ ��� ��������� 
. � constructor  ������� 2 ��������. ��� ����� (�� ������������  ) ����� ��� ��� ������������
(�� �������) . ������ ���� �� ���� ��� ���������� isReady=0 ��� ������ ������� ���� ������ �� 3 equipment compartments ���� �������� ��� ��� �������� �������
� ������� ��� passengerCompartment (passengerCompartmentNum)�� ���������� ������ ��� ���  ��������� ������� ������� ��� ������� Java. � ������� ����� ��� ��������
 �� ����� �������� 1<passengerCompartmentNum<5.���� �� ������� ��� ���������� ��� ����������� -����� .
� process ������� ������ ���� �������� ��� ����� ��� ����������� process ��� �� ���� ��� ����������(��� �� cargobay , ��� �� 3 equipmentcompartment ���
��� �� "�" passengerccompartment).
H beready ���������� ����� �� ready_check ���� ������� �� �� ���� ��������� . ���������� �������� �� �� ��� �� ���� ��� ���������� � �����������-����
(onomaMerous::allOk())  ����������� 1 , ����� ��� �� ���� ����� ������ , ��� �� ��������� ����� ������.��� � private ��������� ��� ��������� �� ����� 
isReady , ������� ��� 0 �� 1. � ready_check ����� ��� beready ��� ...���� ��������� � beready ��������� �� ��������� isReady ��� ������� �� �� ���� ���
������������ ���������� ������.
�������� 3  accessors ��� ����������� �� cargobay , ��� ������ equipmentcompartment ��� ��� ������ passengercompartment ��� 1 accessor ��� ���������� 
��� passengerCompartmentNum .

-������ main.java : � main ����� ��� ������������.


















