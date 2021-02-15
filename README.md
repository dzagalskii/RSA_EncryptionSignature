# Шифрование и проверка подписи RSA

## Настройка среды разработки
Данная программа была реализована на Anaconda 3 на языке программирования Python 3.
Для работы программы требуются библиотеки: asn1, pycryptodome. Остальные зависимости присутствуют в Anaconda 3.
Чтобы установить недостающие библиотеки, нужно выполнить следующие команды:
```
$ pip install asn1
$ pip install pycryptodome
```
## Немного о шифровании
В качестве вспомогательного симметричного алгооритма шифрвоания для RSA используется AES-256 CBC: шифрование файлов при помощи RSA нецелесообразно, поэтому RSA шифрует только ключ симметричного AES-256 CBC. ВНИМАНИЕ: синхропосылка CBC в данной работе состоит из 0. Это небезопасно и должно быть изменено на генерацию случайной синхропосылки, если данная программа будет использована не для демонстрационных целей.

## Немного о подписи
Для вычисления подписи используется алгоритм SHA-256.
