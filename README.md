# FOODE
 NNで一階微分方程式を解く.

 y_prime = f(x,y)の形の微分方程式について、y=g(x)をNNでモデル化し以下の損失関数を用いて学習する。
 初期条件はy0 =g(x0)の形式で与える。

 loss = (f(x,model(x)) - ((model(x)の微分値)) ^ 2 + (定数) * (y0 - model(x0)) ^ 2

 web上でnotebookを見る場合は、no_output.ipynbの方じゃないと容量の問題なのか開けない。

 # results

 - 初期値を用いたバイアスのモデルへの導入を行ったバージョン。比較的安定かつ、高速に解へ収束していっている。 
![result1](https://github.com/ryoryon66/FOODE/assets/46624038/72507b37-a727-41f7-b003-0c1affcc26d2)

- 初期値をモデルに組み込んでいないバージョンの結果。上のものよりも遅いかつ解にうまくフィットできていない。
![result2](https://github.com/ryoryon66/FOODE/assets/46624038/043550d0-0a0c-45af-be8b-616d7c5c61b2)

利用した計算資源は自宅のRTX-3060で2分程度で上のアニメーションを作成できる。
