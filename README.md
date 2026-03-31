# lol-rank-analysis-pings

# 概要
LoLの対戦データからコミュニケーション（Pings）の量がランクに影響するかを統計的に分析するものです。
Riot APIを用いて下位（アイアン）から上位（ダイアモンド）までの各区分（Ⅰ〜Ⅳ）、および最上位（マスター以上）の各層において、それぞれ一律2,500試合ずつのデータを抽出します。
分析手法として、基礎統計・相関分析を層別分析と組み合わせ、Pingsの頻度と習熟度の関係性の抽出と可視化を行います。

# 使用技術
Python 3.11.9\n
Riot API\n
SQLite\n
Libraries: Pandas, Matplotlib, Seaborn

# 実行順番
1．get_match_data.ipynb\n
2．anaryze.ipynb

# 注意点
get_match_dataではRiot APiを用いてデータを取得しますが、2分で100件のリクエストというAPIの制限があります。そのため、目安として2500試合取得するのに1時間程度かかるため十分な時間を確保してください。

# 補足
今回champion_information.csvはコード内で使用していません。
