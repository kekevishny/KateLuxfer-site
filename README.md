# Локальный сервер для показа локального файла

Этот минимальный проект запускает локальный HTTP-сервер, который при обращении к http://localhost:8000/ отдает файл:

`C:\Users\keke\сайт\index.html`

Файлы в репозитории:

- `server.py` — простой Python-сервер, отдающий указанный локальный файл на корневом пути `/`.
- `run.ps1` — PowerShell-скрипт для запуска сервера.
- `start.bat` — bat-файл для запуска сервера в Windows.

Файл `CNAME` с вашим доменом `kateluxfer.moscow` уже создан в корне проекта (если хотите изменить — отредактируйте `CNAME`).

Как запустить (PowerShell):

```powershell
python .\server.py
# или указать порт
python .\server.py --port 8000
```

Альтернативно в PowerShell можно запустить `run.ps1`, в классическом терминале — `start.bat`.

Примечания:

- Сервер использует стандартную библиотеку Python, внешние зависимости не требуются.
- Убедитесь, что файл `C:\Users\keke\сайт\index.html` существует и доступен для чтения.

## Настройка Git

Если вы хотите связать свой локальный репозиторий с удаленным на GitHub, выполните следующие команды:

```bash
git remote add origin https://github.com/yourusername/kateluxfer-site.git
git branch -M main
git push -u origin main
```

Не забудьте заменить `yourusername` на ваше имя пользователя GitHub.
