# wiki_model_bin_splited
## 日本語版wikipediaの全文fasttextに学習させたデータです
    - 日本語版wikipediaをDLし、パース後、mecabで形態素解析したデータをfasttextに学習させたデータを40MBごとに分割しました
        - 学習はfasttextのデフォルトの設定で行いました
        - (補足) wikipediaのデータは20170120のバージョンのものを利用しました
            - https://dumps.wikimedia.org/jawiki/20170120/ 
        - (補足) wikipediaのパースにはWikipedia_Extractorを使用 
            - http://medialab.di.unipi.it/wiki/Wikipedia_Extractor を使用
        - (補足) 辞書はmecab-ipadic-neologdを使用
            - https://github.com/neologd/mecab-ipadic-neologd を使用

## 利用方法
    - このリポジトリをclone後、$ cat wiki_model.bin.* > wiki_model.bin を実行してください
        - (補足) githubのルール上、50MB以上のファイルはアップロードできないため、spliteコマンドで分割してアップしました。
