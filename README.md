# Dota2watcher
Dota2配信を自動でツイートしてくれる便利なやつ。

# 使ったもの
Python 3.5.2  
OAuthのライブラリは<https://github.com/requests/requests-oauthlib>  
`$ pip install requests requests_oauthlib`でインストールできる

# 問題点と解決策
ツイート140文字超えると多分死ぬ  
→配信タイトルを一定の長さで切る  
  
コード中にAPIトークンを書かないようにする  
→環境変数設定してそこから持ってくるようにする  
  
コード中にユーザーを書いているのよくない  
→データベース使う  

# メモ
2月くらいにTwitch APIの仕様が変わる  
https://blog.twitch.tv/action-required-twitch-api-version-update-f3a21e6c3410#.hupl0lrcd
