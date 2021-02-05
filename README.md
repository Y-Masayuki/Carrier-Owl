# Slack astroph
## About Slack astroph
- Carrier-Owlさんのデータを参考にしました。
<img src='./data/images/system.png' width='1000'>

- 2日前のarxivから気になる論文にスコアを付けてslackに通知するシステムです。  
- 通知の際に、abstractをDeepLで翻訳しています。  
- スコアは、ターゲットとなるキーワードに重み付けをして決まります。(例 resnet=5, kaggle=3, audio=3)    
- ユーザーが**好きな領域**、**好きなキーワード**を登録することで、通知される論文は変わります。

- 登録キーワード例 (**config.yaml**に入力します)
    ```
    # arxivの学問領域の指定
    subject: 'astro-ph'

    # 検索キーワード
    keywords:
            protoplanetary disk: 1
            circumstellar disk: 1
            protoplanet: 1
            pre-main sequence: 1
            debris disk: 1
            T Tauri star: 1
            transition disk: 1
            planet formation: 1
            radio interferometry: 1
            sparse modeling: 1
            protostar: 1
            SETI: 1
    # 通知の閾値
    score_threshold: 0

    ```
