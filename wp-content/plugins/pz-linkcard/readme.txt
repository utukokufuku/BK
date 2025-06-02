=== Pz-LinkCard ===
Contributors: Poporon
Tags: LinkCard, BlogCard, Internal Link, External Link
Requires at least: 5.7
Tested up to: 6.3.1
Requires PHP: 7.0
Stable tag: trunk
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html
Donate link: https://www.amazon.co.jp/gp/registry/wishlist/2KIBQLC1VLA9X

This plugin is intended to display a link in a blog card format. The goodbye to the text-only link.


== Description ==

This plugin is intended to display a link in a blog card format.

Easy to use. Just to write a short code.

You can change the appearance in the settings screen.

You can edit or delete the cache on the manage screen.

The goodbye to the text-only link.

* It will access to WebAPI for the thumbnail image acquisition and site icon of acquisition. In addition , it will save the title and excerpt statement to the database. For more information you want to read the item of arbitrary section about this.


このプラグインはショートコードでURLを指定する事で、リンクをブログカード形式で表示させるものです。

外部リンクと内部リンクで、カードの色や新しくウィンドウを開くか等、設定を変更する事ができます。

リンク先の情報はキャッシュされるため、ソーシャルカウント等も表示されるカード形式のリンクとしては高速に表示されます。

カード管理画面から、キャッシュされた情報の再取得や編集、削除等が行えます。

テキストにリンク設定しただけでは物足りないと感じていたら、ぜひお試しください。

※このプラグインはサムネイル取得やサイトアイコン取得のためにリンク先URLをWebAPIに送信します。
※タイトルや抜粋文等をDBへ保存します。詳細は「Arbitrary section」をお読みください。


== Installation ==

Install from WordPress admin panel

1. From the WordPress admin panel, click "Plugins" -> "Add new".
2. In the browser input box, type "Pz-LinkCard".
3. Select the "Pz-LinkCard" plugin and click "Install".
4. Activate the plugin.


Install from .zip file

1. Download the plugin from this page.
2. Save the .zip file to a location on your computer.
3. Open the WordPress admin panel, and click "Plugins" -> "Add new".
4. Click "upload" then browse to the .zip file downloaded from this page.
5. Click "Install" and then "Activate plugin".


WordPressダッシュボードからのインストール

1. WordPress管理画面から「プラグイン」→「新規追加」とクリックしていきます。
2. 検索ボックスに「Pz-LinkCard」を入力して検索します。
3. プラグイン名「Pz-LinkCard」と作者「poporon」を確認して「今すぐインストール」をクリックします。
4. 「有効化する」をクリックして有効化します。


WordPress.org からのダウンロードおよびインストール

1. WordPress.orgのプラグイン一覧から「Pz-LinkCard」を検索します。
2. プラグイン名「Pz-LinkCard」と作者「poporon」を確認してダウンロードします。
3. WordPress管理画面から「プラグイン」→「新規追加」とクリックしていきます。
4. 「プラグインのアップロード」をクリックしてダウンロードしてあるZIPファイルを選択します。
5. プラグイン一覧から「有効化」をクリックして有効化します。


新しいバージョンを有効化したら動作しなくなった場合

1. FTPソフトやサーバーのコントロールパネルからWordPressのインストールされているディレクトリを確認します。
2. 「/wp-content/plugins/pz-linkcard」のディレクトリ名を変更します。（例．pz-linkcard-disable ）
2. WordPressダッシュボードに入ると、プラグインが無効化されたというメッセージが表示されます。
3. 先ほど変更したディレクトリ名を元に戻します（戻してもプラグインは勝手に有効化されません）
4. プラグインのページから古い安定版をダウンロードします
5. 上書きコピーを行ったあと、有効化を選んで、有効化します
6. 不具合が起きた状態や状況、テストサイトであれば、アクセスするためのURLを教えていただけると早急に修正できる場合があります


== Frequently asked questions ==

= データベースの容量を圧迫しませんか？ =

リンク先URL、タイトル、抜粋文等を取得してデータベースに格納します。
URLごとに保存されるため、別の記事でも同一URLを指定した場合にデータは増えません。
結果として記事内にタイトルや抜粋文を記述してリンクを設定するのと大きな差は無いと思います。
記事からショートコードを消してもデータベースからキャッシュ情報は削除されません。
キャッシュ情報を削除する場合、カード管理画面から個別で削除してください。
また、アンインストール時にプラグインと設定内容、キャッシュ用のデータベースを削除します。
外部リンクのサムネイルに「直接取得」を指定すると、リンク先サイトの画像を取得してサイズを拡大・縮小したファイルを作成します。
画像サイズを大きくするとファイル容量が増えるのでご注意ください。

= 内部リンクでの場合も新しいウィンドウで開きたいのですが？ =

設定画面から「外部リンク」と「内部リンク」、それぞれ「新しいタブで開く」の設定項目があります。
「モバイルのみ」と設定すると、パソコン等では別タブで開き、スマートフォンでは同一タブに開く事もできます。
新しいウィンドウで開くか、新しいタブで開くかは、ブラウザ側の制御となるため、ほとんどの場合新しいタブで開く事となります。

= WordPressのピンバックがリンク先へ飛びません。 =

WordPressピンバックは記事中にリンクを直接記述しないと飛びません。
ショートコード内にURLを記述した場合、ピンバックは飛びません。
直接URLを記述し、設定画面の「エディタ」タブから「URL行の変換」を有効にする事で対応できます。

= SSLサイトの内容が取得できません。 =

WordPressが動作しているサーバー側のSSL証明書が更新されていない場合等の場合、SSL検証が失敗されるのが原因と思われます。
「SSL検証を行わない」を有効にする事で改善される場合があります。（非推奨）

= nofollowの設定は重要ですか？ =

外部リンクにのみnofollowが設定できます。
Googleではnofollowを指定したリンク先はリンク元のサイトの評価に使用しないとしています。
通常は使用しない事をお勧めしますが、サイトの運用ポリシーによって使用する事は差し支えありません。

= noopenerの設定は重要ですか？ =

外部リンクにnoopenerを設定する事で、悪意を持ったサイトからリンク元のタブを保護する事ができるため設定する事を推奨します。
最近のウェブブラウザでは指定が無くてもnoopenerの動作をする物が増えています。

= 直接取得したサムネイルが粗い。 =

外部リンクのサムネイルの直接取得は著作権法上の引用の範囲を超える事のないように低解像度（100px四方）としていました。
Ver.2.1.2から200px四方に変更、Ver.2.4.1から自由に指定できるように変更しました。
イラストや写真が載っているサイトの画像を高画質で取得し、ギャラリーのような形で表示した場合等は違法と判断される恐れがあります。

= 「続きを読む」ボタンが表示されない。 =

カードの「高さ」を空欄にして記事内容が全て表示されるように指定しないと表示されない事があります。


== Screenshots ==

1. "Options screen"
2. "Cache manager screen"
3. "Edit cache data"
4. "The appearance of the 'LinkCard'"
5. "Write shortcode and url"


== Changelog ==

= 2.4.8 =
* WordPress 6.3.1 での動作確認。
  Compatible with WordPress 6.3.1.
* カード管理画面にてSQLの構文エラーがあったのを修正。（Thanks @in_seki on Twitter）
  Fixed: Fixed SQL syntax error in card management screen.
* 設定画面の「外部リンク」タブに「サムネイル」と「サイトアイコン」の「代替テキスト」の設定を追加。（Thanks @ on Twitter）
  Added: Added "ALT Text" settings for "Thumbnail" and "Site Icon" to the "External Links" tab of the Settings page.
* 設定画面の「内部リンク」タブに「サムネイル」と「サイトアイコン」の「代替テキスト」の設定を追加。（Thanks @ on Twitter）
  Added: Added "ALT Text" settings for "Thumbnail" and "Site Icon" to the "Internal Links" tab of the Settings page.
* 設定画面の「Twitter」のシェア数の単位を「Posts」と「Tweets」から選べる設定を追加。
  Added: Added a setting that allows users to choose between "Posts" and "Tweets" as the unit for the number of shares for "Twitter" on the settings screen.
* X (Twitter)のシェア数が取得できないため、WebAPIの利用を停止。
  Modified: Stopped using WebAPI because the number of X (Twitter) shares cannot be obtained.

= 2.4.7 =
* WordPress 6.0.2 での動作確認。
  Compatible with WordPress 6.0.2.
* ビジュアル エディタの「リンクカード挿入」ボタンが表示されない不具合を修正。（Thanks @hutagoparadise on Twitter）
  Fixed: Fixed a bug that prevented the "Insert Link Card" button in the Visual Editor from appearing.

= 2.4.6.1 =
* WordPress 6.0.1 での動作確認。
  Compatible with WordPress 6.0.1.
* 国際化ドメイン（日本語ドメイン）の記事が取得できない不具合を修正。（Thanks @kozy_1919 on Twitter）
  Fixed: Fixed a bug that prevented the acquisition of articles with an IDNA-ASCII-Domain.

= 2.4.6 =
* WordPress 6.0 での動作確認。
  Compatible with WordPress 6.0.
* 画像のリダイレクトに対応。（CDN対応）（Thanks @in_seki on Twitter）
  Modified: Support for image URL redirects in CDNs, etc.
* 特定のテーマでAMPと誤判定してしまう不具合を修正。（Thanks @360bpk on Twitter）
  Fixed: Fixed a bug that caused misidentification as AMP when combined with certain themes.

= 2.4.5.4 =
* WordPress 5.9.5 での動作確認。
  Compatible with WordPress 5.9.5.
* プラグインのアンインストールが失敗する不具合を修正。
  Fixed: Fixed a bug that caused uninstallation to fail.
* 管理画面に記事情報が登録されない不具合を修正。（Thanks @OrganicRelife on Twitter）
  Fixed: Fixed a bug that article information could not be cached.
* 管理画面で入力したページ数に移動しなかったのを修正。
  Fixed: Fixed a bug that prevented moving by specifying the number of pages.

= 2.4.5.3 =
* 相対指定のURLを使用した場合に致命的エラーが出る不具合を修正。（Thanks @wiashia on Twitter）
  Fixed: Fixed a bug that caused a fatal error when using a relative URL.

= 2.4.5.2 =
* カード管理画面のエスケープ処理を追加。（XSS脆弱性の対応）（Thanks tkusagaya on WordPress.org）
  Fixed: Added escaping of display items to address XSS vulnerability.

