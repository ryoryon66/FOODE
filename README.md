# FOODE
 NNで一階微分方程式を解く

 y_prime = f(x,y)の形の微分方程式について、y=g(x)をNNでモデル化し以下の損失関数を用いて学習する。
 初期条件はy0 =g(x0)の形式で与える。

 loss = (f(x,model(x)) - ((model(x)の微分値)) ^ 2 + (定数) * (y0 - model(x0)) ^ 2
