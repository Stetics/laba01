# laba01

Скачивание и распаковка `(wget "ссылка" & tar -xf boost_1_69_0.tar.gz)`
 )`

![image](https://user-images.githubusercontent.com/91694520/155757040-900b25a9-b860-4efb-bad6-6234e87d004d.png)


количество файлов, не включая вложенных папок

![image](https://user-images.githubusercontent.com/91694520/155758691-a3b14310-6360-424b-b51f-bcb785793e6a.png)

Включая вложенные папки `(tree boost_1_69_0)`:


![image](https://user-images.githubusercontent.com/91694520/155759105-317f056b-85d0-46d4-91d0-0eb4c1d0c0f0.png)


4. подсчет с расширением ".cpp" `(tree boost_1_69_0 -P "*.cpp")`


![image](https://user-images.githubusercontent.com/91694520/155759669-10c0651d-42d4-4ad2-a877-d55d6b00fd18.png)


5. Количество без ".cpp" & ".hpp" `(tree boost_1_69_0 -I "*.cpp|*.hpp")`

![image](https://user-images.githubusercontent.com/91694520/155760272-3066a94b-7a2d-4cae-b19f-f5fa297a9aeb.png)

6. поиск и вывод полного пути `(find ./boost_1_69_0 -name "any.hpp")`

![image](https://user-images.githubusercontent.com/91694520/155761040-70f1f9d2-b515-4a42-acaa-d5717b32d559.png)


7. все файлы содержащие "boost::asio" `(grep -rL "boost::asio)`

![image](https://user-images.githubusercontent.com/91694520/155762486-def64fd7-0070-4a05-8f86-44da64e53fa7.png)