= 2.4.5.1 =
* 内部リンクの投稿日・更新日が表示されるように修正。（Thanks A-Jin）
  Fixed: Fixed internal links not displaying posted and updated dates.

= 2.4.5 =
* 最低動作環境を WordPress 5.7 に変更。
  Changed the minimum system requirements to WordPress 5.7.
* WordPress 5.8.2 での動作確認。
  Compatible with WordPress 5.8.2.
* PHP 7.3 での動作確認。
  Compatible with PHP 7.3.
* PHP 7.4 での動作確認。
  Compatible with PHP 7.4.
* PHP 8.0 に対応。PHPの仕様変更により出るようになったエラーを修正。
  Compatible with PHP 8.0.
* PHP 8.1 での動作確認。（WordPress本体や他のプラグインでエラーが出る状態です）
  Compatible with PHP 8.1.
* リンクカードのタイトルと抜粋文のエスケープ処理を追加。（XSS脆弱性の対応）
  Fixed: Added escaping of display items to address XSS vulnerability.
* リンクカードのHTMLの"noopener"の表記ミスを修正。（Thanks @jh4vaj on Twitter）
  Fixed: Corrected a spelling error in "noopener".
* カード情報のエクスポート時、改行が入らないように修正。
  Fixed: Fixed that line feeds are not inserted when exporting card information.

= 2.4.4.4 =
* WordPress 5.7.1 での動作確認。
  Compatible with WordPress 5.7.1.
* WordPress 5.7.2 での動作確認。
  Compatible with WordPress 5.7.2.
* WordPress 5.8 での動作確認。
  Compatible with WordPress 5.8.
* WordPress 5.8.1 での動作確認。
  Compatible with WordPress 5.8.1.
* カード管理画面の一覧画面に表示される文字列にエスケープ処理を追加。（XSS脆弱性の対応）
  Fixed: Added escaping of display items to address XSS vulnerability.
* カード管理画面の編集画面に表示される文字列にエスケープ処理を追加。（XSS脆弱性の対応）
  Fixed: Added escaping of display items to address XSS vulnerability.
* リンクカードを表示する際の文字列にエスケープ処理を追加。（XSS脆弱性の対応）
  Fixed: Added escaping of display items to address XSS vulnerability.

= 2.4.4.3 =
* 設定画面の「エディタ」タブの「テキストリンク行を変換」を有効にした場合、行の始めから終わりまでAタグで囲われている場合、画像等があっても変換してしまう不具合を修正。（Thanks @magemagemaaage）
  Fixed: Fixed a bug that "Convert text link line" on the "Editor" tab of the setting screen converts even if there is something other than text.
* 設定画面とカード管理画面のアイコンをemojiスタイルに変更。（U+FE0F VARIATION SELECTOR-16 (EPVS) を付与。）
  Modified: Change the icons on the setting screen and card management screen to emoji style.

= 2.4.4.2 =
* URLに%20（半角スペース）が含まれていた場合、除去しないように修正。
  Modified: Corresponds to the case where the URL contains a half-width space.
* ショートコードの閉じに全角ダブルクォートを指定してもリンクが機能するように修正。（「“」と「”」は対応していましたが「″」の対応が抜けていました）
  Modified: Corresponds to the case of using double-byte quotes for shortcodes.

= 2.4.4.1 =
* WordPress 5.7 での動作確認。
  Compatible with WordPress 5.7.
* 設定画面の「内部リンク」タブの「記事取得方法」で「抜粋文を優先」を選んでも抜粋文が取得できていない不具合を修正。（Thanks @OrganicRelife）
  Fixed: Fixed a bug that excerpts could not be obtained even if "Prioritize excerpts" was selected in "Article acquisition method" on the "Internal link" tab of the setting screen.

= 2.4.4 =
* URLパラメーターにクォート文字が残ってしまう不具合を修正。（Thanks @OrganicRelife）
  Fixed: Fixed a bug that quotes remained in URL parameters.
* URLパラメーターで許容するスキーム（プロトコル）を追加。（http: / https: / file: / ftp: / data: / ogg: を許容します。）
  Modified: Added protocols allowed by URL parameters.
* URLパラメーターが不正な場合、カード管理画面に登録されないように修正。
  Fixed: Corrected so that it will not be registered if the URL parameter is incorrect.
* ソーシャルカウント数が表示されていなかった不具合を修正。（Ver.2.4.2.1から発生）（Thanks @san5w）
  Fixed: Fixed a bug where the social count was not displayed.
* ソーシャルカウントの取得が出来ない不具合を修正。（Thanks @san5w）
  Fixed: Fixed a bug that social count could not be obtained.
* 旧バージョンからのオプション引継ぎの処理を一部変更。
  Modified: Changed the method of inheriting options from the previous version.
* 設定画面のレイアウトを一部見直し。
  Modified: Review the layout of the setting screen.
* 設定画面の見出しに「ギア」のアイコンを追加。
  Added: Added an icon to the heading of the settings screen.
* 設定画面の各設定の見出しの書式を変更。
  Modified: Add format to each setting heading on the settings screen.
* 設定画面のスタイルシートを直書きしていたものをCSSファイルへ移動。
  Modified: Move stylesheets from HTML to CSS.
* 設定画面の右上に「カード管理画面」へのリンクを追加。
  Added: Added a link to the management screen at the top right of the setting screen.
* 設定画面の「エラー」タブのエラー解除方法をチェックを外す方法からボタンを押す方法へ変更。
  Modified: Modified the error cancellation method on the setting screen.
* 設定画面の「外部リンク」タブの「記事取得方法」が正しく表示されない不具合を修正。
  Fixed: Fixed a bug that could not be selected in "Get Contents" on the "External link" tab of the setting screen.
* 設定画面の「内部リンク」タブの「記事取得方法」を選んでも反映されない不具合を修正。（Thanks @OrganicRelife）
  Fixed: Fixed a bug that could not be selected in "Get Contents" on the "Internal link" tab of the setting screen.
* 設定画面の「リンク先の検査」タブの「ユーザーエージェント」を書き換え可能項目に変更。
  Modified: Modified "User Agent" on the "Link Check" tab of the setting screen to be changeable.
* 設定画面の「エディタ」タブの「テキストリンク行を変換」を有効にした場合、URLが認識されず変換されないパターンがあったため修正。（マルチバイト文字が入っている場合、?や&といったパラメーターがある場合等）
  Fixed: Fixed a bug that URL is not converted in "Convert text link line" on the "Editor" tab of the setting screen.
* 設定画面の「エディタ」タブの「URL行を変換」を有効にした場合、URLが認識されず変換されないパターンがあったため修正。（マルチバイト文字が入っている場合、?や&といったパラメーターがある場合等）
  Fixed: Fixed a bug that URL is not converted in "Convert URL line" on the "Editor" tab of the setting screen.
* 設定画面の「エディタ」タブの「パラメータ（表記例）」を修正。
  Modified: Added a description example of "Parameter" on the "Editor" tab of the setting screen.
* 設定画面に「管理者」タブを追加。
  Added: Added "Admin" tab to the setting screen. (Available only in admin mode)
* 設定画面に「管理者」タブに「WP-Cronの設定」を追加。
  Added: Added "WP-Cron Settings" setting to "Admin" tab of the setting screen. (Available only in admin mode)
* 設定画面の「上級者向け」タブ内に「上級者向けの設定」を追加。
  Added: Added "Senior Settings" setting to "Advanced" tab of the setting screen.
* 設定画面の「上級者向け」タブ内に「拡張機能の設定」を追加。
  Added: Added "Extension Settings" setting to "Advanced" tab of the setting screen.
* 設定画面の「上級者向け」タブ内の「上級者向けの設定」から一部項目を「上級者向けの設定」へ移動。
  Modified: Moved any setting item on the setting screen from the "Advanced Settings" to the "Senior Settings".
* 設定画面の「上級者向け」タブ内の「上級者向けの設定」から一部項目を「拡張機能の設定」へ移動。
  Modified: Moved any setting item on the setting screen from the "Advanced Settings" to the "Extension Settings".
* 設定画面の「マルチサイト」タブに設定が変更できない旨のメッセージを追加。
  Added: Added a message to the "Multi-site" tab of the setting screen that it cannot be changed.
* 設定画面の「マルチサイト」タブに「テーブル名称」を追加。
  Added: Added "Multi-site" tab "Table name" on the setting screen.
* 設定画面の「マルチサイト」タブに「サブサイトへのリンク」の設定を追加。
  Added: Added the setting of "Multi-site" tab "Link to sub-site" on the setting screen.
* 設定画面の「初期化タブ」「調査モード」「管理者モード」「開発者モード」を変更した際、「変更を保存」を押さなくても即時反映されるように修正。
  Modified: Changed some check items on the setting screen to reflect immediately.
* 設定画面の「設定を保存した日時」の表示項目を「上級者向け」タブから「基本」タブへ移動。
  Modified: Moved the display item of "Saved Time" on the setting screen from the "Advanced" tab to the "Basic" tab.
* カード管理画面のレイアウトを一部見直し。
  Modified: Review the layout of the manager screen.
* カード管理画面の見出しに「カードボックス」のアイコンを追加。
  Added: Added an icon to the heading of the mamager screen.
* カード管理画面の検索窓の左側に「虫眼鏡」のアイコンを追加。
  Added: Added an icon to the search-box of the mamager screen.
* カード管理画面のスタイルシートを直書きしていたものをCSSファイルへ移動。
  Modified: Move stylesheets from HTML to CSS.
* カード管理画面の右上に「設定画面」へのリンクを追加。
  Added: Added a link to the settings screen at the top right of the management screen.
* カード管理画面のエディタ画面のレイアウトを一部見直し。
  Modified: Review the layout of the editor screen of the card management screen.
* カード管理画面のエディタ画面に見出しを追加。
  Modified: Added heading to the editor screen of the card management screen.
* カード管理画面のエディタ画面の上側にも保存とキャンセルのボタンを追加。
  Modified: Added save and cancel buttons at the top of the editor screen of the card management screen.
* カード管理画面の一覧のサムネイル画像をクリックすると新しいタブで画像を表示するように変更。
  Modified: Click the thumbnail image in the list on the management screen to display the image in a new tab.
