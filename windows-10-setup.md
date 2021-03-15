# Windows 10: disabling trackers and removing default applications

1. Checking Windows for latest updates (Settings - Updates & Security - Check for updates). If there are updates available, install them.
2. Select 'Delivery Optimization' tab (left side) and make sure to switch off the 'Allow download from other PC's' parameter.
3. Click 'Windows + R' buttons on the keyboard and type in the dialogbox 'services.msc'. Press 'Enter'.
4. In the Services window search for 'Connected User Experiences and Telemetry' option. Double click on the option, change 'Status type' to 'Disabled' and 'Service status' to 'Stop'. Click 'Apply' and 'OK'.
5. Search for 'Windows update' option. Select the same properties as in step 4.
6. Download and install 'Windows Update Blocker application' -  [https://www.sordum.org/9470/windows-update-blocker-v1-6/](https://www.sordum.org/9470/windows-update-blocker-v1-6/)
7. Open 'Windows Update Blocker' application as Administrtor. Select an option 'Disable updates', mark the 'Protect Services Settings' checkbox and click on 'Apply Now' button.
8. Download 'Windows10Debloater' repository from Github (Code - Download ZIP) - [https://github.com/Sycnex/Windows10Debloater](https://github.com/Sycnex/Windows10Debloater)
9. Unzip the downloaded archive on the Desktop.
10. Open Powershell as Administrator and navigate to home directory ```cd ~```.
11. Navigate to Desktop directory ```cd Desktop```.
12. Type the command ```Set-Executionpolicy unrestricted```.
13. Navigate to Windows10Debloater-master ```cd Windows10Debloater-master``` and run ```Windows10Debloater.ps1``` script.
14. Click 'Yes' on the most of the pop-up windows, except for the last one - 'Reboot'. Click 'No' when asking to reboot.
15. Navigate to Settings - Privacy - General. Switch all options to 'Off'.
16. Switch all options to 'Off' also for tabs 'Speech', 'Inking & typing personalization', 'Diagnostics & feedback', 'Activity history', 'Location', 'Background apps', 'App diagnostics'.
17. Restart the computer.

## Настройка Windows 10: отключение трекеров и удаление дефолтных программ

1. Проверяем Windows на наличие обновлений (Параметры - Обновление и безопасность - Проверить наличие обновлений). Если есть обновления, нужно их установить.
2. Во вкладке "Оптимизация доставки" (находится слева) меняем параметр "Разрешить загрузки с других компьютеров" на "Откл.".
3. На клавиатуре нажимаем 'Windows + R' и в диалоговом окне вводим 'services.msc'.
4. Ищем строку "Connected User Experiences and Telemetry («Функциональные возможности для подключенных пользователей и телеметрия»". Меняем занчение "Тип запуска" на "Отключена". "Состояние" меняем на "Остановть". Нажимаем "Применить" и "ОК".
5. Ищем строку "Центр Обновления Windows" и меняем все значения как в п.2.
6. Скачиваем и устанавливаем программу Windows Update Blocker - [https://www.sordum.org/9470/windows-update-blocker-v1-6/](https://www.sordum.org/9470/windows-update-blocker-v1-6/)
7. Запускаем Windows Update BLocker от имени администратора. Выбираем опцию "Disable Updates", ставим галочку на опцию "Protect Services Settings" и нажимаем "Apply Now". Закрываем программу.
8. Скачиваем репозиторий "Windows10Debloater" (Code - Download ZIP) с Github по ссылке - [https://github.com/Sycnex/Windows10Debloater](https://github.com/Sycnex/Windows10Debloater)
9. Разархивируем скаченный архив на рабочем столе.
10. Запускаем Powershell от имени администратора и переходм в домашнюю директорию командой ```cd ~```.
11. Переходим в директорию рабочего стола ```cd Desktop```.
12. Вводим команду ```Set-ExecutionPolicy unrestricted``` и ```y``` (да) для подтверждения.
13. Переходим в папку Windows10Debloater-master ```cd Windows10Debloater-master```s и запускаем скрипт ```Windows10Debloater.ps1```. 
14. На большинстве всплывающих окнах нажимаем "Да"/"Yes", кроме последнего "Reboot". На "Reboot" нажимаем "No".
15. Переходим в "Параметры - Конфиденциальность - Общие". Отключаем все опции.
16. Повторяем те же действия для разделов: "Голосовые функции", "Персонализация рукописного ввода с клавиатуры", "Диагностика и отзывы", "Журнал действий", "Расположение", "Фоновые приложения", "Диагностика приложений".
17. Перезагружаем компьютер.