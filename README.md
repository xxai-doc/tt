<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

Башта nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) урнаштырырга киңәш ителә, аннары `direnv allow` ( [.envrc](https://github.com/xxai-art/doc/blob/main/.envrc) каталогка кергәннән соң автоматик рәвештә башкарылачак).

Мәгънәсе: Кытай, Япон, Корея, Инглиз, Инглиз телләренә тәрҗемә итү. Әгәр дә сез кытай һәм инглиз телләренә ярдәм итәсегез килсә, сез `zh: en` яза аласыз.

Мәгънәсе: Кытай, Япон, Корея, Инглиз, Инглиз телләренә тәрҗемә итү. Әгәр дә сез кытай һәм инглиз телләренә ярдәм итәсегез килсә, сез `zh: en` яза аласыз.

* [алгы код](https://github.com/xxai-art/web)
* [Тулаем алганда сайт өчен тел пакетлары](https://github.com/xxai-art/web/tree/main/i18n)
* [Логин модульләре өчен тел пакетлары](https://github.com/wacpkg/user/tree/main/ui.i18n)
* [Вебсайт күп телле документация](https://github.com/xxai-doc)

Алгы планлаштыру теле [@ w5 / coffee_plus](http://npmjs.com/@w5/coffee_plus) , ул кофескрипт синтаксисына нигезләнеп кайбер үзенчәлекләр өсти, кара [./coffee_plus.md](./coffee_plus.md) .

## Вебсайтларны һәм документларны интернационализацияләү

Түбәндәге 3 проектка нигез салыгыз

* [@ w5 / mdt](https://www.npmjs.com/package/@w5/mdt)

  Суффикс `.mdt` , сез тышкы файлларга мөрәҗәгать итү өчен `<+ ./coffee_plus/import.js>` синтаксисын куллана аласыз `.md` суффиксы белән билгеләр ясый аласыз.

* [@ w5 / trmd](https://www.npmjs.com/package/@w5/trmd)

  Маркдаун тәрҗемәсе кодларны һәм сылтамаларны тәрҗемә итмәячәк, һәм тәрҗемә ителгән җөмләләрне кэшлаячак. Әгәр дә тәрҗемә үзгәртелсә, ләкин оригиналь текст үзгәртелмәсә, аны яңадан башкару тәрҗемә модификациясен язмаячак.

* [@ w5 / i18n](https://www.npmjs.com/package/@w5/i18n)

  `yaml` ясалган вебсайтларны тәрҗемә итү өчен тел файллары.

### Документ тәрҗемәсен автоматлаштыру күрсәтмәләре

Код саклагычын карагыз [xxai-art / doc](https://github.com/xxai-art/doc)

Башта nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) урнаштырырга киңәш ителә, аннары `direnv allow` ( [.envrc](https://github.com/xxai-art/doc/blob/main/.envrc) каталогка кергәннән соң автоматик рәвештә башкарылачак).

Йөзләгән телләргә тәрҗемә ителгән зур код базасын булдырмас өчен, мин һәр тел өчен аерым код базасы булдырдым һәм код базасын саклаучы оешма булдырдым.

`GITHUB_ACCESS_TOKEN` әйләнә-тирә үзгәрүчене кую, аннары [create.github.coffee](https://github.com/xxai-art/doc/blob/main/create.github.coffee) белән эшләү автоматик рәвештә код саклагычын булдырачак.

Әлбәттә, сез аны код базасына да куя аласыз.

Тәрҗемә сценарийына сылтама [run.sh](https://github.com/xxai-art/doc/blob/main/run.sh)

Сценарий коды түбәндәгечә аңлатыла:

[bunx](https://bun.sh/docs/cli/bunx) - тизрәк булган npx өчен алмаштыру. Әлбәттә, бунка урнаштырылмаган булса, аның урынына `npx` куллана аласыз.

`bunx mdt zh` `.mdt` zh каталогында `.md` итеп күрсәтә, астагы 2 бәйләнгән файлны карагыз

* [кофе_плус.mdt](https://github.com/xxai-doc/zh/blob/main/coffee_plus.mdt)
* [кофе_плус.md](https://github.com/xxai-doc/zh/blob/main/coffee_plus.md)

`bunx i18n` - тәрҗемә итүнең төп коды (сездә `nodejs` гына урнаштырылган булса, `bun` һәм `direnv` урнаштырылмаган булса, сез тәрҗемә итү өчен `npx i18n` да эшли аласыз).

Бу [i18n.yml](https://github.com/xxai-art/doc/blob/main/i18n.yml) анализлаячак, бу документтагы `i18n.yml` конфигурациясе түбәндәгечә:

```
en:
zh: ja ko en
```

Мәгънәсе: Кытай, Япон, Корея, Инглиз, Инглиз телләренә тәрҗемә итү. Әгәр дә сез кытай һәм инглиз телләренә ярдәм итәсегез килсә, сез `zh: en` яза аласыз.

Соңгысы - [gen.README.coffee](https://github.com/xxai-art/doc/blob/main/gen.README.coffee) , ул төп исем белән һәр телнең `README.md` беренче субтитры арасындагы эчтәлекне чыгарып, `README.md` кертү өчен. Код бик гади, сез аңа үзегез карый аласыз.

Google API бушлай тәрҗемә өчен кулланыла. Әгәр дә сез Google'ка керә алмыйсыз икән, зинһар, прокси конфигурациясе һәм көйләгез, мәсәлән:

```
export https_proxy=http://127.0.0.1:7890 http_proxy=http://127.0.0.1:7890 all_proxy=socks5://127.0.0.1:7890
```

Тәрҗемә скрипты `.i18n` каталогында тәрҗемә ителгән кэш барлыкка китерәчәк, зинһар, аны `git status` белән тикшерегез һәм кабат-кабат тәрҗемә итмәс өчен код саклагычына өстәгез.

Зинһар, кэшны яңарту өчен тәрҗемәне үзгәрткән саен `bunx i18n` эшләгез.

Әгәр дә оригиналь текст һәм тәрҗемә бер үк вакытта үзгәртелсә, кэш буталачак, шуңа күрә үзгәртәсегез килсә, сез аны үзгәртә аласыз, аннары кэшны яңарту өчен `bunx i18n` эшли аласыз.