* カード管理画面の一覧のURLの先頭に、アクセス不能な場合「⛔（通行禁止）」のアイコンを表示するように変更。
  Modified: Added an icon at the beginning of the URL of the management screen list when inaccessible.
* カード管理画面の一覧のURLの先頭に、アクセス不能だがエラー無視の設定をしている場合「⚠（警告）」のアイコンを表示するように変更。
  Modified: Added an icon at the beginning of the URL in the list of management screens when "Inaccessible but ignored"
* カード管理画面の一覧のURLの先頭のアイコンの大きさを9pxから16pxへ変更。
  Modified: Change the size of the icon at the beginning of the URL in the management screen list.
* カード管理画面の一覧の結果コードの数字にポインタを合わせると結果メッセージがツールチップで表示されるように変更。
  Modified: Added tooltip to the result code in the list of management screens.
* カード管理画面の一覧のクイックメニューを選択中の行のみに表示されるように変更。
  Modified: Changed the display method of the quick menu of the list on the management screen.
* カード管理画面の一覧の下側にもページナビを追加。
  Modified: Page navigation has also been added to the bottom of the list on the card management screen.
* カード管理画面のエディタの結果コードの横に結果メッセージを表示するように変更。
  Modified: Add a message next to the result code in the editor on the admin screen.
* カード管理画面のエディタに結果コードがエラーでもリンク切れ状態にしない「エラーを無視」の項目を追加。（Thanks @wordmovies2018）
  Added: Added "Ignore error" setting to the editor of the management screen.
* カード管理画面の「ファイルメニュー」の見出しに「書類」のアイコンを追加。
  Modified: Added an icon to the file menu of the management screen.
* カード管理画面の「エクスポート」の出力項目を現在の記録項目に合わせて修正。
  Modified: Change the output items of the export of the management screen.
* require_once を include に変更。
  Modified: Replace require_once with include.

