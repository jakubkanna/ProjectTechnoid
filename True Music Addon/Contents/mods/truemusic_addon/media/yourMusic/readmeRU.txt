1. Видеоинструкция: https://youtu.be/b7SUjPzmgfM

2. Разместите файлы в формате mp3, wav, ogg в папках "TCBoombox" и "TCVinylplayer".

3. (опционально) Поместите виниловые обложки в папку TCVinylplayer в формате jpg. Они должны называться так же, как файл с музыкой. У каждого музыкального файла может быть своя обложка.
Например, файл с треком называется «AC DC - Highway To Hell (1979).mp3», файл с обложкой должен называться «AC DC - Highway To Hell (1979).jpg».
Самый простой способ найти обложку - это погуглить: "AC DC - Highway To Hell vinyl cover".

4. Запустите AddYourMusicToTheMod.exe. В зависимости от того, в какую папку помещены файлы, будет создана кассета или винил.

5. В файле mod.info измените ID на свой собственный 

6. Чтобы ваш мод не конфликтовал с другими аддонами True Music, вам необходимо переименовать файлы:

media\lua\server\Items\TCGLoadingTCBoombox.lua
media\lua\server\Items\TCGLoadingTCVinylplayer.lua
media\lua\shared\TCGMusicDefenitionsTCBoombox.lua
media\lua\shared\TCGMusicDefenitionsTCVinylplayer.lua
media\scripts\TCGMusicScriptTCBoombox.txt
media\scripts\TCGMusicScriptTCVinylplayer.txt
media\scripts\TCGSoundsTCBoombox.txt
media\scripts\TCGSoundsTCVinylplayer.txt

Например, добавьте к их названию Workshop ID вашего мода:
media\lua\server\Items\TCGLoadingTCBoombox2722332157.lua
media\lua\server\Items\TCGLoadingTCVinylplayer2722332157.lua
media\lua\shared\TCGMusicDefenitionsTCBoombox2722332157.lua
media\lua\shared\TCGMusicDefenitionsTCVinylplayer2722332157.lua
media\scripts\TCGMusicScriptTCBoombox2722332157.txt
media\scripts\TCGMusicScriptTCVinylplayer2722332157.txt
media\scripts\TCGSoundsTCBoombox2722332157.txt
media\scripts\TCGSoundsTCVinylplayer2722332157.txt

7. Отправить мод всем пользователям сервера (мы разрешаем вам публиковать мод созданный из шаблона).

8. Если вы хотите загрузить работу в Workshop, вам необходимо будет удалить папки и файлы:
\media\yourMusic\audioConverter
\media\yourMusic\pictureConverter
\media\yourMusic\AddYourMusicToTheMod.exe
\media\yourMusic\DeleteYourMusicFromTheMod.exe

-----------------

P.S. Если у Вас есть опасения по поводу запуска exe-файла, Вы можете изучить его исходный код (файлы AddYourMusicToTheMod.cs, DeleteYourMusicFromTheMod.cs) и скомпилировать его самостоятельно при помощи стандартного компилятора Microsoft .NET Framework (csc.exe).