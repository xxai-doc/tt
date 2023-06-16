<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

# xxAI.art

Вебсайт кодының бер өлеше ачык чыганак, тәрҗемәне оптимальләштерергә ярдәм итегез.

## алгы код

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
