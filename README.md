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


7. все файлы содержащие "boost::asio" `(grep -rl "boost::asio")`

![image](https://user-images.githubusercontent.com/91694520/157916815-7acba213-4aca-4fe3-a46f-0249f29e75cd.png)


8. Компиляция boost `(./bootstrap.sh + ./b2)`

![image](https://user-images.githubusercontent.com/91694520/156928782-33eb7b60-33ed-4bd0-a395-692615fca86d.png)

![image](https://user-images.githubusercontent.com/91694520/156928824-f9fe1d8b-23d2-4d89-883b-5ccc60bb4ef1.png)


9. Перенос всех скомпилированных на предыдущем шаге статических библиотек в директорию ~/boost-libs. `( mv stage/lib/ ~/boost-libs

![image](https://user-images.githubusercontent.com/91694520/156929605-3fd25fde-f7cb-4895-96f1-31bb1268ec65.png)


10. Подсчёт дискового пространства `(du -a)`

![image](https://user-images.githubusercontent.com/91694520/156930277-436c6f47-94ac-425d-b680-92da0900dc08.png)


11. Вывод 10 самых тяжелых файлов в текущей директории `(du -ahx . | sort -rh | head -5)`

![image](https://user-images.githubusercontent.com/91694520/156930387-3924499d-3558-49a3-a4d1-bebe5244f1c2.png)




