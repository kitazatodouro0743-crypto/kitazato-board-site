全体管理表（打合せボード）の公開用リポジトリ

ここに入れてよいのは、StatiCrypt で合言葉をかけた（暗号化した）HTML と board_salt.json だけ。
元のボード（金額・人名入り）は絶対に入れない。元はそれぞれの工事フォルダ（Dropbox）や平川さんのPCにある。

置き方：スキル koji-zentai-board の scripts/build-publish.js（工事ごとの設定ファイルを渡す）。
  自分の工事のファイルだけ書き換えて push する。push すると GitHub Pages が同じURLに出す（1〜2分）。
  このリポジトリは公開（GitHub Pages を無料で使うため）。中身は暗号文だけなので、合言葉なしでは読めない。
board_salt.json を消したり変えたりしない（見る人が合言葉を入れ直すことになる）。
合言葉は各PCの %LOCALAPPDATA%\kitazato-private\<工事番号>_board_pass.txt（ここに書かない）。
