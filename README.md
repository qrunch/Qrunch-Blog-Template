# Qrunch Blog Template
Qrunch（クランチ）のブログテンプレートです。  
<br />
Qrunchで作成した全てのブログの雛形HTMLとなりますので、デザインテーマを制作する際や、カスタマイズをする際はこちらのリポジトリを参考にしてください。  
<br />
このテンプレートは一部例外を除いて、「[BEM](https://en.bem.info/)」を元にマークアップ設計しています。  
<br />
公式デザインテーマ：「[Editorial](https://google.com)」（初期設定）  
<br />

## ページ構成
トップページ  
┣ 記事一覧  
┃　　┗ 記事ページ  
┣ ログ一覧  
┃　　┗ ログページ  
┣ アーカイブ  
┃　　┣ 年別アーカイブ　　　　（記事）  
┃　　┣ 　　　〃　　　　　　　（ログ）  
┃　　┣ 月別アーカイブ　　　　（記事）  
┃　　┣ 　　　〃　　　　　　　（ログ）  
┃　　┣ 日別アーカイブ　　　　（記事）  
┃　　┣ 　　　〃　　　　　　　（ログ）  
┃　　┣ カテゴリー別アーカイブ（記事）   
┃　　┣ 　　　〃　　　　　　　（ログ）  
┃　　┣ タグ別アーカイブ　　　（記事）  
┃　　┗ 　　　〃　　　　　　　（ログ）  
┣ 検索ページ（記事）  
┗ 　　〃　　（ログ）

<br />

## 各ページの概要
| ページの種類 | URL（パス） |
| --- | --- |
| トップページ | / |
| 記事一覧 | /entries |
| 記事ページ | /entries/{{entry_id}} |
| ログ一覧 | /logs |
| ログページ | logs/{{log_id}} |
| アーカイブ | /archive |
| 年別アーカイブ | 記事：/archive/date/{{ year }}/entries<br>ログ：/archive/{{ year }}/logs |
| 月別アーカイブ | 記事：/archive/date/{{ year }}/{{ month }}/entries<br>ログ：/archive/{{ year }}/{{ month }}/logs |
| 日別アーカイブ | 記事：/archive/date/{{ year }}/{{ month }}/{{ day }}/entries<br>ログ：/archive/{{ year }}/{{ month }}/{{ day }}/logs |
| カテゴリー別アーカイブ | 記事：/archive/category/{{ entry_category_id }}/entries<br>タグ：/archive/category/{{ log_category_id }}/logs |
| タグ別アーカイブ | 記事：/archive/tag/{{ entry_tag_id }}/entries<br>タグ：/archive/tag/{{ log_tag_id }}/logs |
| 検索ページ | 記事：/search?q={{word}}&content_type=entry<br>ログ：/search?q={{word}}&content_type=log |

<br />

## ファイル構成
| ファイル名（/src/） | URL（パス） |
| --- | --- |
| index.html | / |
| /entries/index.html | /entries |
| /entries/entry.html | /entries/{{entry_id}} |
| /logs/index.html | /logs |
| /logs/log.html | /logs/{{log_id}} |
| /archive/date/entries.html | /archive/date/{{ year }}/entries<br>/archive/{{ year }}/{{ month }}/entries<br>/archive/{{ year }}/{{ month }}/{{ day }}/entries |
| /archive/date/logs.html | /archive/date/{{ year }}/logs<br>/archive/{{ year }}/{{ month }}/logs<br>/archive/{{ year }}/{{ month }}/{{ day }}/logs |
| /archive/category/entries.html | /archive/category/{{ entry_tag_id }}/entries |
| /archive/category/logs.html | /archive/category/{{ log_tag_id }}/logs |
| /archive/tag/entries.html | /archive/tag/{{ entry_tag_id }}/entries |
| /archive/tag/logs.html | /archive/tag/{{ log_tag_id }}/logs |
| /search/entries.html | /search?q={{word}}&content_type=entry |
| /search/log.html | /search?q={{word}}&content_type=log |
| commons.html | /* （全ページ共通のHTML） |
