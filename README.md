<html>
  <head>
    <script>
      function onSubmit(token) {
        alert('thanks ' + document.getElementById('field').value);
      }

      function validate(event) {
        event.preventDefault();

        if (!document.getElementById('field').value) {
          alert('You must add text to the required field');
        } else {
          hcaptcha.execute();
        }
      }

      function onLoad() {
        var element = document.getElementById('submit');

        element.onclick = validate;
      }
    </script>
    <script src="https://js.hcaptcha.com/1/api.js?onload=onLoad" async defer></script>
  </head>
  <body>
    <form>
      Name: (required) <input id="field" name="field" />
      <div
        id="hcaptcha"
        class="h-captcha"
        data-sitekey="your_site_key"
        data-callback="onSubmit"
        data-size="invisible"
      ></div>
      <button id="submit">submit</button>
    </form>
  </body>
</html>{
   "theme": "dark",
   "size": "compact",
   "sitekey": "your_site_key"
}<script type="text/javascript">
  hcaptcha.render('captcha-1', {
    sitekey: 'your_site_key',
    theme: 'dark',
    'error-callback': 'onError',
  });
   </script><div
  class="h-captcha"
  data-sitekey="your_site_key"
  data-theme="dark"
  data-error-callback="onError"
></div>08.12.2023 - 11:16 ID Título Personal Bonus Requisitos Cumplidos Cantidad 30.00 M$ Moneda MXN Válido Hasta 09.12.2023 - 11:16 Tipo Bono08.12.2023 - 10:58 ID Título Personal Free Spins Jugado Cantidad 20.00 Moneda Válido Hasta 09.12.2023 - 11:04 Tipo Giro Gratis<script
  src="https://js.hcaptcha.com/1/api.js?onload=yourFunction&render=explicit"
  async
  defer
