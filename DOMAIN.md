# Как запустить сайт

## Сейчас: бесплатно на https://qsissow.github.io

Сайт уже собран под этот адрес. Имя `qsissow` на GitHub свободно (проверено 20.10.2026).

### Шаг 1. Создать бесплатную организацию qsissow (2 минуты)
1. Открой https://github.com/account/organizations/new?plan=free
2. Organization name: **qsissow**
3. Contact email: твоя почта
4. «This organization belongs to»: **My personal account**
5. Нажми **Next**, приглашать участников не нужно (**Skip this step** / **Complete setup**).

### Шаг 2. Создать в ней репозиторий
1. Открой https://github.com/organizations/qsissow/repositories/new
2. Repository name: **qsissow.github.io** (именно так, с точками)
3. **Public**
4. Ничего не добавлять: без README, без .gitignore, без лицензии.
5. **Create repository**

### Шаг 3. Написать мне
Я отправлю сайт в этот репозиторий. Репозиторий с таким именем GitHub публикует автоматически: через 1–2 минуты сайт откроется на **https://qsissow.github.io**.

Если сайт не появился: репозиторий → **Settings** → **Pages** → Source: **Deploy from a branch**, Branch: **main**, папка **/ (root)** → **Save**.

---

## Потом: свой домен qsissow.com (когда появятся деньги)

Цены на 20.10.2026: **NiceNIC** $14.99 за первый год и $16.99 за продление, оплата USDT; **NameSilo** $17.29 в год.

1. Купить `qsissow.com`.
2. Сказать мне: я верну в репозиторий файл `CNAME` и пересоберу сайт под новый адрес (одна команда).
3. Репозиторий → **Settings** → **Pages** → Custom domain: `qsissow.com` → Save, потом включить **Enforce HTTPS**.
4. В панели регистратора добавить DNS-записи (старые A-записи «парковки» удалить):

| Тип | Имя (Host) | Значение |
|---|---|---|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | qsissow.github.io |

Через 10 минут – сутки сайт откроется на https://qsissow.com, а старый адрес qsissow.github.io будет сам перенаправлять туда.

## Как обновлять сайт
Правки делаются в `ночная-смена/site/index.html`, затем:
```bash
python tools/build_site.py . https://qsissow.github.io
```
и в папке `ksisov-site`: коммит + `git push`.