= 2.4.3.3 =
* 設定画面の「上級者向け」タブに「URLの補正」の設定を削除。（不具合が解消されなかったため。）（Thanks @tannpura00）
  Modified: Deleted "URL correction" setting from "Advanced" tab of the setting screen. (It wasn't the cause of the problem.)
* URL内の % が %25 とエンコードされていた際に正しいページにリンクがされなかった不具合を修正。（Thanks @tannpura00）
  Fixed: Fixed a bug that the correct page was not linked when "%" in the URL was encoded as "%25".

= 2.4.3.2 =
* 設定画面の「上級者向け」タブに「URLの補正」の設定を追加。パスに日本語を使用している場合等にリンクが大量にリンク切れになる不具合に対応。（Thanks @tannpura00）
  Added: Added "URL correction" setting to "Advanced" tab of the setting screen.

= 2.4.3.1 =
* 設定画面で「変更を保存」を実行した際、一部の設定値が正常に保存されていなかった不具合を修正。
  Fixed: Fixed a bug that some setting values ​​were not saved normally when "Save changes" was executed on the setting screen.
* 設定画面の「マルチサイト」タブの、表示が一部乱れていた不具合を修正。
  Fixed a bug that the display on the "Multi-site" tab of the setting screen was partially disturbed.
* 設定画面の「エディター」タブの、「外部リンクのみ」にチェックを付けた場合にPHPエラーが出てしまう不具合を修正。（Thanks @daigamax）
  Fixed a bug that PHP error appears when "External Link Only" is checked on the "Editor" tab of the setting screen.

= 2.4.3 =
* WordPress 5.6.2 での動作確認。
  Compatible with WordPress 5.6.2.
* ドキュメント（readme.txt）修正。
  Modified: Modify "readme.txt".
* ショートコードのURLパラメータの解釈方法を修正。（Thanks @longer_n）
  Fixed: Fixed interpretation of shortcode URL parameters.
* 外部リンクで指定された画像URLが存在しない場合、警告エラーが発生する不具合を修正。（Thanks @miya_gal_ossan）
  Fixed: Fixed a bug that the image URL specified on the external link does not exist.
* 内部リンクで存在しないカテゴリページを指定した場合、警告エラーが発生する不具合を修正。
  Fixed: Fixed a bug that a warning error occurs when a category page that does not exist is specified in the internal link.
* 内部リンクで存在しないタグページを指定した場合、警告エラーが発生する不具合を修正。
  Fixed: Fixed a bug that a warning error occurs when a tag page that does not exist is specified in the internal link.
* 内部リンクでサムネイルが無い場合、デフォルト画像が出てしまう不具合を修正。
  Fixed: Fixed a bug when there is no thumbnail in the internal link.
* 内部リンクで指定された記事が存在しない場合、警告エラーが発生する不具合を修正。
  Fixed: Fixed a bug when the article specified by the internal link does not exist.
* 相対URLが指定されている場合、分析に失敗して警告エラーが発生する不具合を修正。（Ver.2.1.9から発生）
  Fixed: Fixed a bug that an error occurs when converting relative URLs.
* リンク先のサーバーが見つからない場合にリンクを設定しないように修正。
  Fixed: Fixed not to set the link when the linked server cannot be found.
* <HEAD>や<BODY>といったHTMLタグが無いサイトでもTITLEタグやMETAタグを取得するように修正。
  Fixed: Fixed to get TITLE tag and META tag even on sites without HTML tags such as <HEAD> and <BODY>.
* 外部リンクのサムネイルのキャッシュ画像のURLからスキーム（http:やhttps:）を省略するように変更。（Thanks @miya_gal_ossan）
  Modified: Modified to omit the scheme (http: and https:) from the URL of the cache image of the thumbnail of the external link.
* 設定画面から国際化ドメイン（IDNA ASCIIドメイン）に対応する設定を削除。
  Modified: Deleted the setting corresponding to the internationalized domain (IDNA ASCII domain) from the setting screen.
* 設定に関わらず国際化ドメインに対応。
  Modified: Supports internationalized domains regardless of settings.
* 設定画面で使うカラーピッカーをWordPressの物からHTML5の物に変更。
  Modified: Modified the color picker used on the setting screen from WordPress to HTML5.
* 設定画面の「相対指定URL」の設定項目を「上級者向け」タブから「リンク先の検査」タブへ移動。
  Modified: Moved the setting item of "Relative URL" on the setting screen from the "Advanced" tab to the "Link Check" tab.
* 設定画面の「基本」タブに、「更新履歴」の表示を追加。
  Added: Added the display of "Changelog" to the "Basic" tab of the setting screen.
* 設定画面の「リンク先の検査」タブに「相対指定URL」の設定を追加。
  Added: Added "Relative URL" setting to "Link Check" tab of the setting screen.
* 設定画面の「Web API」タブ、「画像」タブ、「CSS」タブを削除。
  Modified: Removed "Web API" tab, "Image" tab, and "CSS" tab on the setting screen.
* 設定画面に「その他」タブを追加。（「Web API」「画像」「CSS」の内容を統合）
  Added: Added "etc." tab to the setting screen. (Integrates the contents of "Web API", "Image" and "CSS")
* 設定画面の「外部リンク」タブに「サムネイルサイズ」の設定を追加。
  Added: Added "Thumbnail Size" setting to "External Link" tab of the setting screen.
* 設定画面の「内部リンク」タブに「サムネイルサイズ」の設定を追加。（Thanks @in_seki on Twitter）
  Added: Added "Thumbnail Size" setting to "Internal Link" tab of the setting screen.
* 設定画面の「リンクチェック」タブの「相対指定URL」の初期選択をチェック有りに変更。
  Modified: Modified the initial selection of "Relative URL" on the "Link Check" tab of the setting screen to Checked.
* 設定画面に「マルチサイト」タブを追加。（マルチサイト設定時のみ表示されます）（Thanks @i_three_miz on Twitter）
  Added: Added "Multi Site" tab to the setting screen. (Displayed only when multi-site is set)
* 設定画面の「上級者向け」タブに「圧縮」の設定を追加。
  Added: Added settings of "Compress" to the "Advanced" tab of the setting screen.
* 設定画面の「上級者向け」タブに「ファイルメニュー」の設定を追加。
  Added: Added settings of "File Menu" to the "Advanced" tab of the setting screen.
* 設定画面の「上級者向け」タブに「初期化タブ」を表示する設定を追加。
  Added: Added a setting to display the "Initialization Tab" in the "Advanced" tab of the setting screen.
* 設定画面の「上級者向け」タブから「実行時間の表示」の設定を削除。
  Modified: Deleted "Display Execution Time" setting from "Advanced" tab of the setting screen.
* 設定画面の「上級者向け」タブに「調査モード」の設定を追加。（通常は使用しないでください）
  Added a setting to display the "Survey Mode" in the "Advanced" tab of the setting screen. (Do not use normally)
* 設定画面の「上級者向け」タブに「管理者モード」の設定を追加。（動作無能に陥る設定が可能なため、通常は使用しないでください。）
  Added a setting to display the "Administrator Mode" in the "Advanced" tab of the setting screen. (Do not use normally as it can be set to incapacitate.)
* 設定画面の「上級者向け」タブに「開発者モード」の設定を追加。（動作無能に陥る設定が可能なため、通常は使用しないでください。）
  Added a setting to display the "Developer Mode" in the "Advanced" tab of the setting screen. (Do not use normally as it can be set to incapacitate.)
* 設定画面の「上級者向け」タブの「URLによるAMP判断」を非推奨に変更。
  Modified: Modified "AMP judgment by URL" on the "Advanced" tab of the setting screen to Deprecated.
* 設定画面で「変更を保存」を押した際、開いているタブをそのままにするように変更。
  Modified: Modified to leave open tabs when pressing "Save Changes" on the settings screen.
* 設定画面の「初期化」タブを非表示に変更。（「上級者向け」タブから表示させることができます。）
  Modified: Modified "Initialize" tab of the setting screen to hide. (It can be displayed from the "Advanced" tab.)
* 設定画面の「初期化」タブに「プラグインの再起動」を追加。（管理者モードのみで使用できます）
  Added a setting to button "Restart Plugin" in the "Initialize" tab of the setting screen. (Available only in admin mode)
* 設定画面の「初期化」タブに「初期化時の例外」の設定を追加。（管理者モードのみで使用できます）
  Added a setting to "Initialization Exception" in the "Initialize" tab of the setting screen. (Available only in admin mode)
* カード管理画面の一覧に全件表示されていたものを、1ページに10個表示されるように修正。
  Fixed: Fixed all the items displayed in the list on the card management screen so that 10 items are displayed on one page.
* カード管理画面の外部リンクのURLにリンクを追加。
  Added: Added a link to the URL of the external link on the card management screen.
* カード管理画面にインポート・エクスポートの機能を追加。（設定画面で「ファイルメニュー」を有効にする必要があります。）
  Added: Added import / export function to the card management screen. (You need to enable "File Menu" on the settings screen.)
* カード管理画面のドメイン名の表示を国際化ドメインに対応。
  Modified: The domain name display on the card management screen is compatible with internationalized domains.
* URL表示に<CITE>タグを使用しないように変更。（URLがイタリック表示では無くなります。）
  Modified: Modified not to use <CITE> tag in URL. (The URL is no longer displayed in italics.)

= 2.4.2.2 =
* 追加するCSSファイルが呼び出せていなかった不具合を修正。（Thanks @miya_gal_ossan on Twitter）
  Fixed: Fixed a bug that the additional CSS function does not work properly.
* CSSのURLが正しくなくてスタイルシートが適用されない不具合を修正。（Thanks @longer_n on Twitter）
  Fixed a bug that CSS could not be read correctly.

= 2.4.2.1 =
* 外部リンクのサムネイルの取得に失敗して警告エラーが発生する不具合を修正。（Ver.2.4.1から発生）（Thanks ‎@kotobatoad）
  Fixed: Fixed a bug that an error occurs when thumbnail images on external links fail.
* カード管理画面で外部リンクのサムネイルが表示されない不具合を修正。（Ver.2.4.2から発生）
  Fixed: Fixed a bug that thumbnail images of external links are not displayed on the card management screen.

= 2.4.2 =
* 設定画面の「画像」タブにて、指定した画像サイズによっては警告エラーが発生する不具合を修正。（Thanks @miya_gal_ossan on Twitter）
  Fixed: Fixed image size error on settings screen.
* 外部リンクで指定された画像URLが応答しない場合、タイムアウトまで約60秒待ってしまう不具合を修正。（Thanks @miya_gal_ossan on Twitter）
  Fixed: Fixed a bug that the image URL specified on the external link does not respond.
* 設定画面で使用するjQueryを修正。
  Fixed: Review and fix jQuery on the settings screen.
* ビジュアル エディタ（クラシック エディタ）で使用するjQueryを修正。
  Fixed: Review and fix jQuery in classic editor.
* アンインストール時にファイルが残ったままだったのを削除するように修正。
  Fixed: Fixed to delete the directory that remained at the time of uninstallation.
* ドキュメント（readme.txt）修正。
  Modified: Modify "readme.txt".
* 設定画面の項目名を一部修正。
  Modified: Corrected the item name on the setting screen.
* 設定画面の「配置」タブの「BLOCKQUOTEの設定」を非推奨に変更。
  Modified: Modified blockquote setting on the setting screen to deprecated.
* 設定画面の「外部リンク」タブの「rel="nofollow" の設定」を非推奨に変更。
  Modified: Mofified nofollow setting on the setting screen to deprecated.
* 設定画面の「エディタ」タブにて、ショートコード1を設定しなくても設定エラーとしないように変更。
  Modified: Modified shortcode to optional on the setting screen.
* 設定画面の設定保存等のメッセージを閉じられるように変更。
  Modified: Modified to close the message on the setting screen.
* 設定画面で内容が変更されていない場合、設定の保存は行わずスタイルシートの再生成のみ行うように変更。
  Modified: Modified not to save if there is no change on the setting screen.
* 設定画面でのカラーピッカーを表示したときに、レイアウトが崩れるのを修正。
  Modified: Modified the behavior of color-picker on the setting screen.
* カード管理画面の編集画面に表示される日時のフォーマットをWordPressの一般設定に合わせるように変更。
  Modified: Modified date format on card management screen.
* 設定を更新した時、ブラウザのキャッシュに関係無くCSSファイルを読み直すように修正。
  Modified: Modified to read the CSS file again when updating the settings.
* facebookのシェア数が取得できないため、WebAPIの利用を停止。
  Modified: Suspended because the number of shares on facebook cannot be obtained.
* 設定画面の「エディタ」タブの「ショートコード実行」の初期選択をチェック有りに変更。
  Modified: Modified the initial settings.
* 当バージョンへバージョンアップした際、「ショートコード実行」をチェック有りに強制変更。
  Modified: Forcibly set "Do shortcode" to on.
* 「ショートコード実行」がオンになっている場合の動作を「URL行の変換」もしくは「リンク行の変換」がオンになっている場合のみに変更。
  Modified: Modified the condition of "Do shortcode".
* 設定画面に「CSS」タブを追加。
  Added: Added "CSS" tab to the setting screen.
  設定画面の「エラー」タブにて、URL指定エラーのある記事の行へのリンクを追加。
  Added: Added a link to an article with an error on the settings screen.
* 設定画面の「外部リンク」タブに、「rel="noopener"」の設定を追加。
  Added: Added settings of "rel="noopener" to the "External Link" tab of the setting screen.
* 設定画面に「画像」タブを追加。
  Added: Added "Image" tab to the setting screen.
* 設定画面の「画像」タブに、キャッシュ画像のディレクトリ名と使用量の表示を追加。
  Added: Added display of cache image directory name and usage to the "Image" tab of the setting screen.
* 設定画面の「画像」タブに、キャッシュ画像のディレクトリURLの表示を追加。
  Added: Added display of cache image directory URL to the "Image" tab of the setting screen.
* 設定画面の「上級者向け」タブに、「URLエラーを非表示」の設定を追加。（URLエラー時にWordPress管理画面にエラー表示をしなくなります。）
  Added: Added settings of "Hide URL Error" to the "Advanced" tab of the setting screen.(The error will not be displayed on the WordPress administration screen when a URL error occurs.)
* 設定画面の「上級者向け」タブに、設定を保存した日時の表示を追加。
  Added: Added display of "Saved Time" to the "Advanced" tab of the setting screen.

= 2.4.1 =
* WordPress 5.6 での動作確認。
  Compatible with WordPress 5.6.
* 外部リンクの画像をキャッシュするときのサイズを選択できる機能を追加。（Thanks @peacediner on Twitter）
  Added: Added settings to allow you to choose the size when caching images from external link.

= 2.4.0 =
* WordPress 5.4.2 での動作確認。
  Compatible with WordPress 5.4.2.
* WordPress 5.5 での動作確認。
  Compatible with WordPress 5.5.
* WordPress 5.5.3 での動作確認。
  Compatible with WordPress 5.5.3.
* 記事では無いページでURL指定エラーが発生する不具合を修正。（ポストIDが取得できないURLを除外）（Thanks @rindark on Twitter）（Thanks @Rina_sendai on Twitter）
  Fixed: Suppressed incorrect error display.
* サブディレクトリ型マルチサイトの判定において警告エラーが発生する不具合を修正。
  Fixed: Suppressed incorrect error display.

= 2.3.1 =
* WordPress 5.3 での動作確認。
  Compatible with WordPress 5.3.
* ビジュアル エディタの「リンクカード挿入」ボタンが表示されない不具合を修正。
  Fixed a bug that the button of the visual editor is not displayed.

= 2.3.0 =
* プラグイン等のインストール状況によって設定画面のタブが動作しない不具合を修正。
  Fixed: Fixed a bug that the tab of the setting screen does not respond.

= 2.2.9 =
* WordPress 5.2.3 での動作確認。
  Compatible with WordPress 5.2.3.
* 設定画面の「かんたん書式設定」に「コンパクト」を追加。
  Added: Tiny format 'Compact'.
* カード管理画面にヘルプアイコンを設置。
  Added: A help icon has been added to the "Pz Card Manager" screen.
* 設定画面にヘルプアイコンを設置。
  Added: A help icon has been added to the "Pz Card Settings" screen.
* 設定画面をタブ方式に変更。
  Modified: Changed the "Pz card setting" screen to tab method.
* 外部リンク、内部リンク、同ページでそれぞれ枠線の色を選択できるように機能を追加。
  Added: Added settings so that you can select the border color for external links, internal links, and the same page.

= 2.2.8 =
* WordPressテーマ「Cocoon」を使用しているとき、外部リンクのアイコンが表示されないように修正。
  Fixed: When using the WordPress theme "Cocoon", the external link icon was not displayed.
* WordPressテーマ「JIN」を使用しているとき、余分な空行が表示されないように修正。
  Fixed: When using the WordPress theme "JIN", it has been corrected so that extra blank lines are not displayed.
* 「付加情報」をSPAN要素からDIV要素に変更。（Thanks @metro_eight on Twitter）
  Modified: "Additional information" changed from SPAN element to DIV element.
* 「シェア数」をSPAN要素からDIV要素に変更。
  Modified: "Share information" changed from SPAN element to DIV element.
* 「続きを読む」ボタンをSPAN要素からDIV要素に変更。
  Modified: "Read more button" changed from SPAN element to DIV element.

= 2.2.7 =
* サイトアイコンの垂直位置（vertical-align）をテキスト下（text-bottom）から中央（middle）へ変更。
  Modified: Changed the vertical position of the site icon (vertical-align) from the bottom of the text (text-bottom) to the middle (middle).
* サイト追加情報をSPANタグからDIVタグへ変更。
  Modified: Changed site addition information from SPAN to DIV.
* 設定画面にタイトルを折り返さない設定を追加。
  Added: Added a setting that does not wrap the title.
* 設定画面にURLを折り返さない設定を追加。
  Added: Added a setting that does not wrap the URL.
* 設定画面の「文字の設定」のレイアウトを変更。
  Modified: Changed the layout of "Text Settings" on the setting screen.
* 設定画面の「かんたん書式設定」に「囲み」を追加。
  Modified: Added tiny format "Enclose".
* 設定画面の「かんたん書式設定」に「反射」を追加。
  Modified: Added tiny format "Reflection".
* 設定画面の「かんたん書式設定」に「セロハンテープ（斜め）」を追加。
  Modified: Added tiny format "Cellophane tape (digonal)".
* 設定画面の「かんたん書式設定」に「Windows 95」を追加。
  Modified: Added tiny format "Windows 95".
* 設定画面の「かんたん書式設定」に「Windows XP」を追加。
  Modified: Added tiny format "Windows XP".
* 内部リンクがキャッシュされない不具合を修正。（Thanks @Masa_s_Record on Twitter）
  Fixed: Fixed a bug that internal links are not cached.
* サイトアイコンの取得が失敗した際に、警告エラーが発生する不具合を修正。
  Fixed: Fixed a bug.

= 2.2.6.2 =
* バグ修正。
  Fixed: Fixed a bug.

= 2.2.6.1 =
* バグ修正。
  Fixed: Fixed a bug.

= 2.2.6 =
* 設定画面の「余白」に「40px」を追加。
  Added: Added "40px" to "Margin" value.
* ドメイン名（サイト名称）にマウスカーソルを重ねたときにアンダーラインが表示されないように変更。
  Modified: Changed so that the underline is not displayed when the mouse cursor is moved over the domain name (site name).
* ビジュアル エディタの「リンクカード挿入」ボタンを押したとき、モーダルウィンドウが開くように変更。
  Modified: Changed to open a modal window when the insert button is pressed.

= 2.2.5 =
* 内部リンクでもnofollow指定できるように修正。
  Modified: Fixed to be able to specify nofollow even for internal links.
* 押しピンの画像がクリック無効になるように修正。
  Modified: Fixed push pin image to be click invalid.

= 2.2.4 =
* WordPress 5.2.2 での動作確認。
  Compatible with WordPress 5.2.2.
* ショートコードごとにnofollowを追加できる機能を追加。
  Added: Added the function to add nofollow per short code.
* スタイルシートの取得方法を変更。
  Modified: Changed style sheet acquisition method.
* 内部リンクのサムネイルのURLからスキーム（http:やhttps:）を省略するように変更。
  Modified: Changed to omit scheme from URL of internal link thumbnail.

= 2.2.3 =
* 設定画面にショートコードを強制的に展開する機能を追加。
  Added: Added the function to forcibly expand the short code to the setting.
* WordPress 5.2 での動作確認。
  Compatible with WordPress 5.2.
* WordPress 5.2.1 での動作確認。
  Compatible with WordPress 5.2.1.

= 2.2.2.1 =
* ビジュアル エディタで警告エラーが発生する不具合を修正。
  Fixed: Fixed a bug.

= 2.2.2 =
* ビジュアル エディタの「リンクカード挿入」ボタンの仕組みを見直し。
  Modified: Review the mechanism of the insert button in the visual editor.

= 2.2.1 =
* WordPress 5.0.1 での動作確認。
  Compatible with WordPress 5.0.1.
* WordPress 5.0.2 での動作確認。
  Compatible with WordPress 5.0.2.
* WordPress 5.0.3 での動作確認。
  Compatible with WordPress 5.0.3.
* WordPress 5.1 での動作確認。
  Compatible with WordPress 5.1.
* URL指定エラーの解除方法をメッセージに追加。
  Modified: Added a message on how to cancel the URL error.
* 編集画面で警告が出ていたのを修正。
  Fixed: Fix warning on edit screen.

= 2.2.0 =
* WordPress 5.0 での動作確認。
  Compatible with WordPress 5.0.
* 存在しないURLを指定したときに警告エラーが発生する不具合を修正。
  Fixed: Fixed a bug.
* カード管理画面で警告エラーが発生する不具合を修正。
  Fixed: Fixed a bug.

= 2.1.9.1 =
* カード管理画面で警告エラーが発生する不具合を修正。
  Fixed: Fixed a bug.

= 2.1.9 =
* 相対URLを指定したときにサイトURLを補完する機能を追加。
  Added: Added a function to supplement site URL when relative URL is specified.

= 2.1.8.4 =
* サイト情報が「なし」の場合、「続きを読む」ボタンが表示されなかったのを修正。（Thanks Andrew）
  Fixed: Fixed a bug that the "Read more" button is not displayed.

= 2.1.8.3 =
* カード管理画面で警告エラーが発生する不具合を修正。（Thanks @sayataro98 on Twitter）
  Fixed: Fixed a bug.
* 「続きを読む」ボタンが表示されなかったのを修正。（Thanks Andrew）
  Fixed: Fixed a bug that the "Read more" button is not displayed.

= 2.1.8.2 =
* 警告エラーが発生する不具合を修正。
  Fixed: Fixed a bug.

= 2.1.8.1 =
* フィルターの優先度を指定するように修正。
  Modified: Fix to specify filter priority.
* リンク切れチェックの周期が長くなるように修正。
  Modified: Correction was made so that the link break check cycle becomes longer.
* 編集画面に次回のリンク切れチェック日時を表示。
  Modified: The next link break check date and time was displayed on the edit screen.

= 2.1.8 =
* 設定画面の「かんたん書式設定」の「Pzカード 標準書式」を「Pzカード オリジナル」に名称変更。
  Modified: Minor fixes.
* 設定画面の「かんたん書式設定」の「Pzカード 標準書式」を微調整。
  Modified: Fine adjustment tiny format "Pz LinkCard Default".
* 設定画面の「かんたん書式設定」の「見出し」を微調整。
  Modified: Fine adjustment tiny format "Header".
* 設定画面の「かんたん書式設定」の「シンプル」を「ノーマル（はてなブログカード風）」に名称変更。
  Modified: Modified tiny format "Simple" to "Normal".
* 設定画面の「かんたん書式設定」に「シンプル」を追加。
  Added: Added tiny format "Simple".
* 設定画面の「かんたん書式設定」の「押しピン」を微調整。
  Modified: Added tiny format "Pushpin".
* 設定画面のサイト情報の位置に「タイトルの上側」を追加。
  Added: Added setting to set Above the title.
* 設定画面の「サイト情報」を「付加情報」に修正。
  Fixed: Modified "Site information" to "Added information".
* カード管理画面の並び順の表示が昇順になっていたのを修正。
  Fixed: Fixed a bug.
* ソーシャルカウントに「Pocket」を追加。
  Added: Added Pocket social count.
* アンカーテキストの装飾を無くすように修正。
  Added: Added setting to disable anchor text decoration.

= 2.1.7.1 =
* 設定画面の「かんたん書式設定」に「見出し」を追加。
  Added: Tiny format 'Headline'.
* スタイルシートを整理。
  Modified: Minor fixes.

= 2.1.7 =
* 「外部リンク」「内部リンク」「同ページ」の判定方法を修正。
  Modified: Change judgment method.
* 設定画面に外部リンクのみ変換する設定を追加。（テーマに内部リンクのカード化機能がある場合を想定）（Thanks @mocochat on Twitter）
  Added: Added 'Convert only external link'.
* 文字コードを自動判断したときの結果を修正。
  Modified: Minor fixes.

= 2.1.6.2 =
* アンカーテキストのアンダーラインが表示されてしまうのを修正。
  Fixed: Fixed a bug.

= 2.1.6.1 =
* サイト情報を表示しないとき、ワーニングが出ていたのを修正。
  Fixed: Fixed a bug.（Thanks @ryuji120912 on Twitter）

= 2.1.6 =
* 設定画面にTwitterアカウントを表示。
  Added: Added 'When in trouble'.
* タイトル取得方法（正規表現）を修正。
  Modified: Fixed title acquisition method.
* アンカーテキストのアンダーラインを無しに。
  Modified: Changed the text-decoration to "none".

= 2.1.5 =
* 文字装飾を「無し」(none)に変更。
  Modified: Changed the text-decoration to "none".
* 設定画面の「影」の初期設定を「影を付けない」に変更。
  Modified: Changed the initial setting to "Do not add shadows".
* 設定画面の「角をまるめる」の初期設定を「角を丸めない」に変更。
  Modified: Changed the initial setting to "Do not round".
* 設定画面の外部リンクのサムネイルの初期設定を「直接取得できない場合、WebAPIを利用する」に変更。
  Modified: Changed the initial setting to "Use WebAPI ,If can not direct".
* 設定画面の「角をまるめる」にサイズを追加。
  Modified： Square rounding has added some sizes.
* 設定画面の「カードの余白」に「24px」を追加。
  Modified: 24px was added to the card margin.
* 設定画面のサムネイル取得WebAPIのHeartRail社の例をhttpsに変更。
  Modified: Modified HeartRail WebAPI URL to support SSL.
* facebookのシェア数取得WebAPIをhttpsに変更。
  Modified: Modified facebook WebAPI URL to support SSL.
* Twitterのツイート数取得WebAPIをhttpsに変更。
  Modified: Modified Twitter WebAPI URL to support SSL.
* Tweet(s)をクリックしたときの動作をツイート検索に変更。
  Modified: From registration to search at Twitter.
* User(s)をクリックしたときの動作をはてなブックマーク数表示に変更。
  Modified: From registration to search at Hatena.
* 設定画面の「サイト情報」から「サイト名称」と「付加情報」を別項目に変更。
  Added: Add additional information.
* 設定画面の「文字の設定」に「付加情報」の文字設定を追加。
  Added: Add character setting of additional information.
* 設定画面の「付加情報」を「見出し表示」にする設定を追加。（Thanks @hituji_1234 on Twitter）
  Added: Added setting to set additional information as heading.

= 2.1.4.2 =
* WordPress 4.9.8 での動作確認。
  Compatible with WordPress 4.9.8.

= 2.1.4.1 =
* URLの記述ミスを修正。
  Modified: Corresponded to URL mistake.

= 2.1.4 =
* CHARSETを判断できないパターンがあったのを修正。（Thanks サイノア）
  Fixed: There was a pattern which can not judge CHARSET, so I fixed it.
* カード管理画面で「すべて」を選んだときに「内部リンク」のみが表示されていたのを修正。
  Fixed: Fixed a bug in card management.

= 2.1.3.1 =
* WordPress 4.9.6 での動作確認。
  Compatible with WordPress 4.9.6.

= 2.1.3 =
* WordPress管理画面のカード管理画面のサブメニュー項目の横にリンク切れの件数を表示する機能を追加。（Thanks @Oncle1316 on Twitter）
  Added: Added setting to display the number of broken links next to the submenu.

= 2.1.2.2 =
* 定義されていない変数を使用していたため警告エラーが発生する不具合を修正。
  Fixed: Fixed a bug.

= 2.1.2.1 =
* プラグインの新規インストールもしくは停止から有効化した際に警告エラーが発生する不具合を修正。
  Fixed: Fixed a bug.

= 2.1.2 =
* 直接取得するサムネイルのサイズを100pxから200pxへ変更。
  Fixed: Directly acquired thumbnail size was changed from 100px to 200px.
* 横幅に合わせて縮小表示させるときのフォントサイズと行の高さを調整。
  Fixed: Adjusted the font size and line height when reducing the display to fit the width.
* URLを表示できる場所を「タイトルの下」の他に「サイト情報の後ろ」が選べるように変更。
  Added: "Behind site-info" has been added as the display location of the URL.
* カード管理画面に文字列検索を追加。
  Added: A character string search was added to the card management screen.
* カード管理画面の一括メニューに「サムネイルの再取得」を追加。
  Added: "Renew thumbnail" was added to the batch menu of the card management screen.

= 2.1.1.1 =
* WordPress 4.9.5 での動作確認。
  Compatible with WordPress 4.9.5

= 2.1.1 =
* 設定画面に「続きを読む」ボタンの文字の色とサイズを追加。
  Added: Added setting of color and size of "Read more".

= 2.1.0.1 =
* カード管理画面に「リンク切れ」の項目を追加。
  Added: Added "Link broken" item to card management.
* スタイルシートを読み込まないときに簡易表示するように修正。（Google AMP対応）
  Modified: If CSS is not loaded, display simple.
* 設定画面に、テキストエディタのクイックタグを表示するかを選択する設定を追加。
  Added: Added settings to allow you to choose whether to display quick tags in a text editor.
* 設定画面に、ビジュアル エディタの「リンクカード挿入」ボタンを表示するかを選択する設定を追加。
  Added: Added settings to allow you to choose whether to display the insert button in the visual editor.
* 設定画面に、「続きを読むボタン」を追加するかと選択する設定を追加。（Thanks @R18otomegame on Twitter）
  Added: Added so that you can set the Read more button.
* 設定画面の誤記を修正。
  Fixed: The mistyping was corrected.
* 設定画面の設定項目を再配置。
  Modified: The setting items on the setting screen have been relocated.
* 設定画面にバージョン表記を追加。
  Modified: Version was written on setting screen.

= 2.0.8 =
* WordPress 4.9.4 での動作確認。
  Compatible with WordPress 4.9.4
* 設定画面の、ショートコードの表示を修正。
  Fixed: Fixed so that the short code is displayed immediately on the setting screen.
* 設定画面に、スタイルシートを追加する設定を追加。
  Fixed: Fix to be able to add stylesheet.
* カード管理画面で警告エラーが発生する不具合を修正。
  Fixed: Fixed a bug.

= 2.0.7.2 =
* WordPress 4.9.2 での動作確認。
  Compatible with WordPress 4.9.2
* 設定画面の一部が日本語表記になっていなかったのを修正。
  Fixed: A part of the setting screen was not written in Japanese was fixed.

= 2.0.7.1 =
* バグ修正。
  Fixed: Fixed a bug.

= 2.0.7 =
* WordPress 4.9 での動作確認。
  Compatible with WordPress 4.9
* 記事では無いページでURL指定エラーが発生する不具合を修正。（特定のURLを除外）
  Modified: Exclude some URLs from errors.
* 設定画面に、サブディレクトリ型のマルチサイトのとき、メインサイトからサブサイトを外部リンクと判定する設定を追加。
  Added: In the case of the multi-site of the subdirectory type, the site under the subdirectory is judged as an external site.

= 2.0.6 =
* URLパラメーターが無効な場合にURL指定エラーを表示する機能を追加。
  Added the function to display URL parameter.

= 2.0.5 =
* 内部リンクの記事ID取得が失敗した場合に外部アクセスする機能を追加。（サイト全体に負荷がかかる可能性があります）
  Added: If the PostID can not be acquired, the URL of the redirect destination is acquired.

= 2.0.4.1 =
* 設定画面に、アクセスされたURLの末尾が「/?amp=1」だったとき、簡易表示する設定を追加。（Google AMP暫定対応）
  Added: Simple display if the end of URL is "/?amp=1".
* ドキュメント（readme.txt）修正。
  Fixed: Fixed a typo in "readme.txt".

= 2.0.4 =
* WordPress 4.8.2 での動作確認。
  Compatible with WordPress 4.8.2
* 「外部リンクにはてなブログカードを使用」した際のURLを変更。
  Modified: Hatena URL changed.
* ショートコード記述時のURLの記述ミスに対応。
  Modified: Corresponded to URL mistake.
* 「押しピン」の画像を変更。
  Modified: Changed the image of "push pin".
* 設定画面の「かんたん書式設定」にWordPress標準ブログカード風の「スクエア」を追加。
  Added: Tiny format 'Square'.
* 設定画面の「サムネイルの位置」に「上側」を追加。
  Added: "Upper" has been added to the position of the thumbnail.

= 2.0.3 =
* 設定画面に、404エラーのときでもリンクを有効にする設定を追加。（Thanks @toru1231 on Twitter）
  Added: Added setting to enable link even on 404 error.
* 内部リンクの抜粋文が取得できていなかったのを修正。
  Fixed: Fixed an excerpt of the internal link could not be acquired.
* 外部リンクのサムネイル取得が失敗する不具合を修正。
  Fixed: Fixed a bug that you can not acquire thumbnails of external links.

= 2.0.2 =
* 外部リンクの場合、サイトアイコンURLを取得するように修正。
  Fixed: Fix to get URL of site icon.
* サムネイルURL、サイトアイコンURLが相対パスの場合に絶対パスに変換するように修正。
  Modified: Corresponds to relative specified URL.
* パラメータが誤っているときに設定エラーが表示されない場合があったのを修正。
  Fixed: Fix to display error when parameter is wrong.

= 2.0.1.1 =
* 警告エラーが発生する不具合を修正。
  Fixed: Fixed a bug.

= 2.0.1 =
* 内部リンクのカテゴリーページ／タグページに対応。
  Added: Supported display of category page.

= 2.0.0.3 =
* 内部リンクが取得できない不具合を修正。（Ver.2.0.0.2から発生）
  Fixed: Fixed a bug.

= 2.0.0.2 =
* 未実装のJavaScriptを呼び出し、エラーがサーバーログに出力される不具合を修正。
  Fixed: Fixed a bug.

= 2.0.0.1 =
* idn_to_utf8()が実装されていない環境で警告エラーが発生する不具合を修正。
  Fixed: Fixed a bug.

= 2.0.0 =
* ショートコードでURLを指定する際に「href」も使用できるように変更。（Thanks @weblearninglog on Twitter）
  Modified: "href" was added to the parameter that specifies the URL.
* 設定画面に、テキストエディタへ「クイックタグ」を追加する設定を追加。（Thanks @kumasan_kenkou on Twitter）
  Added: A quick tag was added to the text editor.
* 設定画面に、ビジュアル エディタへ「リンクカード作成」を追加する設定を追加。
  Added: A card insertion button was added to the visual editor.
* 設定画面に、テキストリンクだけが記載されている行をリンクカードに変更する機能を追加。
  Added: Added the function to convert text link to card.
* 設定画面に、URLだけが記載されている行をリンクカードに変更する機能を追加。（Thanks @hina01011 on Twitter）
  Added: Added the function to convert URL to card.
* カード管理画面のタイトルと抜粋文を変更されている場合に太文字で表示するように変更。
  Modified: Changed so that changed parts are displayed in bold letters on the card management screen.
* 設定画面に、国際化ドメイン（IDNA ASCIIドメイン）に対応する設定を追加。（Thanks @ichinosecom on Twitter）
  Added: It supports display of IDNA ASCII domain.

= 1.8.2 =
* スタイルシートのURLからスキーム（http:やhttps:）を省略するように変更。（Thanks @mataku_hair on Twitter）
  Modified: The style sheet URL was corrected.
* InstantWPで使用した場合にカード管理画面が文字化けするのを修正。（Thanks aya）
  Fixed: Fixed garbled characters on the management screen.
* 外部リンクのサムネイルの保存ディレクトリを変更。
  Modified: Changed directory to save thumbnails.
* カード管理画面を狭い画面で見ると表示が崩れるのを修正。
  Fixed: Fixed display collapse of the management screen.
* カード管理画面の文字セットの列を非表示に変更。
  Modified: The character set column of the management screen was deleted.
* カード管理画面のソーシャルカウントの表示を複数列から1列に変更。
  Modified: Changed the social count column of the management screen.
* カード管理画面に外部リンクのサムネイルの表示を追加。
  Added: Added display of thumbnail to the management screen.

= 1.8.1 =
* WordPress 4.8 での動作確認。
  Compatible with WordPress 4.8
* 内部リンクのサムネイル取得について、フルサイズ画像を取得していたのを修正。(Thanks @cstudyupdate on Twitter）
  Fixed: Fixed a bug. Corrected the size of thumbnail to be acquired.
* 設定画面の「外部リンク」タブの、「サムネイルの取得方法」で「直接取得」を選択可能に変更。
  Modified: Modified to be able to select "Direct" from "Thumbnail" on the "External Link" tab of the setting screen.
* 設定画面の「かんたん書式設定」にはてなブログカード風の「シンプル」を追加。
  Added: Tiny format 'Simple'.

= 1.8.0 =
* 設定画面のカラーコード入力にチェックを追加。
  Added: Added color code check.
* 設定画面に、アクセスされたURLの末尾が「/amp」「/amp/」だった場合に簡易表示する設定を追加。（Google AMP暫定対応）（Thanks @misoji_13 on Twitter）
  Added: Simple display if the end of URL is "/amp".
* 設定画面の「かんたん書式設定」に「押しピン」を追加。（Thanks @kautakku on Twitter）
  Added: Tiny format 'Pushpin'.

= 1.7.9.1 =
* 抜粋文の文字フォントサイズが枠線のものになってしまう不具合を修正。（Thanks @cgrio0822 on Twitter）
  Fixed: Fixed a bug. Incorrect font size of excerpt.

= 1.7.9 =
* キャッシュ用DBが作成されず、CPUが高負荷になってしまう不具合を修正。
  Fixed: Fixed a bug that table is not created.
* METAタグの名前が大文字が混ざっていると取得できなかったのを修正。（Thanks @J_kindan on Twitter）
* 内部リンクが取得できない時に外部アクセスしていたのが高負荷に繋がっていたため、外部アクセスしないように修正。（Thanks @J_kindan on Twitter）
  Fixed: Fixed a high load bug.

= 1.7.8 =
* キャッシュ用DBが作成されず、CPUが高負荷になってしまう不具合を修正。（Thanks @J_kindan on Twitter）
  Fixed: Fixed a bug that table is not created.

= 1.7.7 =
* アイキャッチ画像が設定されていないテーマの場合に警告エラーが発生する不具合を修正。（Thanks enomoto , sato）
  Fixed: Fixed a bug.

= 1.7.6 =
* 設定画面に、用例等を追加。
  Added: Add tips at settings screen.
* 設定画面の「かんたん書式設定」に「縫い目」を追加。（Thanks @i_tsu_tsu on Twitter）
  Added: Tiny format 'Stitch'.
* 設定画面に、サムネイルのサイズの設定を追加。（Thanks @misoji_13 on Twitter）
  Modified: Able to change the size of the thumbnail.

= 1.7.5 =
* WordPress 4.7.1 での動作確認。
  Compatible with WordPress 4.7.1.
* アクティベート／バージョンアップ時に重複データを削除する機能を追加。
  Cleaning up garbage from the database at activation.
* 設定画面の項目追加と整理。
  Modified: Cleaned up the settings screen.
* 設定画面に用例等を追加。
  Added: Add tips at settings screen.
* 設定画面に、サイト情報、タイトル、URL、抜粋文部分の行の高さを追加。（Thanks @keitaihoo on Twitter）（Thanks @ud_fibonacci on Twitter）
  Added: Added setting. "Height" in letter.
* 設定画面に、「ドメイン名のみ」以外の場合でも末尾のスラッシュを除去する設定を追加。
  Added: Added setting. Trailing slash.
* facebookのシェア数が取得できなくなっていたのを修正。（Thanks @i_tsu_tsu on Twitter）
  Modified: Fixed that the number of shares of facebook could not be obtained.
* カード管理画面での内部リンクの判定方法を修正。
  Modified: Corrected the method of determining internal links on the Pz card management screen.
* 内部リンクのキャッシュが正常に作成されない場合があったのを修正。（Thanks @i_tsu_tsu on Twitter）
  Fixed: Fixed not being cached properly when using internal links.
* 内部リンクをキャッシュから取得した場合に画像が表示されなかったのを修正。（Thanks @i_tsu_tsu on Twitter）
  Fixed: Fixed the image not being displayed properly when using an internal link.
* 設定画面に、リンク先がリダイレクトされているときに追尾するかどうかの設定を追加。（Thanks @fumieblog on Twitter）
  Added: Added a setting so that you can choose whether to track when the link destination is redirected.
* 設定画面に、リンク先がリンク切れになっているかチェックするかどうかの設定を追加。（Thanks @misoji_13 on Twitter）
  Added: Added a setting so that you can choose whether to check if the link destination is broken.
* 設定画面に、リンク先がリンク切れの場合、Aタグを無効にするかどうかの設定を追加。
  Added: Added a setting so that you can choose whether to disable the A tag when the link destination is broken.
* WebAPIに使用しているURLのデフォルトをSSL対応のものに変更。（Thanks @fumieblog on Twitter）（Thanks @hareannie01 on Twitter）
  Modified: Supports SSL for WebAPI URL.

= 1.7.4 =
* キャッシュ用DBが作成されず、CPUが高負荷になってしまう不具合を修正。
  Fixed: Fixed a bug that table is not created.

= 1.7.3 =
* ドメイン名が取得できていない不具合を修正。
  Fixed: Fixed a bug that domain-name disappears.

= 1.7.2 =
* WordPress 4.5.13 での動作確認。
  Compatible with WordPress 4.5.13.
* WordPress 4.5.14 での動作確認。
  Compatible with WordPress 4.5.14.
* WordPress 4.5.15 での動作確認。
  Compatible with WordPress 4.5.15.
* WordPress 4.5.16 での動作確認。
  Compatible with WordPress 4.5.16.
* WordPress 4.5.17 での動作確認。
  Compatible with WordPress 4.5.17.
* WordPress 4.5.18 での動作確認。
  Compatible with WordPress 4.5.18.
* WordPress 4.5.19 での動作確認。
  Compatible with WordPress 4.5.19.
* WordPress 4.5.20 での動作確認。
  Compatible with WordPress 4.5.20.
* WordPress 4.5.21 での動作確認。
  Compatible with WordPress 4.5.21.
* WordPress 4.5.22 での動作確認。
  Compatible with WordPress 4.5.22.
* WordPress 4.5.23 での動作確認。
  Compatible with WordPress 4.5.23.
* WordPress 4.5.24 での動作確認。
  Compatible with WordPress 4.5.24.
* WordPress 4.5.25 での動作確認。
  Compatible with WordPress 4.5.25.
* WordPress 4.5.26 での動作確認。
  Compatible with WordPress 4.5.26.
* WordPress 4.5.27 での動作確認。
  Compatible with WordPress 4.5.27.
* WordPress 4.5.28 での動作確認。
  Compatible with WordPress 4.5.28.
* WordPress 4.6 での動作確認。
  Compatible with WordPress 4.6.
* 幅に合わせて縮小を有効にしたとき、サムネイルと合わせて文字サイズも小さくするように修正。（Thanks @fumieblog on Twitter）
  Modified: Modified so as also to small character size to fit the size of screen.
* カード管理画面で再取得時にソーシャルカウントが消えてしまう不具合を修正。（Ver.1.7.1から発生）（Thanks @i_tsu_tsu on Twitter）
  Fixed: Fixed a bug that social count disappears.
* 内部リンクの画像が取得できない不具合を修正。（Ver.1.7.1から発生）（Thanks @i_tsu_tsu on Twitter）
  Fixed: Fixed a bug that thumbnail can not display.
* マルチサイトへの対応方法が誤っていたため修正。（Ver.1.7.1から発生）（Thanks @kyutechnabe on Twitter）
  Fixed: When the multi-site, fixes a bug that setting is not properly reflected.

= 1.7.1 =
* 記事内容がキャッシュされない不具合を修正。（Thanks @i_tsu_tsu on Twitter）
  Fixed: Fixed a bug that article content can not be acquired.
* 取得エラーが発生するサイトのサムネイルを表示しないように修正。（Thanks @misoji_13 on Twitter）
  Modified: Time of the error, modified so that it does not display the thumbnail.
* マルチサイトへの仮対応。（Thanks @kyutechnabe on Twitter）
  Modified: Modification of the order to respond to multi-site.

= 1.7.0 =
* ドメイン名のみのときに最後のスラッシュを削除する機能を追加。（Thanks @toru1231 on Twitter）
  Added: Added setting. "In the case of domain names, to ignore the trailing-slash".
* 設定画面の「定型書式」に「小麦色」を追加。（Thanks @fumieblog on Twitter）
  Added: Added border "Wheat'.

= 1.6.9 =
* WordPress 4.5.3 での動作確認。
  Compatible with WordPress 4.5.3.
* 設定画面で表示幅によってサムネイルを調整する「幅に合わせて縮小」を初期選択するように変更。
  Modified: Scaled down to fit the screen size in setting. Default change "disabled" to "enabled".
* Twitter代替WebAPI「count.jsoon」を使用してツイート数の取得に対応。
  Modified: Use an alternative WebAPI to get the Twitter count.
* 設定画面で、内部リンクのときでWordPress標準のサイトアイコンが設定されていない場合、内部取得を選べないように修正。（Thanks @meiko2285 on Twitter）
  Fixed: Fix the method of acquiring the site icon in the internal site.
* 設定画面に、内部リンクのときでサムネイルが設定されていない場合、WebAPIを利用できる設定を追加。（Thanks @fumieblog on Twitter）
  Added: Added thumbnail acquisition method at the internal links.
* 設定画面に、SSL証明書の検証を無効にできる設定を追加。
  Added: Added the ability to disable the verification of SSL certificate.
* リンク切れチェック機能の追加にあたってプログラムを一部見直し。(Thanks @misoji_13 on Twitter）

= 1.6.8 =
* WordPress 4.4.1 での動作確認。
  Compatible with WordPress 4.4.1.
* WordPress 4.4.2 での動作確認。
  Compatible with WordPress 4.4.2.
* WordPress 4.4.15 での動作確認。
  Compatible with WordPress 4.4.15.
* WordPress 4.4.16 での動作確認。
  Compatible with WordPress 4.4.16.
* WordPress 4.4.17 での動作確認。
  Compatible with WordPress 4.4.17.
* WordPress 4.4.18 での動作確認。
  Compatible with WordPress 4.4.18.
* WordPress 4.4.19 での動作確認。
  Compatible with WordPress 4.4.19.
* WordPress 4.4.20 での動作確認。
  Compatible with WordPress 4.4.20.
* WordPress 4.4.21 での動作確認。
  Compatible with WordPress 4.4.21.
* WordPress 4.4.22 での動作確認。
  Compatible with WordPress 4.4.22.
* WordPress 4.4.23 での動作確認。
  Compatible with WordPress 4.4.23.
* WordPress 4.4.24 での動作確認。
  Compatible with WordPress 4.4.24.
* WordPress 4.4.25 での動作確認。
  Compatible with WordPress 4.4.25.
* WordPress 4.4.26 での動作確認。
  Compatible with WordPress 4.4.26.
* WordPress 4.4.27 での動作確認。
  Compatible with WordPress 4.4.27.
* WordPress 4.4.28 での動作確認。
  Compatible with WordPress 4.4.28.
* WordPress 4.4.29 での動作確認。
  Compatible with WordPress 4.4.29.
* WordPress 4.5 での動作確認。
  Compatible with WordPress 4.5.
* WordPress 4.5.1 での動作確認。
  Compatible with WordPress 4.5.1.
* WordPress 4.5.2 での動作確認。
  Compatible with WordPress 4.5.2.
* 警告エラーが発生する不具合を修正。(@junya_0606)
  Fixed: Fixed a notice.
* 指定したリンク先によってはMETAタグを内部テーブルに展開するのに失敗して致命的エラーが発生する不具合を修正。(Thanks @misoji_13 on Twitter）（Thanks @ryu-blacknd on Twitter）
  Fixed: Fixed an error. In had failed Perth META tags.
* カード管理画面のPHPショートタグを使用しないように修正。(Thanks @toru1231 on Twitter）
  Fixed: Fixed so as not to use PHP-short-tags.

= 1.6.7 =
* 設定画面にて、内部リンクの記事抜粋方法を選択できるように修正。（Thanks @okamurajun on Twitter）
  Added: Added a method of article excerpt internal link in setting.

= 1.6.6 =
* 設定画面に「画面の幅によってサムネイルを小さくする」機能を追加。（Thanks 弁保社長）
  Added: Scaled down to fit the screen size in setting.

= 1.6.5 =
* WordPress 4.4 での動作確認。
  Compatible with WordPress 4.4.
* 設定画面に文字のふちどり指定を追加。(Thanks @okaerinasainet on Twitter）
  Added: Add a border of letters in setting.
* facebookのシェア数取得WebAPIのURLが誤っていたため修正。
  Fixed: Fixed incorrect facebook WebAPI URL.

= 1.6.4 =
* facebookのシェア数が2以上でも1と表示されていたのを修正。（Thanks 弁保社長）
  Fixed: Shares of facebook has not been able to properly get.
* 設定画面にリンクカードのDIV要素に任意のクラス名を設定できるように追加。（Thanks @misoji_13 on Twitter）
  Added: Grant function of any class name.

= 1.6.3 =
* 「Twitter純正WebAPI」の公開終了に伴ってツイート数取得処理を削除。設定画面に更新されない旨のメッセージを追加。
  Modified: Correspondence associated with the end Tweets number acquiring WebAPI.
* 設定画面のツイート数表示の初期選択を「表示しない」に変更。
  Modified: Changed the initial selection of the number of tweets display on the setting screen to "Hide".
* カード管理画面からソーシャルカウントの再取得を行ったとき、処理を二度行っていたので修正。（Ver.1.6.0から発生）
  Fixed: Bugfix.

= 1.6.2 =
* サンフランシスコ時間で11月20日を経過したが「Twitter純正WebAPI」でツイート数が取得できているので制限を一時的に解除。
  Modified: Deadline of Tweets number get me grew day.

= 1.6.1 =
* 標準時間で11月20日を経過したが「Twitter純正WebAPI」でツイート数が取得できているので制限を一日延長。
  Modified: Deadline of Tweets number get me grew day.

= 1.6.0 =
* リンク先の取得に wp_remote_get() を使用していたのを、cURL に変更。
  Modified: Acquired without the wp_remote_get, modified to use a cURL.
* charsetの取得方法を変更。
  Modified: Fixed character set acquisition method.
* ソーシャルカウントの取得をスケジュール方式に変更。
  Modified: Fixed social count set acquisition method.
* 「カード内側の余白」の設定を追加と、それに伴うCSS修正。（Thanks yunosuke）
  Added: Add the margins of the inner card.

= 1.1.1 =
* METAタグの取得方法を修正。
  Fixed: Fixed to had failed parsing of meta tags.

= 1.1.0 =
* 2015年11月20日に「Twitter純正WebAPI」が廃止される事に伴い、同日以降取得しないように修正。
  Modified: Since November 20, 2015 , it does not use the Twitter WebAPI.
* 設定画面の「新しいウィンドウで開く」をチェックボックスからリストに変更。
  Modified: Change "Open in new window" from the check box to the list on the setting screen.
* 設定画面の「新しいウィンドウで開く」に「モバイル以外（パソコンのみ新しいウィンドウで開く）」を追加。（Thanks @misoji_13 on Twitter）
  Added: Added "Other than mobile" to "Open in new window" on the settings screen.

= 1.0.3 =
* キャッシュ保存時にキーが正しく設定されない事があったのを修正。
* カード管理画面で内部ID（連番）の表示を追加。
* 設定画面の「定型書式」に「紙がめくれる効果」を修正。（テーマによってはレイアウトが崩れる可能性があります）
* 設定画面の「定型書式」に「テープと紙めくれ」を追加。（テーマによってはレイアウトが崩れる可能性があります）

= 1.0.2 =
* カード管理画面でキャッシュを編集したとき、一部の文字をエスケープしていなかったのを修正。
* バージョンアップの度に一部のパラメータがデフォルトに戻っていたのを修正。
* プログラム内でのキャッシュの読み書き方法の改善。

= 1.0.1 =
* カード管理画面でキャッシュを編集したとき、内部IDがクリアされてしまう不具合を修正。

= 1.0.0 =
* 全体的なプログラムの見直し。
  * URLが空欄等の場合の対応。
  * 文字エンコードまわりを修正。
  * DBキャッシュまわりを修正。
* ショートコードの囲い文字の扱いの仕様変更。
  * ショートコード1にのみ適用されるように修正。
  * タイトルがURLになってしまう不具合修正。
* ショートコード3を解放。
* カード管理画面を修正。
  * リンク先単体の「編集」「再取得」「削除」が行えるように修正。
  * 一括処理に「再取得」を追加。
  * 抽出条件にドメイン名を追加。
  * 内部リンクのURLにもリンク（Aタグ）を追加。
  * ページング機能を追加。

= 0.1.4 =
* <head>にprefix等があるときに、metaタグの解析に失敗していたのを修正。
* パラメータに閉じの「半角角かっこ（大かっこ）」がある場合に、URLに余分なコードが入ってしまう不具合を修正。

= 0.1.3 =
* content=''となっているOGP情報は無視するように修正。
* metaタグ表記にシングルクォートが使われている場合でも取得できるように修正。
* 設定画面の定型書式に「Pzカード標準書式」を使用し、「サイト情報」を「下側」にしている場合、サイト名が見えなくなる不具合を修正。
* カード管理画面のセキュリティを強化。
* 設定画面の「サイト情報」の位置を追加。
* 設定画面に「サイト情報」と「記事内容」の間を区切るための「区切り線」を追加。
* サムネイル取得WebAPIの初期設定をWordPress.comのものに変更。
* タイトルや抜粋文をパラメータ等で設定した場合にもHTML等を除去するように変更。

= 0.1.2 =
* 「新しいウィンドウで開く」の設定を追加。
* カード管理画面のソート順を修正。
* facebookの表記を「f」から「fb」へ変更。

= 0.1.1 =
* 公開後発見されたバグを修正。

= 0.1.0 =
* 公式プラグインディレクトリでの最初の公開バージョン。

= 0.0.1 =
* サイト「ぽぽづれ」内での最初の公開バージョン。

= 0.0.0 =
* 途中まで作成していたバージョンを破棄。
* Pz-HatenaBlogCard Ver.1.2.5 を元にDBアクセス部分を移植してPz-LinkCardを作成。
* サイト「ぽぽづれ（開発環境）」での動作検証。
* サイト「ぽぽづれ」での動作検証。


== Upgrade notice ==


== Arbitrary section ==

= Display and DB cache =

This plug-in one create a DB table when you have activated. (Prefix + "pz_linkcard")

Open the pages of the article when the "For the first time it appears " , and caches by obtaining the title excerpt from the linked site to the DB.

Therefore , the display for the first time is slow , the second and subsequent display is fast.


= Create files =

CSS file are stored in a custom folder under "/wp-content/Uploads".


= Use Web API =

Number of SNS share have been acquired by the JSON request.

* Twitter ... https://jsoon.digitiminimi.com/twitter/count.json?url=[URL]

* Facebook ... https://graph.facebook.com?fields=og_object{engagement}&id=[URL]

* Hatena ... http://api.b.st-hatena.com/entry.count?url=[URL]

* Pocket ... https://widgets.getpocket.com/api/saves?url=[URL]

Displays using the "Google-favicon API" to get the favicon. This can be changed.

Displays using the "WordPress.org mshots API" to get the thumbnail. This can be changed.


= 表示とキャッシュ =

このプラグインは、有効化したときにDBテーブルを一つ作成します。（プレフィックス＋「pz_linkcard」）

外部リンクを設定した場合、記事のページを開いて「初めて表示された」ときに、リンク先のサイトからタイトル・抜粋文を取得してDBへキャッシュします。

外部リンクを設定した場合、カードの枚数分だけ外部サイトへのアクセスが発生するため多量のリンクを作成すると、記事をプレビューした時等、最初の表示に時間がかかります。

次回の表示はDBキャッシュから行うので高速に表示を行います。

（内部でのDBアクセスが発生しますが、通常は軽微なものです。カード1枚表示のたびに、取得のために1クエリ発行します。更新が発生した場合には挿入・更新のためのクエリが1回発生します。）


= ソーシャルカウントの取得 =

ソーシャルカウントについては、「Twitter（ツイッター）のツイート数」「facebook（フェイスブック）のシェア数」「はてなブックマークのブックマーク数」「Pocketの登録数」の4種類に対応しています。

それぞれWebAPIを使用して値を取得します。

バックグラウンドで取得するため、ページの表示速度には影響がありません。

取得した値はタイトルや抜粋文と同様、DBへキャッシュを行うため、直近の表示にはWebAPIアクセスが発生しません。

ソーシャルカウントの再取得は、最後の取得から4時間～36時間程度のランダムな時間で行います。

また、各WebAPIについては、仕様変更やサービス終了に伴い、正常に取得できなくなる場合があります。


= 画像取得WebAPIの利用 =

設定画面からサムネイル取得WebAPIが指定できます。

「WebAPIを利用する」にする事でページのスクリーンショット画像を取得します。

参考．画像取得WebAPIの設定について https://popozure.info/20151004/9317


設定画面からサイトアイコン取得WebAPIが指定できます。

サイトアイコンの場所はサイトによってバリエーションが多いため、WebAPIを使用する前提となります。

正式に公開されているWebAPIでは無いため、仕様変更やサービス終了に伴い、正常に取得できなくなく場合があります。


= その他 =

Pz-HatenaBlogCard からの設定引き継ぎ機能はありません。この機会に触った事のなかった設定項目にも触れていただければ幸いです。

ショートコードを変える事で、Pz-HatenaBlogCard と併用利用する事ができますが、通常はリソース消費が増えるだけなので、推奨はしません。


ショートコード内にURLを記述した場合、WordPressピンバックは飛びません。


設定項目については、WordPress標準の options に設定内容を保存します。キーは「Pz-LinkCard_options」の1レコードです。


なお、アンインストールを行う際には、キャッシュを保管するDBテーブルと、options内の設定ファイルは削除されます。

アンインストール時の削除に関してはプラグインディレクトリ内の uninstall.php で行っています。
