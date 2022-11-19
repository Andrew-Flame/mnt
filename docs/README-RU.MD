<div align=center style='text-align: center'>
    <img src='/images/logo.svg' width=20%/><br>
    <img src='https://img.shields.io/github/repo-size/Andrew-Flame/mnt?style=for-the-badge'/>
    <img src='https://img.shields.io/github/v/release/Andrew-Flame/mnt?style=for-the-badge'/>
    <img src='https://img.shields.io/github/license/Andrew-Flame/mnt?color=%230CD94E&style=for-the-badge'/><br>
    [<a href='/docs/README-EN.MD'>English</a>]
    [Русский]
</div>

# MNT
### Описание
'mnt' — это программа, которая позволяет быстро монтировать и размонтировать дисковые устройства в операционных системах на базе Linux. Это позволит вам сэкономить много времени при монтировании дисков в системах с графической средой или без нее.

### Установка
В корневом каталоге репозитория есть готовый скрипт, который установит программу за вас. Вам нужно только запустить его и следовать инструкциям:
```BASH
git clone https://github.com/Andrew-Flame/mnt.git
cd mnt
chmod +x install
./install
```

### Зависимости
- whiptail
- sudo

### Кастомизация
'mnt' — конфигурируемая программа программа. Расположение файла конфигурации ~/.config/mnt.ini
Вы можете настроить:
- Имя папки, в которую будет смонтирован каждый диск. Секция '[associations]':
  ```INI
  [associations]
  Disk C = C
  Disk I = I
  Disk H = H
  ```
- Отображение дисков в диалоговом окне. Секция '[display]':
  ```INI
  [display]
  # По умолчанию: ON
  Disk C = OFF
  Disk I = ON
  Disk H = ON
  ```
- Некоторые другие значения. Секция '[general]':
  ```INI
  [general]
  # Язык, на котором будет осуществляться вывод программы
  language = 'en'

  # Директория, куда будут монтироваться диски
  mountpoint = '/mnt'
  ```