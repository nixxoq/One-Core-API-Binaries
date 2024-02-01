**Ласкаво просимо до бінарників One-Core-API!**

***
**Language:**    
[English](README.md) | [简体中文](README_CN.md) | [Русский](README_RU.md) | [Українська](README_UK.md) | [日本語](README_JP.md) | [Português do Brasil](README_BR.md)
***

Цей репозиторій містить бінарні версії проєкту One-Core-API. Вони сумісні з Windows Server 2003 SP2, Windows XP SP3 і Windows XP x64 SP2.

**Офіційний Discord сервер**: https://discord.gg/eRcGuFtn6p

**ПРИМІТКА**:
- Windows XP Unofficial SP4 та, можливо, Integral Edition не підтримуються!

**Мовна підтримка**
Мовна підтримка майже всіх частин Windows: Португальська-Бразилія (моя мова), Португальська (Portugual), Турецька, Китайська (традиційна та спрощена), Французька, Італійська, Угорська, Українська (частково), Іспанська, Польська, Російська та Корейська;

**Директорії в цьому репозиторії**
- Documents: Документація за проєктом, відомі помилки, використання sfxcab (для створення інсталяторів) тощо.
- Packages\x86 та Packages\x64: Бінарні файли, які розділені за пакетами. Ви можете завантажити і встановити/оновити пакети прямо звідси (тобто перейшовши в Packages\x86\Base installer\update та запустивши update.exe).
- Todo: To do завдання
- Test: Деякі бінарні файли та документи для тестування;
- Release: Скрипти для генерації нового випуску бінарників;
- Output: Вихідні двійкові файли, які можна згенерувати за допомогою скриптів у папці Release;

**Проєкт One-Core-API Binaries складається з таких пакетів:**
Увага: Якщо пакет OCA вимагає перезавантаження, завжди виконуйте його. Якщо ви встановите всі пакети і перезапустите тільки останній, Windows **може бути** пошкоджена.
- **Base**: Основний пакет One-Core-API, який потрібен усім іншим пакетам, окрім App Compat і Driver Update, і містить усі обгортки, що використовуються в цьому проєкті (наприклад, kernelbase і ntext);
- **Additional Dlls**: Деякі нові dll файли, що з'явилися в пізніших версіях Windows.
- **D3d**: D3D (в основному DX10 і DX11, засновано на WineD3D);
- **App Compat**: Параметри сумісності додатків (Application Compatibility), перенесені з пізніших версій Windows.
- **Driver Update**: Оновлений драйвер acpi з підтримкою ACPI 2.0, нові драйвери Storachi (для контролерів AHCI), NVME (для контролерів NVME M.2) і USBXHCI (USB 3.0);
- **Branding**: Нова система брендингу (branding system), введена в Windows Vista, необхідна для пакетів D3D і Modern Setup;

**Порядок встановлення пакетів:**
- **Звичайний порядок**: Base -> Additional Dlls -> Branding -> D3d -> Driver Update -> App Compat;

- **Окремі пакети (не вимагають встановлення інших пакетів, тільки за бажанням)**
  - **App Compat only:** Цей пакет може бути встановлений без будь-яких інших пакетів;
  - **Driver Update Only**: Цей пакет може бути встановлений без будь-яких інших пакетів;
  - **AppCompat first**: Цей пакет може бути встановлений без будь-яких інших пакетів;

**Основні особливості**:
- Збільшення підтримки пам'яті до 128 ГБ для x86 і 2 ТБ для x64 за замовчуванням;
- Забезпечує підтримку запуску нових програм, розроблених для сучасних ОС Windows;
- Забезпечення підтримки нового обладнання за допомогою нових контролерів із драйверами;


**One-Core-API дозволяє запускати:**
- JetBrains WebStorm 2018;
- JetBrains Intellij 2018 (Інші версії теж можуть працювати);
- JetBrains WebStorm 2023.x.x (Поки що тільки для Windows XP x64)
- JetBrains IntelliJ 2023.x.x (Поки що тільки для Windows XP x64)
- Adobe Photoshop CC 2018;
- Filezilla (остання версія);
- Visual Studio Code до версії 1.83.1;
- Chrome аж до версії 122!
- Opera до версії 105;
- Firefox до версії 116 (з помилками і вимагає обхідні шляхи);
- Microsoft Edge аж до версії 115;
- Brave аж до версії 117;
- Yandex Browser остання версія;
- Thorium browser аж до 109;
- Supermium аж до версії 117;
- Seamonkey аж до версії 2.53.10;
- Thunderbird аж до версії 115;
- Maxthon аж до 7.1.6;
- Vivaldi аж до останньої версії;
- JDK 1.8 (Поки що тільки для Windows XP x64);
- Java Alternative JDK чи OpenJDK до версії 21 (можливо, інші версії працюють). Ви можете завантажити з сайту https://bell-sw.com/pages/downloads/#/java-11-lts;
- Maxthon 6;
- Epic Browser 94;
- Python 3.6;
- .Net Framework аж до 4.8;
- Geekbench 4.2;
- Тести продуктивності;
- Adobe Reader DC (2017);
- Windows 7 ігри;
- Рідні застосунки Windows Vista;
- Spotify після закінчення підтримки Windows XP/Vista, версія 1.0.60;
- Yandex browser (остання версія);
- Zoom;
- Деякі інші застосунки;
- Node 10.24;
- Winrar 7.0 Beta 4 (остання);
- Directx 9EX, 10 та 11 ігри: 
  - Need for Speed Most Wanted 2012;
  - Need for Speed The Run;
  - Street Figther V;
  - Injustice: Gods among us;
  - Assassign Creed Black Flgs;
  - Crysis 1,2, and 3 (directx 10-11 режим);
