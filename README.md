<div align="center">

<br/>

```
    ╔═╗╔═╗  ╔═╗╦  ╦ ╦╔═╗╦╔╗╔╔═╗
    ╠═╣║╣   ╠═╝║  ║ ║║ ╦║║║║╚═╗
    ╩ ╩╚═╝  ╩  ╩═╝╚═╝╚═╝╩╝╚╝╚═╝
         INSTALL SCRIPT
```

# AE Plugins Install Script

**Автоматическая установка плагинов для Adobe After Effects одной командой**

[![Windows](https://img.shields.io/badge/Windows-0078D6?style=flat-square&logo=windows&logoColor=white)](https://github.com/Aks-iom/Aks-iom-AE-Plugins-install-script)
[![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=flat-square&logo=powershell&logoColor=white)](https://github.com/Aks-iom/Aks-iom-AE-Plugins-install-script)
[![After Effects](https://img.shields.io/badge/After_Effects-9999FF?style=flat-square&logo=adobe-after-effects&logoColor=white)](https://github.com/Aks-iom/Aks-iom-AE-Plugins-install-script)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)

<br/>

</div>

---

## Что это?

Устал вручную копировать плагины в нужные папки после каждой переустановки системы? Этот скрипт автоматизирует весь процесс — он определяет версию After Effects, находит правильные директории и устанавливает все плагины за секунды.

---

## Возможности

- **Авто-определение версии AE** — скрипт сам находит установленный After Effects
- **Правильные пути** — устанавливает файлы именно туда, куда нужно
- **Пакетная установка** — все плагины сразу, без возни с каждым вручную
- **Быстрый запуск** — одна команда, и всё готово

---

## Быстрый старт

### Требования

- Windows 10 / 11
- Adobe After Effects (CC 2019 и новее)
- PowerShell 5.0+
- Права администратора

### Установка

**1. Клонируй репозиторий:**

```bash
git clone https://github.com/Aks-iom/Aks-iom-AE-Plugins-install-script.git
cd Aks-iom-AE-Plugins-install-script
```

**2. Запусти скрипт от имени администратора:**

```powershell
# Правой кнопкой мыши на PowerShell → "Запуск от имени администратора"
.\install.ps1
```

**3. Следуй инструкциям на экране** — скрипт сделает всё остальное.

> **Совет:** Перед запуском убедись, что After Effects закрыт.

---

## Структура проекта

```
Aks-iom-AE-Plugins-install-script/
│
├── install.ps1          # Основной скрипт установки
├── plugins/             # Папка с плагинами
│   ├── *.aex            # Файлы плагинов After Effects
│   └── ...
└── README.md
```

---

## Куда устанавливаются плагины?

| Тип | Путь |
|-----|------|
| Плагины (общие) | `C:\Program Files\Adobe\Common\Plug-ins\7.0\MediaCore\` |
| Плагины (для конкретной версии AE) | `C:\Program Files\Adobe\Adobe After Effects [версия]\Support Files\Plug-ins\` |
| Скрипты | `C:\Program Files\Adobe\Adobe After Effects [версия]\Support Files\Scripts\` |
| ScriptUI Panels | `C:\Program Files\Adobe\Adobe After Effects [версия]\Support Files\Scripts\ScriptUI Panels\` |

---

## Частые вопросы

**После установки плагины не появляются в AE?**  
Перезапусти After Effects — плагины загружаются только при старте программы.

**Скрипт выдаёт ошибку прав доступа?**  
Запусти PowerShell от имени администратора.

**У меня несколько версий AE — в какую установится?**  
Скрипт определяет последнюю установленную версию. Если нужна конкретная — измени путь в `install.ps1`.

**Нужно ли закрывать After Effects перед запуском?**  
Да, рекомендуется закрыть AE перед установкой во избежание конфликтов.

---

## Вклад в проект

Нашёл баг или хочешь добавить плагин? Pull requests приветствуются!

1. Форкни репозиторий
2. Создай ветку: `git checkout -b feature/новый-плагин`
3. Зафиксируй изменения: `git commit -m 'Добавлен новый плагин'`
4. Запушь ветку: `git push origin feature/новый-плагин`
5. Открой Pull Request

---

## Лицензия

Распространяется под лицензией MIT. Подробнее — в файле [LICENSE](LICENSE).

---

<div align="center">

Сделано с ❤️ by [Aks-iom](https://github.com/Aks-iom)

*Если проект оказался полезным — поставь ⭐*

</div>
