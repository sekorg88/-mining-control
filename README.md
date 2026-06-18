[Uploading README.md…]()
# ⚡ Mining Control

<div align="center">

![Mining Control](https://img.shields.io/badge/version-1.0.1-00e5ff?style=for-the-badge)
![Platform](https://img.shields.io/badge/platform-Windows-39ff14?style=for-the-badge)
![License](https://img.shields.io/badge/license-MIT-bf5af2?style=for-the-badge)
![Dev Fee](https://img.shields.io/badge/dev%20fee-1%25-ffd60a?style=for-the-badge)
![GPU](https://img.shields.io/badge/GPU-NVIDIA%20only-76b900?style=for-the-badge&logo=nvidia)

**Smart GPU mining panel with auto-switching to the most profitable coin**

*Умная панель управления майнингом с авто-переключением на самую выгодную монету*

[⬇️ Download / Скачать](../../releases/latest) · [🐛 Issues](../../issues) · [⭐ Star us!](../../stargazers)

</div>

---

## 🆕 What's new in v1.0.1 / Что нового в v1.0.1

- 🔒 **Web interface password protection** — the remote web panel now requires a password to access. A random password is generated on first launch and can be changed anytime in Settings.
- 🔒 **Защита веб-интерфейса паролем** — удалённая веб-панель теперь требует пароль для доступа. При первом запуске генерируется случайный пароль, который можно изменить в любой момент в Настройках.

---

## 🇬🇧 English

### 🚀 Features

| Feature | Description |
|---------|-------------|
| ⚡ **Auto-switching** | Automatically switches to the most profitable coin in real time |
| 🔀 **PPLNS / SOLO** | Choose mining mode per coin |
| 📊 **Earnings chart** | Profitability history: 1h / 6h / 24h / 30 days |
| 🎛️ **MSI Afterburner** | Auto-apply GPU overclocking profiles per coin |
| 📡 **Pool statistics** | Balance, payouts, hashrate directly in the interface |
| 📱 **Web interface** | Remote access from phone/PC via `192.168.1.xxx:8765`, password-protected |
| 🎨 **3 Themes** | Neon / Apple / Glass Dark |
| 🌍 **5 Languages** | EN / RU / ZH / VI / PT |
| 💰 **Dev fee 1%** | Standard practice, honest and transparent |

### 📦 Installation

#### Step 1 — Download Mining Control
Download `MiningControl.exe` from [➡️ Releases](../../releases/latest)

#### Step 2 — Download miners

| Miner | Coins | Download |
|-------|-------|----------|
| **T-Rex** | ZANO, NEOX, KRGN | [github.com/trexminer/T-Rex](https://github.com/trexminer/T-Rex/releases) |
| **lolMiner** | NEXA, IRON | [github.com/Lolliedieb/lolMiner-releases](https://github.com/Lolliedieb/lolMiner-releases/releases) |
| **GMiner** | BEAM | [github.com/develsoftware/GMinerRelease](https://github.com/develsoftware/GMinerRelease/releases) |
| **TT-Miner** | EPIC | [tradeproject.de](https://tradeproject.de/) |
| **WildRig Multi** | EVR | [github.com/andru-kun/wildrig-multi](https://github.com/andru-kun/wildrig-multi/releases) |

#### Step 3 — MSI Afterburner (optional)
Download from official site: [msi.com/Landing/afterburner](https://www.msi.com/Landing/afterburner/graphics-cards)

#### Step 4 — Recommended folder structure
```
📁 C:\mining\
   📁 trex\              ← T-Rex miner
   📁 lolminer\          ← lolMiner
   📁 gminer\            ← GMiner
   📁 ttminer\           ← TT-Miner
   📁 wildrig\           ← WildRig Multi (for EVR)
   MiningControl.exe     ← Mining Control
   mining_config.json    ← auto-created on first run
   debug.log             ← logs
```

#### Step 5 — First launch
1. Run `MiningControl.exe`
2. Complete onboarding — enter your wallet addresses
3. Set miner paths (right panel → Configuration → Miner Paths)
4. Run benchmark to detect hashrates
   > 💡 If benchmark fails — enter hashrate manually in "My Hashrate"
5. Enable Auto-switching and start mining! 🎉

### ⚙️ System Requirements

> ⚠️ **NVIDIA GPUs only!** AMD is not supported in this version.

- Windows 10 / 11 (64-bit)
- **NVIDIA GPU** — GTX 1060 / 1660 / RTX 2060 / 3060 / 4060 or newer
- NVIDIA drivers **596.49 or lower** (download: [nvidia.com/drivers](https://www.nvidia.com/drivers))
- > ⚠️ Driver **610.xx breaks OpenCL** for WildRig (EVR mining). Use driver **596.49 or lower** for stable EVR mining!
- Internet connection for price data and pool stats

> 🔜 AMD support is planned for a future version.

### 📊 Supported Pools

| Coin | Pool |
|------|------|
| ZANO | WoolyPooly |
| NEOX | 2Miners |
| NEXA | 2Miners |
| EPIC | EpicMine |
| BEAM | HeroMiners |
| IRON | HeroMiners |
| KRGN | HimPool |
| EVR | EVRPool |


---

## 🗂️ Manual miner batch files

In the repository you'll find ready-to-use `.bat` files for each coin.

> ⚠️ **Before use** — open the file in Notepad and replace `WALLET_ADDRESS` with your actual wallet address!

| File | Coin | Miner |
|------|------|-------|
| `mine_ZANO.bat` | ZANO | T-Rex |
| `mine_NEOX.bat` | NEOX | T-Rex |
| `mine_NEXA.bat` | NEXA | lolMiner |
| `mine_EPIC.bat` | EPIC | TT-Miner |
| `mine_BEAM.bat` | BEAM | GMiner |
| `mine_IRON.bat` | IRON | lolMiner |
| `mine_KRGN.bat` | KRGN | T-Rex |
| `mine_EVR.bat` | EVR | WildRig Multi |

Example — open `mine_ZANO.bat` in Notepad and change:
```
--user WALLET_ADDRESS.rig1
```
to:
```
--user ZxD22Jbi5BF...youraddress.rig1
```

---

## 🇷🇺 Русский

### 🚀 Возможности

| Функция | Описание |
|---------|----------|
| ⚡ **Авто-переключение** | Автоматически переключается на самую выгодную монету в реальном времени |
| 🔀 **PPLNS / SOLO** | Выбор режима майнинга для каждой монеты |
| 📊 **График доходности** | История доходности: 1ч / 6ч / 24ч / 30 дней |
| 🎛️ **MSI Afterburner** | Авто-применение профилей разгона GPU для каждой монеты |
| 📡 **Статистика пулов** | Баланс, выплаты, хешрейт прямо в интерфейсе |
| 📱 **Веб-интерфейс** | Доступ с телефона/ПК по `192.168.1.xxx:8765`, защищён паролем |
| 🎨 **3 темы** | Neon / Apple / Glass Dark |
| 🌍 **5 языков** | EN / RU / ZH / VI / PT |
| 💰 **Dev fee 1%** | Стандартная практика, честно и прозрачно |

### 📦 Установка

#### Шаг 1 — Скачай Mining Control
Скачай `MiningControl.exe` из [➡️ Releases](../../releases/latest)

#### Шаг 2 — Скачай майнеры

| Майнер | Монеты | Ссылка |
|--------|--------|--------|
| **T-Rex** | ZANO, NEOX, KRGN | [github.com/trexminer/T-Rex](https://github.com/trexminer/T-Rex/releases) |
| **lolMiner** | NEXA, IRON | [github.com/Lolliedieb/lolMiner-releases](https://github.com/Lolliedieb/lolMiner-releases/releases) |
| **GMiner** | BEAM | [github.com/develsoftware/GMinerRelease](https://github.com/develsoftware/GMinerRelease/releases) |
| **TT-Miner** | EPIC | [tradeproject.de](https://tradeproject.de/) |
| **WildRig Multi** | EVR | [github.com/andru-kun/wildrig-multi](https://github.com/andru-kun/wildrig-multi/releases) |

#### Шаг 3 — MSI Afterburner (опционально)
Скачай с официального сайта: [msi.com/Landing/afterburner](https://www.msi.com/Landing/afterburner/graphics-cards)

#### Шаг 4 — Рекомендуемая структура папок
```
📁 C:\mining\
   📁 trex\              ← T-Rex майнер
   📁 lolminer\          ← lolMiner
   📁 gminer\            ← GMiner
   📁 ttminer\           ← TT-Miner
   📁 wildrig\           ← WildRig Multi (для EVR)
   MiningControl.exe     ← Mining Control
   mining_config.json    ← создаётся автоматически
   debug.log             ← логи
```

#### Шаг 5 — Первый запуск
1. Запусти `MiningControl.exe`
2. Пройди онбординг — введи адреса кошельков
3. Укажи пути к майнерам (правая панель → Конфигурация → Пути к майнерам)
4. Запусти бенчмарк для определения хешрейтов
   > 💡 Если бенчмарк не прошёл — введи хешрейт вручную в "Мой хешрейт"
5. Включи авто-переключение и начинай майнить! 🎉

### ⚙️ Системные требования

> ⚠️ **Только видеокарты NVIDIA!** AMD не поддерживается в этой версии.

- Windows 10 / 11 (64-bit)
- **Видеокарта NVIDIA** — GTX 1060 / 1660 / RTX 2060 / 3060 / 4060 и новее
- Драйверы NVIDIA **596.49 или ниже** (скачать: [nvidia.com/drivers](https://www.nvidia.com/drivers))
- > ⚠️ Драйвер **610.xx ломает OpenCL** для WildRig (майнинг EVR). Для стабильной работы EVR используй драйвер **596.49 или ниже**!
- Интернет для получения цен и данных пулов

> 🔜 Поддержка AMD запланирована в будущей версии.

### 📊 Поддерживаемые пулы

| Монета | Пул |
|--------|-----|
| ZANO | WoolyPooly |
| NEOX | 2Miners |
| NEXA | 2Miners |
| EPIC | EpicMine |
| BEAM | HeroMiners |
| IRON | HeroMiners |
| KRGN | HimPool |
| EVR | EVRPool |


---

## 🗂️ Bat файлы для ручного запуска майнеров

В репозитории есть готовые `.bat` файлы для каждой монеты.

> ⚠️ **Перед использованием** — открой файл в блокноте и замени `WALLET_ADDRESS` на свой адрес кошелька!

| Файл | Монета | Майнер |
|------|--------|--------|
| `mine_ZANO.bat` | ZANO | T-Rex |
| `mine_NEOX.bat` | NEOX | T-Rex |
| `mine_NEXA.bat` | NEXA | lolMiner |
| `mine_EPIC.bat` | EPIC | TT-Miner |
| `mine_BEAM.bat` | BEAM | GMiner |
| `mine_IRON.bat` | IRON | lolMiner |
| `mine_KRGN.bat` | KRGN | T-Rex |
| `mine_EVR.bat` | EVR | WildRig Multi |

Пример — открой `mine_ZANO.bat` в блокноте и замени:
```
--user WALLET_ADDRESS.rig1
```
на:
```
--user ZxD22Jbi5BF...твойадрес.rig1
```

---

## 📝 License / Лицензия

MIT License — free to use, but keep the author mention.  
Свободное использование, но сохраняй упоминание автора.

---

<div align="center">

*Mining Control v1.0.1 · Dev fee 1% · Made with ❤️ by sekorg88*

</div>
