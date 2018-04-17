## Programming is awesome!

- [設計](#設計)
- [C#](#c)
- [JavaScript](#javascript)
- [CSS・デザイン](#cssデザイン)
- [Webセキュリティ](#webセキュリティ)
- [開発環境](#開発環境)
- [DDD](#ddd)

# 設計

* [.NETの例外処理 Part.1](https://blogs.msdn.microsoft.com/nakama/2008/12/29/net-part-1/) - 例外と業務エラーの違い。
* [エンジニア必須の概念 – 契約による設計と信頼境界線](https://blog.ohgaki.net/design-by-contract-and-trust-boundary) - 『契約による設計(Design by Contract)』の考え方。

# C&#35;

* [C#の非同期の基礎](http://www.kekyo.net/2016/12/06/6186)
* [Top .NET Software Errors: 50 Common Mistakes and How to Fix Them](https://stackify.com/top-net-software-errors/) - C#でよくあるミス50例。
* [Do I need to use ConfigureAwait(false) all the way?](http://danielwertheim.se/do-i-need-to-use-configureawait-false-all-the-way/) - 「.ConfigureAwait(false)」はいつも付けないといけないの？という疑問に対する答え。
* [Loading .NET Assemblies out of Seperate Folders](https://weblog.west-wind.com/posts/2016/Dec/12/Loading-NET-Assemblies-out-of-Seperate-Folders) - 動的にアセンブリをロードする必要が出た時に（プラグイン機能の実装など）考慮すべき事柄など。コメントで言及されているMEF2はMSが公式に用意している手段。
* [gsscoder/commandline](https://github.com/gsscoder/commandline) - イケてるコマンドラインオプションパーサ。 - 使い方は [Wikiを参照](https://github.com/gsscoder/commandline/wiki/Quickstart)
* [Decimal vs Double and Other Tips About Number Types in .NET](https://www.exceptionnotfound.net/decimal-vs-double-and-other-tips-about-number-types-in-net/) - どんな時にどの数値型を使うか。
* [Running .NET Core apps on multiple frameworks and What the Target Framework Monikers (TFMs) are about](https://blogs.msdn.microsoft.com/cesardelatorre/2016/06/28/running-net-core-apps-on-multiple-frameworks-and-what-the-target-framework-monikers-tfms-are-about/) - .Net Coreアプリケーションで複数のフレームワークをサポートする時のproject.jsonの書き方やTFMの詳細。
* [Using dependency injection in a .Net Core console application](http://andrewlock.net/using-dependency-injection-in-a-net-core-console-application/) - DIをコンソールアプリケーションで利用する例＆StructureMapを利用する例。
* [Dependency Injection, Logging and Configuration In A .NET Core Console Application](http://pioneercode.com/post/dependency-injection-logging-and-configuration-in-a-dot-net-core-console-app?platform=hootsuite) - DIの他、.Net Coreの機能をフル活用するコンソールアプリケーションのボイラープレート。
* [Using strongly typed configuration in .NET Core console app](https://blogs.msdn.microsoft.com/fkaduk/2017/02/22/using-strongly-typed-configuration-in-net-core-console-app/) - ASP.Netでよくやる設定ファイルを型付で読み書きする仕組みはコンソールアプリでも使えるよ、という紹介。
* [Try catch, finally throw???or Exception Handling 101 for .NET](https://medium.com/@alexyakunin/try-catch-finally-throw-or-exception-handling-101-9f824136b21b) - 例外をどうやってハンドルするかという詳解。
* [Making string validation faster by not using a regular expression. A story.](https://blog.maartenballiauw.be/post/2017/04/24/making-string-validation-faster-no-regular-expressions.html) - 正規表現の最適化テクニック。
* [Learn Productivity Tips and Tricks for the Debugger in Visual Studio](https://docs.microsoft.com/en-us/visualstudio/debugger/debugger-tips-and-tricks) - Visual Studioのデバッグテクニック。
* [Enums.Net](https://github.com/TylerBrinkley/Enums.NET) - 便利なEnum。

## LINQ

* [A Visual Lexicon of LINQ](https://www.simple-talk.com/dotnet/net-development/visual-lexicon-linq/) - LINQの辞書。
* [LINQの拡張メソッド一覧と、ほぼ全部のサンプルを作ってみました。](http://d.hatena.ne.jp/chiheisen/20111031/1320068429) - 日本語サンプル。

## NuGet

* [NuGetパッケージの作り方、或いはXmlエディタとしてのVisual Studio](http://neue.cc/2011/01/22_298.html)
* [Creating Nuget Packages](https://blogs.msdn.microsoft.com/mvpawardprogram/2016/06/28/creating-nuget-packages/)

## ASP.Net Core

* [Testing SSL in ASP.Net Core](http://wildermuth.com/2016/10/26/Testing-SSL-In-ASP-NET-Core)
* [ASP.NET Core + Dapper で高パフォーマンスWEB開発を実践する ](http://kikki.hatenablog.com/entry/2016/10/26/100604) - DAOをDIでインスタンス化する例。
* [Bare metal APIs with ASP.NET Core MVC](http://benfoster.io/blog/bare-metal-apis-with-aspnet-core-mvc) - ピュアでフットプリントの小さいWeb APIサービスを作るテクニック。（Web APIを作りたいだけなのに）「.AddMvc()」とすると、不要なライブラリも参照されてしまうのでこれを「.AddMvcCode()」に替える。
* [An introduction to ViewComponents](https://andrewlock.net/an-introduction-to-viewcomponents-a-login-status-view-component/) - ViewComponentの性質や使い方。
* [Getting Down to Business Building an ASP.NET Core API Service](http://www.codemag.com/Article/1701061) - Web APIサービスを作る、実践的で詳細なチュートリアル。
* [Building microservices with ASP.NET Core (without MVC)](http://www.strathweb.com/2017/01/building-microservices-with-asp-net-core-without-mvc/) - 超軽量のマイクロサービスの記述例。
* [ASP.NET Core Dependency Injection Deep Dive](https://joonasw.net/view/aspnet-core-di-deep-dive) - DIの詳細。
* [Understanding Middleware in ASP.NET Core](http://myview.rahulnivi.net/understanding-middleware-asp-net-core/) - Middlewareの実装方法詳細やTips。パート3までアリ。
* [How to Trap Uncaught Exceptions and Avoid 5xx Errors in ASP.Net WebAPI](https://blogs.msdn.microsoft.com/timomta/2017/03/04/how-to-trap-uncaught-exceptions-and-avoid-5xx-errors-in-asp-net-webapi/) - うっかり5xxを返してしまわない方法。
* [Sensitive Configuration Data in ASP.NET Core](https://codeopinion.com/sensitive-configuration-data-asp-net-core/) - パスワード等の、gitにはつっ込みたくない情報を管理するUserSecretsの使い方。
* [Support multiple versions of ASP.NET Core Web API](http://www.talkingdotnet.com/support-multiple-versions-of-asp-net-core-web-api/) - Web APIで複数バージョンのAPIを同時にサポートするテクニック。
* [View Components with ASP.NET Core 1.1](https://csharp.christiannagel.com/2017/02/28/viewcomponents/) - ASP.Net Core 1.1で高機能になったViewComponentの解説。
* [Using LocalDB with Full IIS, Part 1: User Profile](https://blogs.msdn.microsoft.com/sqlexpress/2011/12/08/using-localdb-with-full-iis-part-1-user-profile/) - IISでSQL Server localdbを使うための細かい作業。
* [Running multiple independent ASP.NET Core pipelines side by side in the same application](https://www.strathweb.com/2017/04/running-multiple-independent-asp-net-core-pipelines-side-by-side-in-the-same-application/) - 超絶技巧

### ロギング

* [Error Handling in ASP.NET Core](https://dusted.codes/error-handling-in-aspnet-core) - ASP.Net Coreでのエラーハンドリングの基本的な考え方。
* [Best Practices for Error Handling in ASP.NET MVC](https://stackify.com/aspnet-mvc-error-handling/) - 5つの代表的な例。
* [Logging using DiagnosticSource in ASP.NET Core](https://andrewlock.net/logging-using-diagnosticsource-in-asp-net-core/) - DiagnosticSourceの使い方。ILogは特定の具体的なログを記録するのに使い、DiagnosticSourceはインフラストラクチャのイベントを記録するのに使う、という使い分けがよい？

### フィルタ

* [Handling validation responses for ASP.NET Core Web API](http://www.jerriepelser.com/blog/validation-response-aspnet-core-webapi/) - アクションフィルタで返すバリデーションエラーのメッセージをカスタマイズする方法。
* [実際の ASP.NET Core MVC フィルター](https://msdn.microsoft.com/ja-jp/magazine/mt767699.aspx) - フィルターの実装の仕方・使い方。
* [ASP.NET Core MVC で大きく変わったフィルタについて調べた](http://blog.shibayan.jp/entry/20160727/1469596437) - フィルターの実装の仕方と種類別の使い分けのガイドライン。

### フロントエンド

* [Minify CSS and JavaScript files with Visual Studio and ASP.NET Core](https://www.softfluent.com/blog/dev/2017/01/20/Minify-CSS-and-JavaScript-files-with-Visual-Studio-and-ASP-NET-Core) - 標準的な手順でMinifyするとenvironmentタグヘルパーの記述が冗長だね、という問題に対応するソリューション。
* [Simplify Client-side Validation…by Adding a Server](http://timgthomas.com/2013/09/simplify-client-side-validation-by-adding-a-server/) - クライアントサイドでのバリデーションでもサーバサイドのバリデーション機能を利用するテクニック。
* [Getting started on ASP.NET Core & React ? episode 03](http://poznajprogramowanie.pl/getting-started-on-asp-net-core-react-episode-03/) - ASP.Net Coreでwebpackを利用する具体的なチュートリアル。
* [Integrate JavaScript Logging with ASP.NET Core Logging APIs](http://hishambinateya.com/integrate-javascript-logging-with-asp.net-core-logging-apis) - フロントエンドのエラーをバックエンドで記録する！
* [featurist/coypu](https://github.com/featurist/coypu) - ブラウザ自動実行テスト用ライブラリ。

### セキュリティ

* [Cookie authentication in ASP.NET Core 2 without ASP.NET Identity](https://www.meziantou.net/2017/06/22/cookie-authentication-in-asp-net-core-2-without-asp-net-identity) - ASP.Net Identityを使わず、ものすごくシンプルに認証機能を実装する方法。
* [AttributeAuthorization with Custom Roles in ASP.NET Core](https://www.codeproject.com/Articles/1171299/AttributeAuthorization-with-Custom-Roles-in-ASP-NE) - 独自の”パーミッション”的な認証・承認要件を実装するテクニックと実例。
* [Adding WebApi & OAuth Authentication to an Existing Project](https://blogs.msdn.microsoft.com/mvpawardprogram/2017/05/02/adding-webapi-oauth-auth/)
* [Automatically validating anti-forgery tokens in ASP.NET Core with the AutoValidateAntiforgeryTokenAttribute](https://andrewlock.net/automatically-validating-anti-forgery-tokens-in-asp-net-core-with-the-autovalidateantiforgerytokenattribute/) - いちいち[ValidateAntiForgeryToken]を付けて回るのが面倒なときのテクニック。
* [How to Support Windows Authentication for ASP.NET Core in IIS](https://blogs.msdn.microsoft.com/wushuai/2017/06/26/how-to-support-windows-authentication-for-asp-net-core-in-iis/) - ASP.Net CoreアプリケーションをIISで動かすときにWindows認証を使う方法。

#### JWT

* [ASP.NET Core MVC で JWT を使った認証を実装する](http://tnakamura.hatenablog.com/entry/2017/08/04/jwt-bearer-authentication) - JWT利用方法のサンプルコード（日本語）。 - [ASP.NET Core 2.0 で JWT を使った認証を実装する](http://tnakamura.hatenablog.com/entry/2017/08/31/use-jwt-bearer-authentication-on-aspnetcore2) -* ↑のASP.Net Core 2.0バージョン。
* [Bearer Token Authentication in ASP.NET Core](https://blogs.msdn.microsoft.com/webdev/2016/10/27/bearer-token-authentication-in-asp-net-core/)
* [A look behind the JWT bearer authentication middleware in ASP.NET Core](http://andrewlock.net/a-look-behind-the-jwt-bearer-authentication-middleware-in-asp-net-core/) - JWTおよびJwtBearerAuthenticationMiddlewareの詳細な解説と使い方。
* [ASP.NET Core Token Authentication Guide](https://stormpath.com/blog/token-authentication-asp-net-core)
* [Access the JWT bearer token when using the JWT middleware in ASP.NET Core](http://www.jerriepelser.com/blog/aspnetcore-jwt-saving-bearer-token-as-claim/) - JWT bearerトークンに直接アクセスすることが必要になった場合の実装方法。
* [Secure and explore ASP.NET Core Web APIs](http://conductofcode.io/post/secure-and-explore-aspnet-core-web-apis/) - JWTを使ってWeb APIを保護する方法とSwagger・Postmanを利用したテストのテクニック。
* [JWT Validation and Authorization in ASP.NET Core](https://blogs.msdn.microsoft.com/webdev/2017/04/27/jwt-validation-and-authorization-in-asp-net-core-2/) -  Microsoft.AspNetCore.Authentication.JwtBearerのHowto。

## CQRS/MediatR

* [ASP.NET Core Lazy Command Pattern](http://rehansaeed.com/asp-net-core-lazy-command-pattern/) - CQRSパターンが大げさな場合はシンプルなコマンドパターンも候補になるよ。
* [CQRS with Mediatr and ASP.NET Core ](https://www.stevejgordon.co.uk/cqrs-using-mediatr-asp-net-core) - ASP.NetでCQRSをMediatRを使って実装する例。
* [How do I register and use a MediatR pipeline handler, for ASP.NET Core?](https://stackoverflow.com/questions/42259601/how-do-i-register-and-use-a-mediatr-pipeline-handler-for-asp-net-core) - MediatRのPipelineの例。
* [Simplifying Development and Separating Concerns with MediatR](https://blogs.msdn.microsoft.com/cdndevs/2016/01/26/simplifying-development-and-separating-concerns-with-mediatr/)
* [Simplify your controllers with the Command Pattern and MediatR](https://jonhilton.net/2016/06/06/simplify-your-controllers-with-the-command-pattern-and-mediatr/) - コントローラに渡すモデル自体がCommandオブジェクトのパターン。その他外部サービスにイベントを通知するパターンなど（パート2の記事に言及あり）。
* [Dealing with Duplication in MediatR Handlers](https://lostechies.com/jimmybogard/2016/12/12/dealing-with-duplication-in-mediatr-handlers/)
* [Basic CQRS with Dapper.NET](https://www.upnxt.com/blog/basic-cqrs-with-dapper) - Dapperを用いて”ゆるく”CQRSを実装する方法。リポジトリパターンの代替として。
* [seesharper/Blog.Transaction](https://github.com/seesharper/Blog.Transactions) - CQRSとトランザクションとDapperの例。

## データベース

* [Prefix vs Glimpse: SQL Queries](https://stackify.com/prefix-vs-glimpse-sql-queries/) - SQLの監視・分析ツール『Prefix』。
* [5 Ways To Manage Database Schema Changes in 2017 (in .NET) ](https://surfingthecode.com/2017/05/5-ways-to-manage-database-schema-changes-in-dotnet/) - イマドキのマイグレーション。

### Dapper

* [Dapper Tutorial](http://dapper-tutorial.net/dapper) - Dapperのチュートリアル。API一覧が便利。

### EntityFramework

* [Paging with Entity Framework Core](http://gunnarpeipman.com/2017/01/ef-core-paging/) - ページングの実装例。

## テスト

* [Mocking in .NET Core Tests with Moq](http://dontcodetired.com/blog/post/Mocking-in-NET-Core-Tests-with-Moq) - Moqの使用例。

## WPF

* [WPF4.5入門](http://blog.okazuki.jp/entry/2014/12/27/200015)
* [WPF とは何か](http://www.kanazawa-net.ne.jp/~pmansato/wpf/wpf_main.htm) - 内容はやや古いが、WPFの基本的なことを丁寧に解説している。
* [Window vs Page vs UserControl for WPF navigation?](http://stackoverflow.com/questions/12206120/window-vs-page-vs-usercontrol-for-wpf-navigation)
* [A Simple Pattern for Creating Re-useable UserControls in WPF / Silverlight](http://blog.scottlogic.com/2012/02/06/a-simple-pattern-for-creating-re-useable-usercontrols-in-wpf-silverlight.html) - UserControlとBindingのコツ
* [Template10](https://github.com/Windows-XAML/Template10)
* [http://blog.okazuki.jp/entry/2015/02/18/225903](http://blog.okazuki.jp/entry/2015/02/18/225903) - ReactiveProperty & Livet・Prism・?MVVM Light toolkitの比較用サンプルプロジェクト。
* [PrismとReactivePropertyで簡単MVVM！](http://qiita.com/hiki_neet_p/items/e381c687b0644c0e4978) - WPFとPrismとReactivePropertyの基本がわかるチュートリアル。
* [SourceChord](http://sourcechord.hatenablog.com/archive/category/WPF) - WPFのTipsたくさん。
* [ItemsControl 攻略 ～ 外観のカスタマイズ](http://grabacr.net/archives/1240) - ItemControlをカスタマイズする。
* [Different Ways to Bind WPF View And View Model](http://www.dotnetforall.com/different-ways-bind-view-view-model/) - VからVMを作る方法、VMからVを作る方法のおさらい。

## 帳票

* [EPPlusの使い方](http://chawatoyo.blog.fc2.com/blog-entry-15.html) - かなり多数のTips。

# JavaScript

* http://searchlibs.com - javascriptライブラリの検索。
* [もうjQueryには頼らない！素のJavaScriptでDOMを操作するための基礎知識](https://www.webprofessional.jp/dom-manipulation-vanilla-javascript-no-jquery/) - 要素のクラスの変更などが参考になる。
* [すべてをjsにまとめる思想を理解する - webpackハンズオンシリーズ](https://note.mu/konpyu/n/n694491cd9e80) - webpackが何をやっているのか、仕組みの説明。
* [How to open a pdf downloaded from an API with JavaScript](https://blog.jayway.com/2017/07/13/open-pdf-downloaded-api-javascript/) - APIのレスポンスとして返ってきたPDFを表示する方法。

## Vue

* [やわらかVue.js](https://scrapbox.io/vue-yawaraka) - 迷いがちな点のtipsやawesome-vueから漏れるニッチな情報。
* [awesome-vue](https://github.com/vuejs/awesome-vue#libraries--plugins) - Awesome!
* [第6回　Vue.jsの高度なアプリケーション開発](http://gihyo.jp/dev/serial/01/vuejs/0006) - Vue.jsによる実践的な開発のチュートリアル。
* [Vue.js入門](https://www.webprofessional.jp/up-and-running-vue-js-2-0/) - Vue Devtoolの紹介も。
* [chart.js](http://www.chartjs.org/) - サクッと使えるグラフ描画ライブラリ。
* [Vue2.x系のハマりどころ templateとコンパイラを完全解説するよ](https://aloerina01.github.io/javascript/vue/2017/03/08/1.html) - Vue.jsの利用方法別の挙動の違いについて。
* [Vue.jsを使う際のベストプラクティスについて考える](http://qiita.com/edwardkenfox/items/6f4aa591485d2a270841) - ベストプラクティスの紹介。
* [Vue.js 2.2 API Complete Cheatsheat](https://vuejs-tips.github.io/cheatsheet/) - チートシート。モーダルウィンドウのサイズが小さい…
* [CodingExplained](https://codingexplained.com/coding/front-end/vue-js) - 全般的なヒント集

### Vue用ライブラリ

* [Vue.jsのコンポーネント詰め合わせ「Element」がスゴかった](https://s8a.jp/vue-js-library-element) - 特定のコンポーネントだけを使うTipsも。

## Bootstrap

* [Multi-Step Input Forms in ASP.NET MVC](https://www.simple-talk.com/dotnet/asp-net/multi-step-input-forms-asp-net-mvc/) - マルチステップ（ウィザード形式）のフォームを実現する方法。

# CSS・デザイン

* [CSS書きたくなさすぎ問題2017](http://otiai10.hatenablog.com/entry/2017/05/30/161951) - CSSフレームワーク一覧とひと言感想。
* [Loading Styles](https://survivejs.com/webpack/styling/loading/) - webpackでCSSを管理するテクニック。
* [NxWorld](http://www.nxworld.net/) - すぐに使えるデザインテクニック。
* [かつてはJavaScriptを利用していたものの、今ではCSSのみで実装できる10の小技](https://www.webcreatorbox.com/tech/js-to-css/) - CSSだけでできるテクニック。
* [Webデザインを「もっとかっこよくして！」と言われた時に試したいCSS小技5つ](https://www.webcreatorbox.com/tech/snippets-cool-webdesign) - 確かにかっこよくなる。
* [素人でもプロ並みの配色ができるデザインパターン参考サイト21選](https://blog.codecamp.jp/color_pattern) - 色の選び方・サンプル。
* [COLOURlovers](http://www.colourlovers.com/) - 配色やパターンがたくさん。
* [Design Better Data Tables](https://uxdesign.cc/design-better-data-tables-4ecc99d23356) - テーブルを見やすく・使いやすくするテクニック。
* [CSSアニメーションを簡単に実装できるライブラリ 10＋](https://www.nxworld.net/services-resource/css-animation-libraries.html)
* [Orion Icon Library](https://orioniconlibrary.com/app)
* [モバイルサイトのサブナビゲーション](https://u-site.jp/alertbox/mobile-subnavigation)
* [7 Practical Tips for Cheating at Design](https://medium.com/refactoring-ui/7-practical-tips-for-cheating-at-design-40c736799886) - デザインを劇的に改善するTips。

# Webセキュリティ

* [商用環境で設定しておきたいセキュリティ関連 HTTP ヘッダまとめ](http://etc9.hatenablog.com/entry/2018/01/18/215626) - X-Content-Type-Optionsなど、設定が推奨されるHTTPヘッダの紹介。

# 開発環境

* [Windows での最速 Node.js 環境構築](http://tyru.hatenablog.com/entry/2017/03/13/162318) - 最速。

# DDD

* [境界づけられたコンテキスト 概念編 - ドメイン駆動設計用語解説](http://little-hands.hatenablog.com/entry/2017/11/28/bouded-context-concept) - 境界づけられたコンテキストによる分割の考え方。
