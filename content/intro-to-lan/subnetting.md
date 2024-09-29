---
title: Subnetting
---

# Co to jest subnetting?

Jest to termin określający podział sieci na mniejsze podsieci. Dzięki temu możliwe jest zwiększenie wydajności sieci, a także zwiększenie bezpieczeństwa.

## Przykład

Weź pod uwagę pracę w sporym przedsiębiorstwie. Podział w nim wygląda następująco:

- księgowość,
- finanse,
- human resources.

![Schemat przedstawiający subnetting dla przedsiębiorstwa składającego się z trzech działów](/intro-to-lan/images/subnetting.png)

Człowiek w prosty sposób będzie w stanie namierzyć odpowiedni dział, sieci również to widzą. Jednak administrator sieci musi odpowiednio skonfigurować podsieci, aby wszystko działało poprawnie.

# Budowa adresu IP

Adres IP składa się z czterech sekcji zwanych oktetami. To samo dotyczy maski podsieci. Każde oktet składa się z ośmiu bitów, co daje łącznie 32 bity, zasięg adresów IP to 0-255.

```
192.168.1.1
```

| Oktet 1 | .   | Oktet 2 | .   | Oktet 3 | .   | Oktet 4 |
| ------- | --- | ------- | --- | ------- | --- | ------- |
| 192     | .   | 168     | .   | 1       | .   | 1       |
| 0-255   | .   | 0-255   | .   | 0-255   | .   | 0-255   |

# Co wykorzystuje podsieć?

Podsieć wykorzystuje adres IP w trzech wariantach:

- identyfikacja adresu sieci,
- identyfikacja adresu hosta,
- identyfikacja bramy domyślnej.

# Co to jest adres sieci?

Adres sieci to adres IP, który identyfikuje sieć. Wszystkie urządzenia w danej podsieci mają ten sam adres sieci.

## Cel?

Określenie podsieci, w której znajduje się urządzenie.

## Wyjaśnienie

Przykładowo urządzenie z adresem IP `192.168.1.100` będzie w podsieci `192.168.1.0`.
