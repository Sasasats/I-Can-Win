# I-Can-Win

1. Установите git и сгенерируйте пару ssh ключей. Авторизуйте публичный ключ на github.com.
1.1. winget install --id Git.Git -e --source winget
1.2. ssh-keygen -t rsa -C andreysats.v@gmail.com
1.3. cd .ssh
1.4. vi id_rsa.pub

2. Укажите свой user.name и user.email в git.
2.1. git config --global user.name "Andrey Sats"
2.2. git config --global user.email "andreysats.v@gmail.com"

3. Создайте новый репозиторий на github.com и склонируйте его локально на свой компьютер.
3.1 git clone git@github.com:Sasasats/I-Can-Win.git

4. Создайте файл названием song.txt и поместите туда половину текста любимой песни.
4.1 touch song.txt
4.2 echo "half of the lyrics of my favorite song" > song.txt

5. Сделайте коммит с названием "add first half of my favorite song" и отправьте его на сервер.
5.1 git add song.txt
5.2 git commit -m "add first half of my favorite song"
5.3 git push

6. Убедитесь что на github есть файл song.txt с текстом песни.

7. Используя веб-интерфейс гитхаба добавьте вторую половину текста песни и сделайте коммит с названием "finish my song".

8. В локальном репозитории сделайте pull и убедитесь что коммит, который вы создали на github, подтянулся и у вас полный текст песни.
8.1 git pull
8.2 vi song.txt
