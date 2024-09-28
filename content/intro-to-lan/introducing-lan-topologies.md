---
title: Introducing LAN Topologies
---


# Topologie
## Topologia sieci
Schematyczny wygląd sieci komputerowej, określający sposób połączenia ze sobą urządzeń sieciowych. Topologia sieci określa sposób, w jaki urządzenia są połączone ze sobą, a także sposób, w jaki przesyłane są dane między nimi.

## Topologia gwiazdy (Star Topology)
Urządzenia końcowe są połączone z jednym centralnym urządzeniem, które nazywane jest hubem lub switchem. W topologii gwiazdy każde urządzenie jest połączone z centralnym urządzeniem za pomocą osobnego kabla.

> [!warning] Uwaga!
> - W przypadku awarii centralnego urządzenia, cała sieć przestaje działać.

W przypadku awarii jednego z urządzeń, pozostałe urządzenia w sieci **nie** są na to narażone.
![Obrazek przedstawiający schematyczny wygląd topologii gwiazdy](/intro-to-lan/images/star-topology.png)

## Topologia magistrali (Bus Topology)
W topologii magistrali wszystkie urządzenia są połączone z jednym kablem, który jest podzielony na sekcje, z których każda sekcja jest połączona z jednym urządzeniem.

> [!warning] Uwaga!
> - W przypadku przerwania kabla, cała sieć przestaje działać.
> - Sieć można przeciążyć w prosty sposób.

![Obrazek przedstawiający schematyczny wygląd topologii magistrali](/intro-to-lan/images/bus-topology.png)

## Topologia pierścienia (Ring Topology)
W topologii pierścienia każde urządzenie jest połączone z dwoma innymi urządzeniami, tworząc zamknięty pierścień. Dane przesyłane są w jednym kierunku, od jednego urządzenia do drugiego.

> [!warning] Uwaga!
> - W razie przerwania połączenia między dwoma urządzeniami, cała sieć przestaje działać.

![Obrazek przedstawiający schematyczny wygląd topologii pierścienia](/intro-to-lan/images/ring-topology.png)

## Podsumowanie
| Topologia | Zalety | Wady |
| --- | --- | --- |
| Gwiazdy | - łatwa w konfiguracji | - awaria centralnego urządzenia |
| | - łatwa w diagnostyce | |
| | - łatwa w rozbudowie | |
| Magistrali | - łatwa w konfiguracji | - awaria kabla |
| | - tania | - przeciążenie sieci |
| | - łatwa w rozbudowie | |
| Pierścienia | - łatwa w konfiguracji | - awaria połączenia między dwoma urządzeniami |
| | - łatwa w diagnostyce | |
| | - łatwa w rozbudowie | |

# Co to jest switch?
To urządzenia sieciowe, które łączą wiele urządzeń (np.: komputery, drukarki) używając Ethernetu.
Powszechnie spotykane są w dużych sieciach biznesowych, lub szkolnych. Mają wiele portów (4, 8, 16, 32, 64).
W odróżnieniu od Huba, switch wie jakie urządzenie jest podłączone do którego portu, i przesyła dane tylko do odpowiedniego urządzenia, co znacznie zwiększa wydajność sieci.