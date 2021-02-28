![OSSAR](https://github.com/macqael/AdGuard-Home-Filters/workflows/OSSAR/badge.svg)
# AdGuard-Home-Filters
Many list with ABP Syntax for AdGuard Home DNS blocking.

## AND what list do you use ?
This is the filter list i use :
- [Aelisya's Protection](https://raw.githubusercontent.com/macqael/AdGuard-Home-Filters/main/AdGuard-Home/Aelisya's-Protect-Basic.abp) (From this repo)
- [OISD](https://abp.oisd.nl/)

## Ok and the upstream DNS ?
For that i use unfiltered AdGuard :

    quic://dns-unfiltered.adguard.com

## And for the protocol ?
I use DoQ.

## EDNS ?
Yes i have enabled it since they support ECS (who don't send all the ip only the start).

## For the DNS priming servers ?
I use Quad9 the most secure DNS, if i don't use it to as upstream it's because there is many false positive.

Localhost :

    2620:fe::fe
    9.9.9.9

## And for the connection between the client and AdGuard ?
I use Dns Over Https because iPhone/Mac Os Bigsur have DOH support and Windows 10 Will have it too soon, and since i control the server (physically and software) i don't have to worry about cookies and history log or dns spoofing.

## Why is there adult website on allow list ?
It's often a mistake in my script who have missed to remove it (for instance XXX.com is locked but a new domain XXX.lol go through), after a report i add it and remove them from the list, you can report to website@bacq.pro

## And if i think there is a security concern with a witelisted website ?
Send a mail to security@bacq.pro

## Source
- [DMN - NEXTDNS](https://github.com/nextdns/metadata/)
- My own modification.
