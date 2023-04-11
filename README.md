# Verifica-Alimentazione-Raspberry
Dal terminale eseguire questo comando:
```
vcgencmd get_throttled
```
Verrà restituito a schermo il seguente codice:
```
111100000000000001010
||||             ||||_ under-voltage
||||             |||_ currently throttled
||||             ||_ arm frequency capped
||||             |_ soft temperature reached
||||_ under-voltage has occurred since last reboot
|||_ throttling has occurred since last reboot
||_ arm frequency capped has occurred since last reboot
|_ soft temperature reached since last reboot
```
Che verrà interpretato come segue:
```
0x0 significa che non sono presenti problemi.
0x50000 significa che si è verificato un rallentamento dall'ultimo riavvio.
0x50005 significa che il dispositivo è attualmente sotto tensione ed è instabile.
```
