# Сайт: где живёт и как улучшить адрес

## Сейчас (работает с 20.10.2026)
**https://timonparpiev-code.github.io** — бесплатно, GitHub Pages, репозиторий `timonparpiev-code/timonparpiev-code.github.io`.

Обновить сайт: правки в `ночная-смена/site/index.html`, затем
```bash
python tools/build_site.py . https://timonparpiev-code.github.io
```
(из папки `ночная-смена`), потом в папке `ksisov-site`: `git add -A`, `git commit`, `git push`. Через 1–2 минуты изменения на сайте.

## Вариант 1, бесплатно: адрес qsissow.github.io
1. Создай бесплатную организацию **qsissow**: https://github.com/account/organizations/new?plan=free (это новый аккаунт-организация, создаёшь сам).
2. Репозиторий → **Settings** → внизу **Transfer ownership** → новый владелец `qsissow`.
3. В организации переименуй репозиторий в **qsissow.github.io** (Settings → Repository name).
4. Скажи мне: пересоберу сайт под новый адрес и поправлю адрес отправки в git.

## Вариант 2, платно: свой домен qsissow.com
Цены на 20.10.2026: **NiceNIC** $14.99 за первый год, продление $16.99, оплата USDT; **NameSilo** $17.29 в год.

1. Купить `qsissow.com`.
2. Скажи мне: добавлю файл `CNAME` и пересоберу сайт.
3. Репозиторий → **Settings** → **Pages** → Custom domain: `qsissow.com` → Save, потом **Enforce HTTPS**.
4. DNS у регистратора (старые A-записи «парковки» удалить):

| Тип | Имя (Host) | Значение |
|---|---|---|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | timonparpiev-code.github.io (или qsissow.github.io после варианта 1) |

Через 10 минут – сутки сайт откроется на https://qsissow.com.
