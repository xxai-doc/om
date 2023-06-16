<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

Dura nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) , fi sana booda `direnv allow` erga galmee seentee booda fe'uun ni gorfama ( [.envrc](https://github.com/xxai-art/doc/blob/main/.envrc) erga galmee seenee booda ofumaan raawwatama).

Hiikni isaas: Hiika Chaayinaa gara Jaappaan, Kooriyaa, Ingiliffaa, Ingiliffaa afaanota biroo hundaatti hiikuu. Yoo Chaayinaa fi Ingiliffa qofa deeggaru barbaadde, `zh: en` qofa barreessuu dandeessa.

Hiikni isaas: Hiika Chaayinaa gara Jaappaan, Kooriyaa, Ingiliffaa, Ingiliffaa afaanota biroo hundaatti hiikuu. Yoo Chaayinaa fi Ingiliffa qofa deeggaru barbaadde, `zh: en` qofa barreessuu dandeessa.

* [koodii fuulduraa](https://github.com/xxai-art/web)
* [Paakkii afaanii akka waliigalaatti marsariitichaaf](https://github.com/xxai-art/web/tree/main/i18n)
* [Paakkii afaanii moojuulota seensaaf](https://github.com/wacpkg/user/tree/main/ui.i18n)
* [Weebsaayitii Dokumantarii Afaanota Hedduu](https://github.com/xxai-doc)

Afaan sagantaa fuulduraa [@w5/coffee_plus](http://npmjs.com/@w5/coffee_plus) dha, kunis amaloota tokko tokko kan itti dabalu yoo ta'u, kunis walnyaatinsa iskiriiptii coffee irratti hundaa'a, [./coffee_plus.md](./coffee_plus.md) ilaali.

## Weebsaayitii fi sanadoota idil-addunyaa gochuu

Pirojektoota 3 armaan gadii irratti ijaaraa

* [@w5/mdt jedhamuun beekama](https://www.npmjs.com/package/@w5/mdt)

  Fufichi `.mdt` dha, faayilii alaa eeruuf sintaksii `<+ ./coffee_plus/import.js>` wajjin walfakkaatu fayyadamuu dandeessa, fi xumura `.md` tiin mallattoo gadi bu'uu uumuu dandeessa.

* [@w5/trmd jedhamuun beekama](https://www.npmjs.com/package/@w5/trmd)

  Hiikkaan Markdown koodii fi hidhannoo hin hiiku, himoota hiikamanis ni kuusa. Yoo hiikni fooyya'e garuu barreeffamni jalqabaa hin fooyya'in, irra deebi'ee raawwachuun fooyya'iinsa hiikkaa irra hin barreessu.

* [@w5/i18n irratti](https://www.npmjs.com/package/@w5/i18n)

  Faayilota afaanii marsariitiiwwan `yaml` uumaman hiikuuf.

### Qajeelfama Ofumaan Hiikkaa Sanadaa

Kuusaa koodii [xxai-art/doc](https://github.com/xxai-art/doc) ilaali

Dura nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) , fi sana booda `direnv allow` erga galmee seentee booda fe'uun ni gorfama ( [.envrc](https://github.com/xxai-art/doc/blob/main/.envrc) erga galmee seenee booda ofumaan raawwatama).

Bu'uura koodii guddaa gara afaanota dhibbaan lakkaa'amaniitti hiikame akka hin uumamneef, tokkoon tokkoon afaaniif bu'uura koodii adda ta'e uumeera, dhaabbata bu'uura koodii kuusuudhaaf uume

Jijjiiramaa naannoo `GITHUB_ACCESS_TOKEN` saaguun fi sana booda [create.github.coffee](https://github.com/xxai-art/doc/blob/main/create.github.coffee) hojjechuun ofumaan kuusaa koodii uuma.

Dhugaadha, bu'uura koodii keessas kaa'uu dandeessa.

Wabii iskiriiptii hiikkaa [run.sh](https://github.com/xxai-art/doc/blob/main/run.sh)

Koodiin iskiriiptii akka armaan gadiitti hiikama:

[bunx](https://bun.sh/docs/cli/bunx) bakka bu'aa npx ti, kunis saffisaa dha. Dhugaadha, yoo bun installed hin qabne ta'e, bakka isaa `npx` fayyadamuu dandeessa.

`bunx mdt zh` `.mdt` galmee zh keessatti akka `.md` agarsiisa, faayilii 2 walitti hidhaman armaan gadii ilaali

* [buna_dabalata.mdt](https://github.com/xxai-doc/zh/blob/main/coffee_plus.mdt)
* [buna_dabalata.md](https://github.com/xxai-doc/zh/blob/main/coffee_plus.md)

`bunx i18n` koodii ijoo hiikkaa ti (yoo `nodejs` qofa fe'ame qabaatte, garuu `bun` fi `direnv` hin fe'amne, hiikuuf `npx i18n` hojjechuus dandeessa).

Inni [i18n.yml](https://github.com/xxai-art/doc/blob/main/i18n.yml) ni parse , qindeessaan `i18n.yml` galmee kana keessatti akka armaan gadiitti:

```
en:
zh: ja ko en
```

Hiikni isaas: Hiika Chaayinaa gara Jaappaan, Kooriyaa, Ingiliffaa, Ingiliffaa afaanota biroo hundaatti hiikuu. Yoo Chaayinaa fi Ingiliffa qofa deeggaru barbaadde, `zh: en` qofa barreessuu dandeessa.

Inni dhumaa [gen.README.coffee](https://github.com/xxai-art/doc/blob/main/gen.README.coffee) dha, kunis qabiyyee mata duree ijoo fi mata duree xiqqaa jalqabaa afaan tokkoon tokkoo `README.md` gidduu jiru baasee galtee `README.md` maddisiisa. Koodiin baayyee salphaadha, ofuma keessanii ilaaluu dandeessu.

Google APIn hiikkaa bilisaaf fayyadama. Yoo Google argachuu hin dandeenye, maaloo bakka bu'aa qindeessii saagi, kan akka:

```
export https_proxy=http://127.0.0.1:7890 http_proxy=http://127.0.0.1:7890 all_proxy=socks5://127.0.0.1:7890
```

Iskiriiptiin hiikkaa galmee `.i18n` keessatti kaachota hiikame ni uuma, maaloo `git status` waliin ilaalii fi hiikkaa irra deddeebi'amee akka hin raawwatamneef gara kuusaa koodiitti dabali.

Maaloo yeroo hunda hiikkaa fooyyessitee kaachota haaromsuuf `bunx i18n` hojjedhu.

Yoo barreeffamni jalqabaa fi hiikni yeroo tokkotti fooyya'e, kaachoon ni burjaaja'a, kanaaf yoo fooyyessuu barbaadde tokko qofa fooyyessuu dandeessa, sana booda `bunx i18n` fiiguun kaachicha haaromsuu dandeessa.
