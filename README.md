# ansible-test-JDK8
- ansible playbook and templates for delete older and install new JDK, install nginx and share server ip address in index.html

Main task: 
---------------------------------
Есть сервер с ОС Linux, с системой управления пакетами RPM.
На нём установлена Oracle JDK 1.8 из RPM-пакета.
Необходимо:
1) С помощью Ansible обновить (т.е. удалить старую версию и установить новую) JDK до openjdk-17, взятую с https://openjdk.java.net/projects/jdk/17/ (с прописыванием системных путей к бинарникам в PATH).
2) Установить nginx текущей стабильной версии.
3) Создать файл index.html, в котором содержится IP-адрес сервера, на котором он находится. Для выяснения IP-адреса желательно использовать штатные средства Ansible.
4) Раздать данный файл через nginx.
----------------------------------


Now I'm upload first version. Work only for CentOS and don't change nginx.conf. Can make it if needed...
