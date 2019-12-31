[Language abbreviations] in [Nutritive Value of Indian Foods 1989].

```javascript
const languages = require('@nvif1989/languages');
// languages.corpus: Map {abbr => {abbr, lang}}
// languages.load(): true (corpus loaded)
// languages.sql([table], [options]): sql commands
// languages.csv(): path of csv file
// languages(<query>)
// -> {abbr, lang} if supported, null otherwise.


languages.load();
/* load corpus first */

languages('b.');
languages('B.');
// { abbr: 'B.', lang: 'Bengali' }

languages('what is tel.?');
languages('Tel. stands for?');
/* (full stops must immediately follow character, if present) */
/* (for single character abbreviations, full stop is mandatory) */
// { abbr: 'Tel.', lang: 'Telgu' }
```


[![nvif1989](https://i.imgur.com/mGVou5c.png)](https://www.npmjs.com/package/nvif1989)
> You can ask about composition of 592 key foods in India here: [nvif1989.github.io].<br>
> Food composition values were measured by [National Institute of Nutrition, Hyderabad].<br>
> Take a peek at the raw data here: [Document], [Webpage].

[Nutritive Value of Indian Foods 1989]: https://www.icmr.nic.in/content/nutritive-value-indian-foods-nvif-c-gopalan-b-v-rama-sastri-sc-balasubramanian-revised
[Language abbreviations]: https://github.com/nvif1989/languages/blob/master/index.csv
[nvif1989.github.io]: https://nvif1989.github.io
[National Institute of Nutrition, Hyderabad]: https://www.nin.res.in/
[Document]: https://docs.google.com/spreadsheets/d/1C_4ueQcejgpl7ZtsknSU4ebXP4WIj37UG02BDzA28Ns/edit?usp=sharing
[Webpage]: https://docs.google.com/spreadsheets/d/e/2PACX-1vRcvpeU_qzsIUgYo6aWYoeEXehB4AZhxyDodF6AkRPvg5cUrhTv3uMVtDeWtSu_LuUDVtLO7ADAHdzi/pubhtml
