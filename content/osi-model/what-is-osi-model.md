---
title: What is OSI Model?
---

# Co to jest OSI Model?

OSI Model to model warstwowy, który opisuje sposób, w jaki urządzenia sieciowe komunikują się ze sobą. Model ten składa się z siedmiu warstw, z których każda odpowiada za określone zadania.

# Jak brzmi rozwinięcie skrótu OSI?

**O**pen **S**ystems **I**nterconnection

# Dlaczego jest fajny?

Dzięki OSI Modelowi, inżynierowie sieci mogą zrozumieć, jak działa sieć komputerowa. Model ten pomaga również w diagnozowaniu problemów sieciowych.

Dotatkowo firmy mogą implementować różne rozwiązania po swojemu, ale dzięki OSI Modelowi, funkcjonowanie pozostaje przewidywalne.


# Z ilu warstw składa się OSI Model?

Składa się z siedmiu warstw.


# Co to jest enkapsulacja?

Enkapsulacja to proces, w którym dane są przesyłane przez kolejne warstwy modelu OSI. Każda warstwa dodaje swoje własne dane do pakietu, a następnie przekazuje go do kolejnej warstwy.

# Warstwy OSI Modelu

## Warstwa 7: Aplikacji (Application Layer)
Jest to warstwa, w której protokoły i zasady są w jednym miejscu, by określić sposób interakcji użytkownika z danymi wysłanymi lub odebranymi.

Codzienne aplikacje udostępniają przyjazny GUI (**G**raphical **U**ser **I**nterface) do interakcji z danymi wysłanymi lub odebranymi. Inne protokoły zawierają DNS (**D**omain **N**ame **S**ystem), który określa jak adresy stron internetowych są tłumaczone na adresy IP.

## Warstwa 6: Prezentacji (Presentation Layer)
Warstwa w której zachodzi standaryzacja. Na tej warstwie działa na przykład protokół HTTPS.

### Przykład
Każdy deweloper może utworzyć swój własny klient e-mail. Natomiast nie może to wpływać na treść wysłanej lub odebranej wiadomości.

## Warstwa 5: Sesji (Session Layer)
Sesja jest unikalna dla każdego połączenia. Jeśli połączenie zostało nawiązane miedzy komputerem A i B, to również utworzona została sesja. Dane w sesji są przesyłane w częściach (packets), by w razie utraty połączenia przesłać tylko te pakiety, które nie zostały odebrane.

Dane nie mogą podróżować między sesjami, mogą to robić tylko i wyłącznie wewnątrz pojedynczej sesji.

## Warstwa 4: Transportu (Transport Layer)
Kiedy dane są wysłane, mogą podróżować po jednym z dwóch różnych protokołów, w zależności od potrzeby.

### TCP
- Transmission Control Protocol (TCP).
- Stworzony z myślą o niezawodności i gwarancji.
- Rezerwuje stałe połączenie pomiędzy dwoma urządzeniami na czas trwania przesyłu i odbioru danych.
- Posiada weryfikację błędów w swoim designie. Poprzez weryfikację błędów TCP może zagwarantować, że małe części danych (packets) będą odebrane i złożone w tej samej kolejności.

### UDP
- User Datagram Protocol
- Stworzony do szybkiego przesyłu danych.
- Stworzony do transmisji wideo na żywo.
- Nie dba o to czy dane zostały odebrane w całości.

## Warstwa 3: Sieci (Network Layer)
W tej warstwie rozgrywa się kwestia routingu i doboru odpowiedniej ścieżki wysyłki pakietów.
Istnieją dwa protokoły, które optymalizują wysyłanie pakietów:
- OSPF (Open Shortest Path First),
- RIP (Routing Information Protocol).

Kwestie jakie są istotne przy doborze ścieżki, to:
- długość odcinka jaki pakiety muszą przebyć,
- czy ścieżka jest godna zaufania (tj. czy uprzednio pakiety nie zostały zgubione),
- czy połączenie fizyczne jest dobrej jakości (tj. czy występuje połączeni po kablu typu koncentryczny, czy może optyczny).

## Warstwa 2: Łącza danych (Data Link Layer)
W tej warstwie występuje adresowanie fizyczne na podstawie adresu MAC. Jak wiadomo adres MAC jest unikalny dla każdej karty sieciowej. Niestety da się go jednak spoofować. Każde urządzenie mające dostęp do internetu musi posiadać kartę sieciową.

## Warstwa 1: Fizyczna (Physical Layer)
Jest to warstwa dosłownie sprzętu. Najłatwiejsza do zobrazowania. To w niej przesyłane są kolejno pakiety przy pomocy impulsów elektrycznych, które odzwierciedlone są jako 0 i 1 (binarnie).