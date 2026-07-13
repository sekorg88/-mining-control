# ⚡ Mining Control

<div align="center">

![Mining Control](https://img.shields.io/badge/version-1.0.2-00e5ff?style=for-the-badge)
![Platform](https://img.shields.io/badge/platform-Windows-39ff14?style=for-the-badge)
![License](https://img.shields.io/badge/license-MIT-bf5af2?style=for-the-badge)
![Dev Fee](https://img.shields.io/badge/dev%20fee-1%25-ffd60a?style=for-the-badge)
![GPU](https://img.shields.io/badge/GPU-NVIDIA%20only-76b900?style=for-the-badge&logo=nvidia)

**Smart GPU mining panel with auto-switching to the most profitable coin**

*Умная панель управления майнингом с авто-переключением на самую выгодную монету*

[⬇️ Download / Скачать](../../releases/latest) · [🐛 Issues](../../issues) · [⭐ Star us!](../../stargazers)

</div>

---

## 🆕 What's new in v1.0.2 / Что нового в v1.0.2

- 🔧 **Fixed several broken pool endpoints** — KRGN, EVR, and NEXA balance stats were pointing at outdated/incorrect API hosts and have been corrected.
- 🔀 **NEOX switched pools** — moved from a discontinued 2Miners endpoint to **RPlant**, with full automatic balance/hashrate stats.
- 🔑 **EPIC automatic stats (optional)** — you can now link your own EpicMine API key/secret (Settings → EPIC API) to get live balance stats. Without it, EPIC still mines normally, just without auto-stats.
- 🔴 **New-payout indicators** — each coin in the "Total" panel now shows a small pulsing dot when the pool actually sends you a new payout. It clears when you manually refresh.
- 🔄 **Auto-refresh every minute** — pool balances now update automatically in the background, no need to click Refresh constantly.

<br>

- 🔧 **Исправлены несколько нерабочих эндпоинтов пулов** — статистика баланса KRGN, EVR и NEXA указывала на устаревшие/неверные API-хосты, теперь исправлено.
- 🔀 **NEOX сменил пул** — переехал с закрытого эндпоинта 2Miners на **RPlant**, с полной автоматической статистикой баланса/хешрейта.
- 🔑 **Автостатистика EPIC (опционально)** — теперь можно привязать свой личный API-ключ/секрет от EpicMine (Настройки → EPIC API) для получения баланса в реальном времени. Без ключа EPIC всё так же майнит нормально, просто без автостатистики.
- 🔴 **Индикаторы новых начислений** — каждая монета в разделе "Итого" теперь показывает мигающую точку, когда пул реально прислал новую выплату. Гаснет при ручном обновлении.
- 🔄 **Автообновление раз в минуту** — баланс пулов теперь обновляется сам в фоне, не нужно постоянно жать "Обновить".


---

## 🇬🇧 English

### 🚀 Features

| Feature | Description |
|---------|-------------|
| ⚡ **Auto-switching** | Automatically switches to the most profitable coin in real time |
| 🔀 **PPLNS / SOLO** | Choose mining mode per coin |
| 📊 **Earnings chart** | Profitability history: 1h / 6h / 24h / 30 days |
| 🎛️ **MSI Afterburner** | Auto-apply GPU overclocking profiles per coin |
| 📡 **Pool statistics** | Balance, payouts, hashrate directly in the interface, auto-refreshed every minute |
| 🔴 **Payout indicators** | Visual alert in the Total panel when a pool sends a new payout |
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
   > 💡 Want automatic EPIC balance stats? Optionally add your EpicMine API key/secret in the same step — get them at [epicmine.io/account/settings](https://epicmine.io/account/settings) → User API → Generate new key pair
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
| NEOX | RPlant |
| NEXA | 2Miners |
| EPIC | EpicMine |
| BEAM | HeroMiners |
| IRON | HeroMiners |
| KRGN | HimPool |
| EVR | EVRPool |

### 🛠️ Troubleshooting

Having trouble with a specific coin? You can test its stratum connection manually before reporting an issue — for example, for NEOX via RPlant:

```
t-rex.exe -a kawpow -o stratum+ssl://eu.rplant.xyz:17069 -u YOUR_WALLET.rig1 -p x
```

Each pool's exact host/port can be found on its own website's "Connect" / "How to start" page. If the miner authorizes and shares are accepted there but not in Mining Control, please [open an issue](../../issues) with your `debug.log`.

---

## 🇷🇺 Русский

### 🚀 Возможности

| Функция | Описание |
|---------|----------|
| ⚡ **Авто-переключение** | Автоматически переключается на самую выгодную монету в реальном времени |
| 🔀 **PPLNS / SOLO** | Выбор режима майнинга для каждой монеты |
| 📊 **График доходности** | История доходности: 1ч / 6ч / 24ч / 30 дней |
| 🎛️ **MSI Afterburner** | Авто-применение профилей разгона GPU для каждой монеты |
| 📡 **Статистика пулов** | Баланс, выплаты, хешрейт прямо в интерфейсе, автообновление раз в минуту |
| 🔴 **Индикаторы выплат** | Визуальная отметка в разделе "Итого", когда пул присылает новую выплату |
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
   > 💡 Хочешь автостатистику баланса EPIC? Опционально добавь свой API-ключ/секрет от EpicMine на этом же шаге — получить можно на [epicmine.io/account/settings](https://epicmine.io/account/settings) → User API → Generate new key pair
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
| NEOX | RPlant |
| NEXA | 2Miners |
| EPIC | EpicMine |
| BEAM | HeroMiners |
| IRON | HeroMiners |
| KRGN | HimPool |
| EVR | EVRPool |

### 🛠️ Диагностика проблем

Не работает конкретная монета? Можешь вручную проверить подключение к пулу перед тем как создавать issue — например, для NEOX через RPlant:

```
t-rex.exe -a kawpow -o stratum+ssl://eu.rplant.xyz:17069 -u ТВОЙ_КОШЕЛЁК.rig1 -p x
```

Точный хост/порт для каждого пула можно найти на его сайте в разделе "Connect" / "How to start". Если майнер авторизуется и шары принимаются там, но не в Mining Control — пожалуйста, [создай issue](../../issues) и приложи `debug.log`.

---

## 📝 License / Лицензия

MIT License — free to use, but keep the author mention.
Свободное использование, но сохраняй упоминание автора.

---

<div align="center">

*Mining Control v1.0.2 · Dev fee 1% · Made with ❤️ by sekorg88*

</div>
