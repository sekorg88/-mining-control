[README.md](https://github.com/user-attachments/files/29019310/README.md)
⚡ Mining Control
Mining Control Platform License Dev Fee GPU

Smart GPU mining panel with auto-switching to the most profitable coin

Умная панель управления майнингом с авто-переключением на самую выгодную монету

⬇️ Download / Скачать · 🐛 Issues · ⭐ Star us!

🇬🇧 English
🚀 Features
Feature	Description
⚡ Auto-switching	Automatically switches to the most profitable coin in real time
🔀 PPLNS / SOLO	Choose mining mode per coin
📊 Earnings chart	Profitability history: 1h / 6h / 24h / 30 days
🎛️ MSI Afterburner	Auto-apply GPU overclocking profiles per coin
📡 Pool statistics	Balance, payouts, hashrate directly in the interface
📱 Web interface	Remote access from phone/PC via 192.168.1.xxx:8765
🎨 3 Themes	Neon / Apple / Glass Dark
🌍 5 Languages	EN / RU / ZH / VI / PT
💰 Dev fee 1%	Standard practice, honest and transparent
📦 Installation
Step 1 — Download Mining Control
Download MiningControl.exe from ➡️ Releases

Step 2 — Download miners
Miner	Coins	Download
T-Rex	ZANO, NEOX, KRGN	github.com/trexminer/T-Rex
lolMiner	NEXA, IRON	github.com/Lolliedieb/lolMiner-releases
GMiner	BEAM	github.com/develsoftware/GMinerRelease
TT-Miner	EPIC	tradeproject.de
WildRig Multi	EVR	github.com/andru-kun/wildrig-multi

Step 3 — MSI Afterburner (optional)
Download from official site: msi.com/Landing/afterburner

Step 4 — Recommended folder structure
📁 C:\mining\
   📁 trex\              ← T-Rex miner
   📁 lolminer\          ← lolMiner
   📁 gminer\            ← GMiner
   📁 ttminer\           ← TT-Miner
   📁 wildrig\           ← WildRig Multi (for EVR)
   MiningControl.exe     ← Mining Control
   mining_config.json    ← auto-created on first run
   debug.log             ← logs

Step 5 — First launch
Run MiningControl.exe
Complete onboarding — enter your wallet addresses
Set miner paths (right panel → Configuration → Miner Paths)
Run benchmark to detect hashrates
💡 If benchmark fails — enter hashrate manually in "My Hashrate"

Enable Auto-switching and start mining! 🎉

⚙️ System Requirements
⚠️ NVIDIA GPUs only! AMD is not supported in this version.

Windows 10 / 11 (64-bit)
NVIDIA GPU — GTX 1060 / 1660 / RTX 2060 / 3060 / 4060 or newer
NVIDIA drivers version 596.49 or lower (download: nvidia.com/drivers)
⚠️ Driver 610.xx breaks OpenCL for WildRig (EVR mining). For stable EVR mining use driver 596.49 or lower!
Internet connection for price data and pool stats
🔜 AMD support is planned for a future version.

📊 Supported Pools
Coin	Pool
ZANO	WoolyPooly
NEOX	2Miners
NEXA	2Miners
EPIC	EpicMine
BEAM	HeroMiners
IRON	HeroMiners
KRGN	HimPool
EVR	EVRPool

🗂️ Manual miner batch files
In the repository you'll find ready-to-use .bat files for each coin.

⚠️ Before use — open the file in Notepad and replace WALLET_ADDRESS with your actual wallet address!

File	Coin	Miner
mine_ZANO.bat	ZANO	T-Rex
mine_NEOX.bat	NEOX	T-Rex
mine_NEXA.bat	NEXA	lolMiner
mine_EPIC.bat	EPIC	TT-Miner
mine_BEAM.bat	BEAM	GMiner
mine_IRON.bat	IRON	lolMiner
mine_KRGN.bat	KRGN	T-Rex
mine_EVR.bat	EVR	WildRig Multi

Example — open mine_ZANO.bat in Notepad and change:

--user WALLET_ADDRESS.rig1
to:

--user ZxD22Jbi5BF...youraddress.rig1

🇷🇺 Русский
🚀 Возможности
Функция	Описание
⚡ Авто-переключение	Автоматически переключается на самую выгодную монету в реальном времени
🔀 PPLNS / SOLO	Выбор режима майнинга для каждой монеты
📊 График доходности	История доходности: 1ч / 6ч / 24ч / 30 дней
🎛️ MSI Afterburner	Авто-применение профилей разгона GPU для каждой монеты
📡 Статистика пулов	Баланс, выплаты, хешрейт прямо в интерфейсе
📱 Веб-интерфейс	Доступ с телефона/ПК по 192.168.1.xxx:8765
🎨 3 темы	Neon / Apple / Glass Dark
🌍 5 языков	EN / RU / ZH / VI / PT
💰 Dev fee 1%	Стандартная практика, честно и прозрачно

📦 Установка
Шаг 1 — Скачай Mining Control
Скачай MiningControl.exe из ➡️ Releases

Шаг 2 — Скачай майнеры
Майнер	Монеты	Ссылка
T-Rex	ZANO, NEOX, KRGN	github.com/trexminer/T-Rex
lolMiner	NEXA, IRON	github.com/Lolliedieb/lolMiner-releases
GMiner	BEAM	github.com/develsoftware/GMinerRelease
TT-Miner	EPIC	tradeproject.de
WildRig Multi	EVR	github.com/andru-kun/wildrig-multi

Шаг 3 — MSI Afterburner (опционально)
Скачай с официального сайта: msi.com/Landing/afterburner

Шаг 4 — Рекомендуемая структура папок
📁 C:\mining\
   📁 trex\              ← T-Rex майнер
   📁 lolminer\          ← lolMiner
   📁 gminer\            ← GMiner
   📁 ttminer\           ← TT-Miner
   📁 wildrig\           ← WildRig Multi (для EVR)
   MiningControl.exe     ← Mining Control
   mining_config.json    ← создаётся автоматически
   debug.log             ← логи

Шаг 5 — Первый запуск
Запусти MiningControl.exe
Пройди онбординг — введи адреса кошельков
Укажи пути к майнерам (правая панель → Конфигурация → Пути к майнерам)
Запусти бенчмарк для определения хешрейтов
💡 Если бенчмарк не прошёл — введи хешрейт вручную в "Мой хешрейт"

Включи авто-переключение и начинай майнить! 🎉

⚙️ Системные требования
⚠️ Только видеокарты NVIDIA! AMD не поддерживается в этой версии.

Windows 10 / 11 (64-bit)
Видеокарта NVIDIA — GTX 1060 / 1660 / RTX 2060 / 3060 / 4060 и новее
Драйверы NVIDIA версии 596.49 или ниже (скачать: nvidia.com/drivers)
⚠️ Драйвер 610.xx ломает OpenCL для WildRig (майнинг EVR). Для стабильной работы EVR используй драйвер 596.49 или ниже!
Интернет для получения цен и данных пулов
🔜 Поддержка AMD запланирована в будущей версии.

📊 Поддерживаемые пулы
Монета	Пул
ZANO	WoolyPooly
NEOX	2Miners
NEXA	2Miners
EPIC	EpicMine
BEAM	HeroMiners
IRON	HeroMiners
KRGN	HimPool
EVR	EVRPool

🗂️ Bat файлы для ручного запуска майнеров
В репозитории есть готовые .bat файлы для каждой монеты.

⚠️ Перед использованием — открой файл в блокноте и замени WALLET_ADDRESS на свой адрес кошелька!

Файл	Монета	Майнер
mine_ZANO.bat	ZANO	T-Rex
mine_NEOX.bat	NEOX	T-Rex
mine_NEXA.bat	NEXA	lolMiner
mine_EPIC.bat	EPIC	TT-Miner
mine_BEAM.bat	BEAM	GMiner
mine_IRON.bat	IRON	lolMiner
mine_KRGN.bat	KRGN	T-Rex
mine_EVR.bat	EVR	WildRig Multi

Пример — открой mine_ZANO.bat в блокноте и замени:

--user WALLET_ADDRESS.rig1
на:

--user ZxD22Jbi5BF...твойадрес.rig1

📝 License / Лицензия
MIT License — free to use, but keep the author mention.
Свободное использование, но сохраняй упоминание автора.

Mining Control v1.0.0 · Dev fee 1% · Made with ❤️ by sekorg88
