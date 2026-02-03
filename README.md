## resolving-public ![GitHub last commit (branch)](https://img.shields.io/github/last-commit/you-oops-dev/resolving-public/main?style=plastic)

| File      | CIDR  | IP's| Total IP's | Size in memory (ipset)|Line in file | Size file (Mb)
|:----------:|:------------:|:------------:|:------------:|:------------:|:------------:|:------------:
|unblock_suite_ip.txt [RAW](https://raw.githubusercontent.com/you-oops-dev/resolving-public/main/unblock_suite_ip.txt)|13958|8658|103565562|0.61 Mb|22616|0.358 Mb
|unblock_suite_ip_ipset.txt [RAW](https://raw.githubusercontent.com/you-oops-dev/resolving-public/main/unblock_suite_ip_ipset.txt)|1993|7657|103857321|0.267 Mb|9650|0.152 Mb

Размер потребления (ОЗУ) приблизительна, потому что на разных хостах с одним тем же списком она разная погрешность потребления +- меньше 1-ого процента от указанного. 

***RUS:***

Описание:
В этих списках находятся адреса этих доменов из этого [списка](https://antizapret.prostovpn.org/domains-export.txt).
К ним добавлены подсети Meta (Instagram,Facebook,Whatsapp),Twitter,Google.
Некоторые CDN подсети для работы Spotify,Twitter.
Добавлены некоторые свои домена (весь список огласить не могу) например: [ReturnDislike](https://returnyoutubedislike.com) (включая их API),[SponsorBlock](https://sponsor.ajay.app) (и их резервное зеркало). 100 самых популярных (статический лист, c некоторыми правками убрал сайты из списка не относящиеся к adult категории) [сайтов](https://gist.githubusercontent.com/lord-alfred/9235861756400b9dd2593d727c31b0b1/raw/59b688029ebb44ebc4e36c64a024377dfd7b27c0/porn_sites.txt) для взрослых,[ChatGPT](https://chat.openai.com), Docker хаб с регистром. 

***Что исключается из списка?***

Подсети:

- **Яндекса**

- **Авито**

- **Rutube**

- **Beget**

- **Rambler**

- **Вконтакте**

- **Озон**

- **Alibaba**

- **GitHub**

- **Китайские IP-адреса** [country block IPs](https://raw.githubusercontent.com/herrbischoff/country-ip-blocks/master/ipv4/cn.cidr)

- **Публичные DNS-сервера (Google,CloudFlare,Yandex)**

- **Домена организаторов распространения информации** [список](https://reestr.rublacklist.net/api/v3/disseminators/)  
А точнее их адреса с некоторым исключением например из подсетей CloudFlare,DigitalOcean,Amazon такие адреса исключаются из списка ОРИ. Всякие Beget,TimeWeb идут на исключения из целевого списка.

- **Из [перечня](http://www.adm.nov.ru/page/38300) отечественных социально значимых**  
Выше указанные исключения работают и в этом случае.

- **Российские интернет-провайдеры (Корбина,Билайн,МТС,Ростелеком)**

- **Правительственные сайты или около правительственные сайты (например сайт МВД)**   
А точнее их адреса с некоторым исключением например из подсетей CloudFlare,DigitalOcean,Amazon такие адреса исключаются из списка ОРИ. Всякие Beget,TimeWeb идут на исключения из целевого списка. Таких сайтов мало, но они есть пару видел есстественно они не правительственные (gov).

- **Удалены СКАМ сайты,онлайн-казино и их зеркала,сайты по выдачи "левых" справок,сайты по вызову путан,сайты по покупке наркотических средств,алгоколя,табака. Удалена антивоенщина, политика. Удалены зеркала нормальных сайтов например резки вместо них оставленый 1-2 сайта обосную ниже почему я удалил.**

Хостера, которые находится в реестре распространения информациии (их подсети):

- **[WebHost1](https://webhost1.ru/)**

- **[RU-Center](https://www.nic.ru/)**

- **[DataCheap](https://datacheap.ru/)**

- **[Adman](https://adman.com/)**

- **[NTX](https://ntx.ru/)**

- **[IpServer](https://www.ipserver.su/ru)**

- **[TimeWeb](https://timeweb.com/ru/)**

- **[VDSina](https://vdsina.ru/)**

- **[IHC](https://www.ihc.ru/)**

- **[Biterika](https://www.biterika.com/)**

Банки (их подсети):

- **Сбербанк**

- **Альфа Банк**

- **Райффайзен**

- **Tinkoff**

- **Юmoney**

- **VTB**

- **Почта Банк**

- **Газпром Банк**

- **QIWI**

Во-первых среднестатистический пользователь не наркоман,порядочный семьянин (но и не святоша Фландерс =;) если где-то гуляет "на стороне", то делает это иными путями. Алкоголь и табак покупается в магазине. Все что ему нужно открыть рутрекер,включить Ютуб, и онлайн-кинотеатр, чтобы бесплатно посмотреть фильмы\сериалы. Вот секрет полного счастья.
Если кому-то не нравится моя политика добавляйте сами вручную. К тому же всем не угодить. Каждый удаленный домен этот как минимум -1 IP из списка, что позволяет разницу пустить совсем в другое русло+сокращение время на resolving доменов. Да, удалены не все домены, но разница уже в 27 тысяч доменов. Также могут попасть под раздачу невинные "сервисы\сайты" т.к удаляются регулярками sedом "с говорящим" вхождением casino,azino и т.д. Если такое произошло откройте Issues. Этот список предназначен для опытных пользователей, которые знаю куда его надо пихнуть чтобы все заработало. **Список впервую очередь для себя делался**, а потом уже для всех остальных.

Списки обновляются ***до 05:00*** по Москве (МСК +3) автоматически каждый день.
Также можно запустить вручную GitHub Action (нужна авторизация и учетная запись). И подождать часа 3+- где-то так.

**FAQ**:

**Q**: Почему два файла? В чем отличие?

**A**: Отличие ни в чем состоит,списки грубо говоря одинаковые. Просто утилита ipset при загоне unblock_suite_ip_ipset.txt за счет "грязной" суммаризации меньше памяти потребляет, но тут подхвох кроется засчет такой суммаризации могут присутствовать адреса из исключаемых подсетей. И общее количество IP-адресов больше чем в другом списке. Что позволяет использовать этот список с ipset на роутерах с 64Mb RAM (пока что).

**Q**: У меня подключен безлимит на социальные сети(Facebook,Instagram и т.д) будет ли работать безлимит?

**A**: ***НЕТ!!!*** К тому же они заблокированные какая тут будет без тариффикация траффика. К слову МТС вообще убрал данную опцию для подключения и это логично, потому, что заблочен, а пустите через прокси или VPN тарификация траффика будет. Во всех остальных случаях надо разбираться отдельно. YouTube сразу говорю тариффицироваться будет.   

**Q**: Что может не работать? Какие именно сайты?

**A**: Лично я проверял не работает мобильное приложение Facebook, но сайт браузерный работает. Также могут остаться заблокированные сайты т.к [nnmclub](https://nnmclub.to),[meduza](https://meduza.io) и т.д ,несмотря на то, что эти домены в списке и их адреса тоже в списке. Исключение составляет если у вас VPN-сервер в США тогда может и будет работать. В основном это сайты за CloudFlare, а этот CDN в данный момент не полностью добавлен не вся подсеть. Для работоспособности нужно самостоятельно добавить в список адреса этих доменов маску указываем /32. Ну пару сайтов не 10 тыс. =) основная работа моя выполнена.


## См. также репозитория:

https://github.com/you-oops-dev/ipranges

https://github.com/you-oops-dev/ipranges-shadowsocks

***ENG:***

Description:
These lists contain the addresses of these domains from this [list](https://antizapret.prostovpn.org/domains-export.txt).
Meta subnets (Instagram,Facebook,Whatsapp),Twitter,Google have been added to them.
Some CDN subnets to run Spotify,Twitter.
Some own domains have been added (I can't tell you the whole list) such as: [ReturnDislike](https://returnyoutubedislike.com) (including their API),[SponsorBlock](https://sponsor.ajay.app) (and their backup mirror).
The 100 most popular adult [websites](https://gist.githubusercontent.com/lord-alfred/9235861756400b9dd2593d727c31b0b1/raw/59b688029ebb44ebc4e36c64a024377dfd7b27c0/porn_sites.txt) (static list),[ChatGPT](https://chat.openai.com), Docker with registry.

***What is excluded from the list?***

Subnets:

- **Yandex**

- **Avito**

- **Rutube**

- **Timeweb**

- **vdsina**

- **beget**

- **Rambler**

- **Vkontakte**

- **Ozon**

- **Sberbank**

- **Alibaba**

- **Chinese IP addresses** [country block IPs](https://raw.githubusercontent.com/herrbischoff/country-ip-blocks/master/ipv4/cn.cidr)

- **Public DNS servers (Google,CloudFlare,Yandex)**

- **information dissemination organizers** [list](https://reestr.rublacklist.net/api/v3/disseminators/)

- **GitHub**

- **Russian ISPs (MTS, Beeline, Corbina, Rostelecom)**

- **Government Domain (Their IP addresses)** 

Lists are updated ***before 02:00*** (UTC 0) automatically every day.
You can also manually run GitHub Action (you need authorization and account). And wait 3+- hours or so.

## See also repository:

https://github.com/you-oops-dev/ipranges

https://github.com/you-oops-dev/ipranges-shadowsocks
