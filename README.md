【flask 操作メモ】

＊正しくはvscをご参照ください

VSCとターミナル（コマンドプロンプト）を使用

①VSCでフォルダ作成
②cmdを使って仮想環境の構築（venv）
③Flaskのインストール
④メインフォルダ内にpythonファイル（.py）を作成
⑤.pyにコードを入力
⑥Flask runで実行
⑦http://localhost:5000/に表示


＜仮想構築＞
python -m venv ./venv

＜仮想開始＞
venv＼Scripts＼activate

＜仮想内にFlaskインストール＞
pip install Flask

＜無効化メモ＞
venv＼Scripts＼deactivate　

＜layout.html＞
<!DOCTYPE html>
<html>
<head>
    <titile>{{ title }}</titile>
</head>
<body>
    {% block content %}
    <!-- main-->
    {% endblock %}
</body>
</html>

＜続きhtml＞
<!-- layout.htmlをテンプレートに拡張する-->
{% extends "layout.html" %}
<!-- block content ~ endblock-の範囲がテンプレートの同宣言範囲に差し込まれる -->
{% block content %}
<h3>Hello</h3>
こんにちは。{{ name }}さん。
{% endblock %}

＜デバッグモード＞
app.run(debug=True, use_reloader=False, use_debugger=False) 

＜GETメソッド＞
<form action="/calc" method="GET">
    <input type="hidden" Number="part" value="bass">
    <input type="text" Number="members[number]">
    <input type="submit"> 
  </form>
</body>


＜アップグレード控え＞
pip install --upgrade pip　（venv内では使えない）

＜環境書き出し＞
pip freeze > requirements.txt


＜参考資料＞
https://qiita.com/probabilityhill/items/18b6ac07df89b9859fa4


●Jinja2の拡張機能のインストール忘れに注意！
