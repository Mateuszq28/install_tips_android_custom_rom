# Recenzja softu
*crDroidAndroid-14.0-20240819-ginkgo-v10.7*
*Xiaomi Redmi Note 8T*
Matiz - udało się zainstalować. Nie działają tapety, bo nikki gapps mi nadpisało luncher i tapety? A tak ogólnie to a początku byłem zachwycony. Potem wszystko wróciło do normy, to znaczy telefon tnie się jak cholera. No ale i tak ma już 5 lat. Odinstalowałem część apek, wymusiłem zakończenie pracy i przestawiłem na "disable" w ustawienia/apps i jest trochę lepiej - podobno trzeba tak zamykać apki, to telefon lepiej chodzi. Ogólnie szału nie ma. Następnym razem spróbowałbym wersję Nikki Gapps najmniejszą (core) zamiast "Stock".

# Pliki
1. *info_mm.md* - ten plik
2. *'Install Official crDroid.mp4'* - lepszy tutorial, ale bez unlock
3. *'How to Root Magisk using TWRP.mp4'* - gorszy tutorial
4. *crDroidAndroid-14.0-20240819-ginkgo-v10.7.zip* - plik z systemem crdroid (dla Redmi Note 8T), nie trzeba rozpakowywać
5. *NikGapps-full-arm64-14-20241231-signed.zip* - aplikacje googla w wersji rozszerzonej - pełen pakiet
6. *NikGapps-core-arm64-14-20250127-signed.zip* - tylko niezbędne pliki do działaniu Google Play
7. *nikgapps.config* - plik konfiguracyjny do instalowania Gapps, można sobie wybrać, które chce się zainstalować
8. *RO2RW-StableBeta.v3.7.2.1.zip* - to miało być niezbędne do zainstalowania sklepu Google, ale jednak okazało się niepotrzebne
9. *'OrangeFox-ginkgo-stable@R11.1.zip'* - TWRP, tylko lepsze, potrzebne żeby sflashować system na telefon
10. *'OrangeFox-ginkgo-stable@R11.1'/*
11. *platform-tools-latest-windows.zip* - rozpakować i dodać do ścieżki (path), są to narzędzia do obsługi telefonu po kablu, najważniejsze to adb
(update) właściwie to nawet nie trzeba dodawać do ścieżki. Można operować z poziomu folderu, w którym są te narzędzia.
12. *platform-tools-latest-windows/*
13. *Qualcomm_USB_Driver_v1.0.10065.1.zip* - sterownik Qualcomm (wybiera się w zależności od procesora telefonu, żeby komunikować się komendami w terminalu po kablu z telefonem). Rozpakować i zainstalować.
14. *Qualcomm_USB_Driver_v1.0.10065.1/*
15. *miflash_unlock-en-6.5.224.28.zip* - oryginalny program ze strony xiaomi do odblokowywania telefonu
16. *miflash_unlock-en-6.5.224.28/*
17. *XMT2_Win_Setup_20.7.28.zip* - open source program do obsługi xiaomi, jeśli jest problem z widocznością telefonu w trybie fastboot, to ten program pobierze potrzebne sterowniki i umożliwi połączenie
18. *XMT2_Win_Setup_20.7.28.exe*

# CrDroid strona
https://crdroid.net/downloads#google_vignette
https://crdroid.net/ginkgo/10
Forum XDA

# Aplikacje Google
https://nikgapps.com/
(na stronie crDroid też jest link od razu przy obrazie systemu)

# Działania do wykonania
*Xiaomi Note 8 (Ginkgo) & Note 8T (Willow) : Tutorial Howto Root Magisk using TWRP*
**'How to Root Magisk using TWRP.mp4'**
[hindus - ten sam model](https://www.youtube.com/watch?v=N_TbR2elBCE&t=101s)
*Install Official Android 14 crDroid ON Redmi Note 12 4G English*
**'Install Official crDroid.mp4'**
[inny model - z tego korzystałem i akcja zakończyła się sukcesem](https://www.youtube.com/watch?v=2t71pAggh1U&t=259s)

#
1. Włączyć debuggowanie USB i OEM unlocking
2. podłączyć telefon, otworzyć terminal i wpisać
adb reboot bootloader
3. włączyć miflash_unlock
zalogować się
kliknąć Unlock
czasem trzeba czekać ileś godzin, np ja musiałem czekać 168 h



skopiować recovery?

fastboot flash recovery recovery.img
fastboot reboot
od razu po tej komendzie przytrzymuję volume up na telefonie