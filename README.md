# [PrestaShop module "ZiZuu SEO ToolKit"](https://github.com/ZiZuu-store/zzSEOtk)

[![SensioLabsInsight](https://insight.sensiolabs.com/projects/30806e55-0fe6-4323-ade1-fba266db8b4e/mini.png)](https://insight.sensiolabs.com/projects/30806e55-0fe6-4323-ade1-fba266db8b4e)
[![GitHub issues](https://img.shields.io/github/issues/ZiZuu-store/zzSEOtk.svg?style=plastic)](https://github.com/ZiZuu-store/zzSEOtk/issues)

[![GitHub stars](https://img.shields.io/github/stars/ZiZuu-store/zzSEOtk.svg?style=social)](https://github.com/ZiZuu-store/zzSEOtk/stargazers)
[![Twitter](https://img.shields.io/twitter/url/https/github.com/ZiZuu-store/zzSEOtk.svg?style=social)](https://twitter.com/intent/tweet?text=Fantastic%20@PrestaShop%20module%20by%20@ZiZuu_Store:%20%22ZiZuu%20SEO%20ToolKit%22&url=https%3A%2F%2Fgithub.com%2FZiZuu-store%2FzzSEOtk)

[![Join the chat at https://gitter.im/ZiZuu-store/zzSEOtk](https://img.shields.io/badge/Gitter-CHAT%20NOW-brightgreen.svg?style=plastic)](https://gitter.im/ZiZuu-store/zzSEOtk?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)


Handles a few basic SEO related improvements such as:
* "hreflang"
* "canonical"
* "noindex"

Being reported to work on **PS >= 1.6.0.9** .. but it should work on PS 1.6.x.x too and *could work* on PS >= 1.5.0.1

For production use the **latest stable [release](https://github.com/ZiZuu-store/zzSEOtk/releases/)**

For developing or Pull Request please use only the **[dev](https://github.com/ZiZuu-store/zzSEOtk/tree/dev)** branch


## Canonical URLs

Insert the `<meta rel="canonical">` html tag to avoid content duplication

Query string is removed only when needed, pagination is retained and handled (an existing "prev/next" mechanism is needed, newer PS already does it)

## HrefLang

Handle multilingual sites.
Insert the `<meta rel="hreflang">` html tag, a default lang is handled too.

**hreflang meta is only added on canonical pages**, as explained in the following image and explained by [Eoghan Henn](http://www.rebelytics.com/hreflang-canonical/)

<img src="./hreflang-canonical-image.jpg">

## NoIndex

Automatically assure a `<meta robots="noindex">` tag is added to every PS controller that should not been indexed by search engines.
This allows for big "robots.txt" cleanup .. and a better SEO 

The phylosophy is "Don't use robots.txt to tell robots to do not index a page, it should be used to block them .. it's different"

# License

[LICENSE.md](LICENSE.md)