></script>6a4aa10d488d8a0a260e212d2042408aa1b51b18a0a0ca8c4108.12.2023 - 12:13 ID 767234715804710078 Sistema De Pago SPEI Cantidad 500.00 M$ Acción Retirar![Screenshot_20231209_205031_Chrome](https://github.com/hCaptcha/hcaptcha-integrations-list/assets/152949710/102bface-a35e-4723-9236-065eed307a03)
# hCaptcha integrations list
A collection of all known integration packages for hCaptcha.

**This is a community-maintained list.** Added or found another one? Open a PR to submit it!

Instructions: run `npm install`, edit README.md, then run `./upd_toc.sh` to re-create the TOC.
(Please maintain alpha-sort order.)

## Table of Contents

<!-- toc -->

- [Frontend](#frontend)
  * [JavaScript](#javascript)
    + [Angular](#angular)
    + [Ember.js](#emberjs)
    + [Plain JS reference](#plain-js-reference)
    + [Preact](#reactjs)
    + [ReactJS](#reactjs)
    + [Vanilla JS (use with Angular, Vue, etc)](#vanilla-js-use-with-angular-vue-etc)
    + [Vue JS](#vue-js)
    + [SolidJS](#solidjs)
- [Backend](#backend)
  * [AdonisJS middleware](#adonisjs-middleware)
  * [Cloudflare Worker siteverify](#cloudflare-worker-siteverify)
  * [curl](#curl)
  * [Elixir](#elixir)
  * [Firebase App Check (hCaptcha as Custom Provider)](#firebase-app-check-hcaptcha-as-custom-provider)
  * [Go middleware](#go-middleware)
  * [Go-hCaptcha](#go-hcaptcha)
  * [Java](#java)
  * [Laravel](#laravel)
  * [Next.js API Routes](#nextjs-api-routes)
  * [node.js](#nodejs)
  * [Plain PHP](#plain-php)
  * [Python: Django](#python-django)
  * [Python: Django + Crispy](#python-django--crispy)
  * [Python: Flask](#python-flask)
  * [Ruby/Rails](#rubyrails)
  * [Rust](#rust)
- [Serverless Backend](#serverless-backend)
  * [Cloudflare: Rust](#cloudflare-rust)
  * [Cloudflare: JS](#cloudflare-js)
  * [Fastly: Rust](#fastly-rust)
- [Native Integrations: CMS platforms](#native-integrations-cms-platforms)
  * [MyBB](#mybb)
  * [XenForo](#xenforo)
- [Plugins](#plugins)
  * [Craft CMS](#craft-cms)
    + [Freeform Plugin](#freeform-plugin)
  * [Drupal](#drupal)
  * [Invision Community](#invision-community)
  * [Joomla](#joomla)
    + [Joomla RSForm!Pro Plugin](#joomla-rsformpro-plugin)
  * [Magento](#magento)
  * [MediaWiki](#mediawiki)
  * [OXID eShop](#oxid-eshop)
  * [phpBB](#phpbb)
  * [Plone](#plone)
    + [Volto Form Block](#volto-form-block)
  * [SMF](#smf)
  * [Silverstripe](#silverstripe)
  * [Symfony](#symfony)
  * [Typo3](#typo3)
  * [Umbraco](#umbraco)
    + [UmbracoForms.uCaptcha](#umbracoformsucaptcha)
  * [Vanilla Forums](#vanilla-forums)
  * [WordPress](#wordpress)
    + [WordPress WPForms Plugin](#wordpress-wpforms-plugin)
  * [XenForo](#xenforo-1)
  * [Kentico Xperience](#kentico-xperience)
- [Chat protection bots](#chat-protection-bots)
    + [Honk](#honk)
  * [Telegram](#telegram)
- [Mobile apps](#mobile-apps)
  * [iOS](#ios)
  * [Android](#android)
  * [React Native](#react-native)
  * [Flutter](#flutter)
- [Access Management Platforms](#access-management-platforms)
  * [ForgeRock](#forgerock)
- [More](#more)
  * [.NET and ASP.NET Core](#net-and-aspnet-core)
  * [RoundCube](#roundcube)
  * [Salesforce VFP (Aura)](#salesforce-vfp-aura)

<!-- tocstop -->

## Frontend

### JavaScript

#### Angular
[hCaptcha Component Library for Angular](https://github.com/leNicDev/ng-hcaptcha)

#### Ember.js
[hCaptcha Component Library for Ember.js](https://github.com/sinankeskin/ember-h-captcha)

#### Plain JS reference
[Official docs](https://docs.hcaptcha.com/)

#### ReactJS
[hCaptcha Component Library for ReactJS](https://github.com/hCaptcha/react-hcaptcha)

Note: also supports Preact.

#### Vanilla JS (use with Angular, Vue, etc)
[Source](https://github.com/DSergiu/vanilla-hcaptcha)
[NPM](https://www.npmjs.com/package/vanilla-hcaptcha)

#### Vue JS
[hCaptcha Component Library for Vue.js](https://github.com/hCaptcha/vue-hcaptcha)

#### SolidJS
[hCaptcha Component Library for Solid](https://github.com/Vexcited/solid-hcaptcha)

## Backend

### AdonisJS middleware
[Code](https://github.com/NerdyLuffy/adonisjs-hcaptcha)

### Cloudflare Worker siteverify
[Code](https://github.com/glenstack/glenstack/tree/master/packages/cf-workers-hcaptcha)

### curl
[Official docs](https://docs.hcaptcha.com/#server)

### Elixir
[Hex](https://hex.pm/packages/hcaptcha)

### Firebase App Check (hCaptcha as Custom Provider)
[Full example](https://github.com/firebase/firebase-js-sdk/discussions/5095)

### Go middleware
[Source](https://github.com/kataras/hcaptcha)

### Go-hCaptcha
[Source](https://github.com/ross714/hcaptcha)  
[Full example](https://github.com/ross714/hcaptcha/tree/main/examples/fiber)

### Java
[Blog with source](https://golb.hplar.ch/2020/05/hcaptcha.html)

### Laravel
[Full example blog with source](https://serversideup.net/laravel-hcaptcha-custom-validation-rule/)

#### Packages

- [codise/hclaravel](https://github.com/tojorodialson/hc-laravel)
- [scyllaly/hcaptcha](https://github.com/Scyllaly/hcaptcha)
- [buzz/laravel-h-captcha](https://github.com/thinhbuzz/laravel-h-captcha)
- [rvxlab/hcaptcha](https://github.com/rvxlab/hcaptcha)

### Next.js API Routes
[npm Package](https://www.npmjs.com/package/next-hcaptcha)  
[GitHub Repository](https://github.com/neg4n/next-hcaptcha)

### node.js
[npm Package](https://www.npmjs.com/package/hcaptcha)

### Plain PHP
[Full example blog with source](https://medium.com/@hCaptcha/using-hcaptcha-with-php-fc31884aa9ea)

### Python: Django
[Source](https://github.com/tiesjan/django-hcaptcha-field)  
[PyPI](https://pypi.org/project/django-hcaptcha-field/)

### Python: Django + Crispy
[Blog post with source](https://medium.com/python-in-plain-english/how-to-add-hcaptcha-to-your-django-crispy-form-and-be-more-privacy-conscious-273e7f39bbfd)

### Python: Flask
[Source](https://github.com/KnugiHK/flask-hcaptcha)  
[PyPI](https://pypi.org/project/Flask-hCaptcha/)

### Ruby/Rails
[RubyGems](https://rubygems.org/gems/hcaptcha)  
[Source](https://github.com/Nexus-Mods/hcaptcha)

### Rust
[Source](https://github.com/jerusdp/hcaptcha-rs)

## Serverless Backend

### Cloudflare: Rust

[hCaptcha verify endpoint using Cloudflare Workers written in Rust](https://github.com/rodneylab/hcaptcha-serverless-rust-worker)

### Cloudflare: JS

[NPM package: Verify a hCaptcha token from within a Cloudflare Worker.](https://github.com/glenstack/glenstack)

### Fastly: Rust

[hCaptcha Serverless on Fastly Compute@Edge (Rust)](https://github.com/JAR33/hcaptcha-fastly-compute)


## Native Integrations: CMS platforms

### MyBB
Starting from verison 1.8.23: [Docs](https://docs.mybb.com/1.8/administration/spam/#captcha-images-for-registration--posting) & [Release Notes](https://mybb.com/versions/1.8.23/)

### XenForo
Starting from version 2.2: [Announcement](https://xenforo.com/community/posts/1437264)

### Kentico Xperience

[hCaptcha Kentico Xperience Form Component](https://github.com/wiredviews/xperience-hcaptcha)

## Plugins

### Craft CMS

[Plugin](https://plugins.craftcms.com/craft-hcaptcha)
[Source](https://github.com/c10d-dev/craft-hcaptcha)

#### Freeform Plugin

[Plugin](https://plugins.craftcms.com/freeform)
[Source](https://github.com/solspace/craft3-freeform)

### Drupal
[Plugin](https://www.drupal.org/project/hcaptcha)

### Invision Community
[Plugin](https://invisioncommunity.com/files/file/9657-hcaptcha-integration/)

### Joomla

[Source](https://github.com/pe7er/hCaptcha)
[Extension](https://extensions.joomla.org/extension/hcaptcha/)

#### Joomla RSForm!Pro Plugin

[Extension](https://www.rsjoomla.com/support/documentation/rsform-pro/plugins-and-modules/plugin-hcaptcha-spam-protection-.html)

### Magento

[Plugin](https://magecomp.com/magento-2-hcaptcha.html)

### MediaWiki

[Plugin](https://www.mediawiki.org/wiki/Extension:ConfirmEdit#hCaptcha)
[Source](https://gerrit.wikimedia.org/r/mediawiki/extensions/ConfirmEdit)

### OXID eShop

[Plugin](https://packagist.org/packages/tremendo/oxid-hcaptcha)
[Source](https://github.com/KalteSterne/oxid-hcaptcha)

### phpBB
[Extension](https://www.phpbb.com/customise/db/extension/hcaptcha/)

### Plone

[Plugin](https://github.com/plone/plone.formwidget.hcaptcha)

#### Volto Form Block

[Volto form add-on](https://github.com/collective/volto-form-block)

### SMF

[Add-on](https://custom.simplemachines.org/mods/index.php?mod=4255)


### Silverstripe

[Plugin](https://packagist.org/packages/oposs/silverstripe-hcaptcha)
[Source](https://github.com/oposs/silverstripe-hcaptcha)

### Symfony

[Source](https://github.com/Meteo-Concept/hcaptcha-bundle)
[Symfony/flex recipe](https://github.com/symfony/recipes-contrib/pull/979)

### Typo3

[Blog post](https://susi.dev/hcaptcha)
[Typo3 extension](https://extensions.typo3.org/extension/hcaptcha/)

### Umbraco

#### UmbracoForms.uCaptcha

[Source](https://github.com/AaronSadlerUK/UmbracoForms.uCaptcha)
[Plugin](https://our.umbraco.com/packages/website-utilities/umbracoformsucaptcha/)
[NuGet](https://www.nuget.org/packages/AaronSadler.uCaptcha/)

### Vanilla Forums
[Plugin](https://open.vanillaforums.com/addon/hcaptcha-plugin)
[Source](https://github.com/unkorneglosk/hcaptcha)

### WordPress
[Plugin](https://wordpress.org/plugins/hcaptcha-for-forms-and-more/)
[Source](https://github.com/hCaptcha/hcaptcha-wordpress-plugin)

#### WordPress WPForms Plugin
[Native integration: instructions to enable](https://wpforms.com/docs/how-to-set-up-and-use-hcaptcha-in-wpforms/)

### XenForo

[Add-on](https://xenforo.com/community/resources/hcaptcha-integration.7696/)
[Source](https://github.com/ticktackk/hCaptchaIntegrationForXF2)

## Chat protection bots

#### Honk
[source](https://github.com/KeithPatrick5/hcaptcha-honk-bot)

### Telegram
[Blog post + code](https://medium.com/@hCaptcha/fight-spam-on-your-telegram-group-with-hcaptcha-2bab3efc34b3)

## Mobile apps

### iOS

[iOS Native SDK](https://github.com/hCaptcha/HCaptcha-ios-sdk)

### Android

[Android Native SDK](https://github.com/hCaptcha/hcaptcha-android-sdk)

### React Native

[React Native integration](https://github.com/hCaptcha/react-native-hcaptcha)

### Flutter
[Flutter example with source blog post](https://medium.com/@hCaptcha/implementing-hcaptcha-in-your-flutter-app-13ea6ddca71b)

## Access Management Platforms

### ForgeRock
[Access Management: CAPTCHA Node config instructions](https://backstage.forgerock.com/docs/am/7/authentication-guide/auth-node-configuration-hints.html#auth-node-captcha)

## More

### .NET and ASP.NET Core
[source](https://github.com/BenjaminAbt/hcaptcha)

### RoundCube
[source](https://github.com/NeverBehave/rc_hcaptcha)

### Salesforce VFP (Aura)
[source](https://github.com/chrisludovice/SFDX_hCaptcha)
<html>
  <head>
    <script>
      function onSubmit(token) {
        alert('thanks ' + document.getElementById('field').value);
      }

      function validate(event) {
        event.preventDefault();

        if (!document.getElementById('field').value) {
          alert('You must add text to the required field');
        } else {
          hcaptcha.execute();
        }
      }

      function onLoad() {
        var element = document.getElementById('submit');

        element.onclick = validate;
      }
    </script>
    <script src="https://js.hcaptcha.com/1/api.js?onload=onLoad" async defer></script>
  </head>
  <body>
    <form>
      Name: (required) <input id="field" name="field" />
      <div
        id="hcaptcha"
        class="h-captcha"
        data-sitekey="your_site_key"
        data-callback="onSubmit"
        data-size="invisible"
      ></div>
      <button id="submit">submit</button>
    </form>
  </body>
</html>💫 Are you ready to add joy to your week? 
We have just what you need - our weekly raffle

Subscribe to Instagram or Twitter to enter a $50 drawing each week💸

Don't miss out on this exciting opportunity to win some extra cash while playing your favorite games

CATCH THE PROMO CODE👇
- Promo Code: 5H9W37ch
- Value: $5
- Requirement: 2500$ wagered in the last 7 days
- Total Drop Limit: 50 activation

Best of luck 💥 Play and win 👉 COINS.GAMEhttps://swc.page.link/?link=https://sweatco.in/loves/jesusflores63643067787?channel%3Dother%26feature%3Dinvite%26inviter_id%3D150125337%26inviter_name%3DJesus%2520Flores&apn=in.sweatco.app&isi=971023427&ibi=swc&ius=swc&ct=invite_other&pt=117705952&_icp=10xb4b9dc1c77bdbb135ea907fd5a08094d98883a35https://t.me/coins_game/1131646180333100000003up8xhzz6461802609045506310657 1308 0166 5808.12.2023 - 12:11 ID 836084715674480784 Sistema De Pago SPEI Cantidad 10.00 M$ Acción Retirar Pendiente1277 6501 3080 1665 8008.12.2023 - 12:13 ID 767234715804710078 Sistema De Pago SPEI Cantidad 500.00 M$ Acción Retirar Pendiente63818001014906415308.12.2023 - 12:25 ID 852054716542941853 Sistema De Pago SPEI Cantidad 500.00 M$ Acción Retirar Pendiente08.12.2023 - 12:25 ID 852054716542941853 Sistema De Pago SPEI Cantidad 500.00 M$ Acción Retirar Cancelado https://go9.pw/?referralCode=c4vx8vp https://go9.pw/?referralCode=c4vx8vphttps://t.me/c/2045234837/21646017206897166447RSBROW6+52 637 125 4467https://ninecasino.com/es670184954714864419098920646180260904576521
