# tcp-udp-scanner
Сканер TCP, UDP портов

Автор: `Ивашкин Роман, КН-204`

## Параметры запуска
```
usage: scanner.py [-h] [-p PORTS] target

positional arguments:
  target                Целевой адрес сканирования

optional arguments:
  -h, --help            show this help message and exit
  -p PORTS, --ports PORTS
                        Список портов для сканирования, указанных через ",";
                        можно указывать диапазон (80, 144, 2303-2400)
```

## Пример запуска

```
>python3 scanner.py -p 631,6942,53 127.0.0.1
Scanning 127.0.0.1...
631/tcp 	ipp 	open
6942/udp 	open
53/tcp 	closed
```