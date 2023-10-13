хранятся основные команды на линукс: 
cd .. — перейти в директорию уровнем выше.
cd ../.. — перейти в директорию двумя уровнями выше.
cd — перейти в домашнюю директорию пользователя.
cd ~user_name— перейти в домашнюю директорию пользователя user_name.
cd - — перейти в директорию, в которой находились до перехода в текущую директорию.

mkdir — создать директорию.
touch — создать файл.
cp — копировать файл или директорию.
mv — переместить файл или директорию.
rm — удалить файл или директорию.

Чтобы удалить директорию с именем dir1 и рекурсивно всё ее содержимое, наберите: rm -r dir1
Чтобы переименовать файл, выполните команду или директорию: mv название_файла новое_название
Чтобы переместить файл или директорию, используется команда: mv название_файла путь/

Копировать директорию dir1 в директорию dir2: cp -a dir1/ dir2/
Копировать файл с именем file1 в директорию c именем dir1: cp file1 dir1/

more — постраничный вывод файла только вперед.
less— постраничный вывод файла вперед и назад.
head— просмотр файла с заданным количеством строк с начала.
tail — просмотр файла с заданным количеством строк с конца.
cat — просмотр всего файла.

Чтобы найти слова во всех файлах с расширением .txt, введите команду:
grep слово *.txt
Команда grep "Chrome" *.txtизвлечет все предложения, содержащие слово Chrome, из всех файлов с расширением .txt
.Можно игнорировать регистр строки поиска и выводить результаты поиска на основе этой строки с помощью опции 
-i: grep -i слово *.txt
Команда grep -i "Chrome" *.txt извлечет все предложения, содержащие строку "Chrome", из всех файлов с расширением .txt
. При этом не будет учитываться, в верхнем или нижнем регистре была строка поиска.
Чтобы найти строки, содержащие выражение, начинающееся и заканчивающееся определенным словом, поможет команда:grep "слово1.*.слово2" file
Команда выведет предложение, содержащее выражение, которое начинается с "слово1" и заканчивается на "слово2" из файла, который указан в команде 
grep.

whoami— узнать имя текущего пользователя.
useradd -m user1— создать юзера user1 с домашней директорией.
userdel –r user1— стереть юзера user1 с его домашней директорией.
passwd user1— изменить пароль для юзера user1.
groupadd Developers — создать группу Developers.
groupdel Developers— стереть группу Developers.
usermod –aG Developers user1— добавить юзера user1 в группу Developers.
deluser user1 Developers— удалить юзера user1 из групы Developers.

r — чтение;
w — запись;
x — исполнение.

sudo dpkg -i -уставнока пакета 
history - история всех запросов 

русификация мазилы:
sudo apt update && sudo apt install firefox firefox-locale-ru

