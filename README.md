[![Typing SVG](https://readme-typing-svg.herokuapp.com?color=%2336BCF7&duration=8000&lines=Привет,+_+я+_+Степанов+_+Роман+.......|)](https://git.io/typing-svg)

## Немного обо мне
![Me](images/aboutME.png)

### Кратко о себе:

- Я --> Степанов Роман Сергеевич;
- Мне `22` года `(07.09.2003)`;
- Студент **СКФ МТУСИ**. Обучаюсь *на втором курсе* по специальности **"Защищённые инфокоммуникационные сети и системы"**;
- Ответственная, трудолюбивая, творческая, законопослушная личность;
- Знаток по *компьютерным сетям* и в *инфобезе* **(документация, криптография, физическая защита, программно-аппаратная защита)**;
- На данный момент, изучаю *веб-программирование, ИИ*;
- Разбираюсь в **документировании**, настройке **чистой архитектуры** проекта, **сборке** и **деплое** проектов на виртуальный сервер;
- Есть несколько интересных проектов на github.

## Навыки и технологии

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=Cricko7&layout=compact)](https://github.com/Cricko7/github-readme-stats)

- Операционные системы:
  
![Cent OS](https://img.shields.io/badge/cent%20os-002260?style=for-the-badge&logo=centos&logoColor=F0F0F0)
![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
![Debian](https://img.shields.io/badge/Debian-D70A53?style=for-the-badge&logo=debian&logoColor=white)
![Kali](https://img.shields.io/badge/Kali-268BEE?style=for-the-badge&logo=kalilinux&logoColor=white)
![Windows 11](https://img.shields.io/badge/Windows%2011-%230079d5.svg?style=for-the-badge&logo=Windows%2011&logoColor=white)

- Утилиты/программы:
  
![PowerShell](https://img.shields.io/badge/PowerShell-%235391FE.svg?style=for-the-badge&logo=powershell&logoColor=white)
![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)

- Языки программирования:
  
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![Vue.js](https://img.shields.io/badge/vuejs-%2335495e.svg?style=for-the-badge&logo=vuedotjs&logoColor=%234FC08D)
![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)

- Изучаю следующие ЯП:

![Golang](https://img.shields.io/badge/go-%2300ADD8.svg?style=for-the-badge&logo=go&logoColor=white)
![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![Rust](https://img.shields.io/badge/rust-%23000000.svg?style=for-the-badge&logo=rust&logoColor=white)

- СУБД:
  
![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)

- Технологии/библиотеки ЯП:
  
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)

- Хостинг проектов:
  
![PythonAnywhere](https://img.shields.io/badge/pythonanywhere-%232F9FD7.svg?style=for-the-badge&logo=pythonanywhere&logoColor=151515)
![Nginx](https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white)

- Сетевые технологии:
  
![Cisco](https://img.shields.io/badge/cisco-%23049fd9.svg?style=for-the-badge&logo=cisco&logoColor=black)

- Хранение проектов:
  
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)
![GitLab](https://img.shields.io/badge/gitlab-%23181717.svg?style=for-the-badge&logo=gitlab&logoColor=white)


## Опыт и проекты

![opit](gif/experrr.gif)

### Проект 1 — [Resume Vizor - веб-платформа цифровой верификации дипломов](https://github.com/Cricko7/resum-vizor)

Платформа цифровой верификации дипломов с backend на `Rust` + `Axum`, frontend для пользователей и отдельным `QR-сервисом`.

#### Платформа позволяет:
- вузу загружать дипломы по одному или массово через CSV/XLSX
- хранить чувствительные данные дипломов в хешированном виде
- автоматически подписывать записи дипломов цифровой подписью вуза
- студенту находить и привязывать свои дипломы
- студенту делиться временной ссылкой на диплом
- студенту запрашивать QR-код на свой диплом через отдельный QR-микросервис
- HR/ATS-системам проверять диплом через API
- вузу аннулировать диплом и восстанавливать его обратно

Текущий стек:

- `Rust`
- `Axum`
- `Tokio`
- `SQLx`
- `PostgreSQL`
- `Redis`

`in-memory` persistence сохранен для тестов и быстрых unit/integration-style сценариев.
`Redis` используется для трех production-полезных задач: распределенного rate limiting для machine-to-machine endpoints, response caching для read-heavy verification/search сценариев и кэширования QR-изображений, чтобы не дергать внешний QR-сервис на каждый повторный запрос фронта.

Результат работы:

<details>
<summary>Скриншоты интерфейса</summary>

<p>
  <img src="screenshots/photo_2026-04-05_08-52-14.jpg" alt="Главный экран Resume Vizor" width="32%" />
  <img src="screenshots/photo_2026-04-05_08-54-44.jpg" alt="Пользовательский сценарий Resume Vizor" width="32%" />
  <img src="screenshots/photo_2026-04-05_09-09-47.jpg" alt="Рабочий экран Resume Vizor" width="32%" />
</p>
  
</details>

### Проект 2 — Название
Краткая информация о проекте, ссылки, достижения.

## Образование и сертификаты
- Окончил 4 года обучения в РКСИ по специальности "Информационная безопасность в телекоммуникационных системах".

## Контакты
- *Email по работе:*

```
S73PANOW.WORK@yandex.ru
```

- *Telegram:*

```
@giraffick
```

- *VKontakte:* [профиль](https://vk.com/crickette)

---

<div align="center">
  <img src="gif/goodb.gif" alt="описание" />
</div>
