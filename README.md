# サクッと簡単！flask操作メモ

GETメソッドなど、詳しくは別ファイルの「vsc」をご参照ください。

VSCとターミナル（コマンドプロンプト）を使用

<p>①VSCでフォルダ作成</p>
<p>②cmdを使って仮想環境の構築（venv）</p>
<p>③Flaskのインストール</p>
<p>④メインフォルダ内にpythonファイル（.py）を作成</p>
<p>⑤.pyにコードを入力</p>
<p>⑥Flask runで実行</p>
<p>⑦http://localhost:5000/に表示</p>


＜仮想構築＞
python -m venv ./venv

＜仮想開始＞
venv＼Scripts＼activate

＜仮想内にFlaskインストール＞
pip install Flask

＜無効化メモ＞
venv＼Scripts＼deactivate　



＜アップグレード控え＞
pip install --upgrade pip　（venv内では使えない）

＜環境書き出し＞
pip freeze > requirements.txt


＜参考資料＞
https://qiita.com/probabilityhill/items/18b6ac07df89b9859fa4


●Jinja2の拡張機能のインストール忘れに注意！