- Kate 23.08.1 (Поки що тільки для Windows XP x64)


**Відомі обмеження:**
- Деякі місця в діалогах або вікнах підтримують тільки англійську мову. Робота над інтернаціоналізацією триває; Деякі проблеми зі встановленими MUI пакетами;
- Інсталятори нових застосунків можуть не працювати, наприклад Chrome, Maxthon, Discord, Team viewer тощо падають, і застосунок не встановлюється. Необхідно 
використовувати попередньо встановлену версію, скопійовану з іншої операційної системи;
- Пакети не можуть бути інтегровані за допомогою nlite в Windows Iso, оскільки використовують інструмент під назвою "SFXCAB Substitute", а не стандартну версію Microsoft;
- Стандартні інсталятори .Net Framework, починаючи з 4.6, поки що не підтримуються. Вам потрібна перепакована версія, як тут: https://github.com/abbodi1406/dotNetFx4xW7. І доступна, як тут: https://www.wincert.net/forum/topic/13805-microsoft-net-framework-472-full-x86x64-incl-language-packs-by-ricktendo/#comment-123251. Інші версії теж доступні, шукайте в темах на форумі;
- У нових версіях Palemoon може виникнути проблема з помилками конфігурації (configuration error);
- Для запуску Opera 39 - 46 можуть знадобитися такі параметри: --disable-gpu (для запобігання чорного екрана) і --single-process (для запобігання вічного завантаження першої сторінки);

**Звіт про проблеми**

**Нотатка:**

Якщо у вас виникли проблеми з Chrome або браузерами на основі Chromium, будь ласка, повідомте про це за цим посиланням: https://github.com/Skulltrail192/One-Core-API-Binaries/issues/178.

Якщо проблеми пов'язані з браузерами Firefox або Gecko подібними, будь ласка, використовуйте наступне посилання на GitHub для повідомлень: https://github.com/Skulltrail192/One-Core-API-Binaries/issues/214.

Якщо проблема пов'язана з BSoD (Синій екран смерті), повідомте про неї на цій сторінці: https://github.com/Skulltrail192/One-Core-API-Binaries/issues/233.

Для допомоги у відтворенні проблеми рекомендується **завжди** дотримуватися цього шаблону:
- Опис того, що сталося.
  Наприклад: Завжди отримуйте BSOD під час спроби завантажити Windows. Windows застрягла на екрані завантаження. Windows завжди отримує чорний екран тощо;
- Конфігурація віртуальної машини/ПК
  Наприклад: Vmware 10, virtualBox 6.1.0 або Core 2 Duo 8400, 2Gb DDR2, IDE/SATA Hard Disk;
- Версія Windows і конфігурація
  Наприклад: Windows XP Service Pack 3 зі встановленими оновленнями POSReady 2009, з таким списком програм: Adobe, Office тощо;

Декілька скріншотів застосунків, що працюють на XP/Server 2003:

**Chrome 122**
![Chrome 122](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/6442a5b0-036b-48e0-a6e8-3624825d3882)

**Edge 122**
![Edge122](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/734954f4-2540-4657-9a2d-ce6aed809bf5)

**Opera 106**
![Opera106](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/db509ccf-4e66-4e2b-ad4b-fd8512495333)

**Firefox 122**
![Firefox122](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/db647daf-0960-4ace-ad2f-63469dbf3881)

**Basilisk**
![image_2022_04_08T21_38_17_976Z](https://user-images.githubusercontent.com/5159776/178077859-079bfca4-bdb6-402e-8991-b88e7dfe387c.png)

**Vivaldi**
![vivaldi](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/86d5895f-977a-414f-b0d5-0e877a658676)

**Spotify (Для Windows 7)**
![Spotify-Windows7](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/09de7c20-8670-45dc-9471-a6db9349abd0)

**Visual Studio Code 1.81**
![VisualCode](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/b21748b9-25bb-412d-95b3-2219d2efdf42)

**Microsoft Chess 3d**
![Chess3d](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/bd1ad0c6-edde-4ff2-a6e0-074c7379fab6)

**Libre Office 24 (остання версія)**
![LibreOffice](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/11fd191d-270c-428d-8d41-0498e8fafb3b)
![Writer-LibreOffice](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/e389a39b-febd-45f6-9c6f-25f64e460142)

**Discord 0.309**
![Discord-Login](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/8a4c12b5-19fc-454d-b02a-a1db807d3900)
![Discord](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/eb673541-4e66-4c76-867e-346edbaaa0af)

**Telegram Desktop**
![Telegram-Desktop](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/d23b9add-629d-45a3-a8e1-c331271bc0d3)

**Zoom meeting**
![Zoom](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/d002cf1b-c5f4-4c0c-b629-00e031a56765)

**Java 11**
![Capturar](https://user-images.githubusercontent.com/5159776/178078132-da504607-a1ca-4f8d-ae25-6a7eb367bdaa.PNG)

**Avast та Chromium 68**
![Avast](https://user-images.githubusercontent.com/5159776/178078208-c13b3448-ee6a-4c56-9d94-d0c62d51949e.PNG)

**Windows 7 Sticky Notes**
![StickyNotes](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/669ba3e4-b831-4a96-ad40-d87e3e9531e2)

**Windows 7 Paint**
![Paint](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/81728a44-c9e7-41e8-b68b-8ea7b119ebba)

**Windows 7 Wordpad**
![Wordpad](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/9dac02c7-7139-47fe-8732-ccd9ef91090b)
