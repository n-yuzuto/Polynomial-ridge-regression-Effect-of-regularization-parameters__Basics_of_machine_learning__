# Polynomial-ridge-regression-Effect-of-regularization-parameters
degree=30の多項式特徴量による正則化多項式回帰において、正則化パラメータlambdaを1e-30から100まで変化させ、ambda、訓練誤差、テスト誤差、そのプロットを出力しました。

***
正則化の利用目的:  
正則化は、テスト誤差を制御するために利用します。  
複雑度の高いモデルについて訓練誤差は低くテスト誤差は高い時、過学習が起きていると考えられます。
訓練誤差は直接最小化できますが、テスト誤差は直接最小化できません。学習時にテスト事例を使ったら、その事例はテスト誤差評価には使うことができないからです。  
その代わりに正則化を使います。

***
考察：  
正則化パラメータを変化させ、グラフを見ることで次の関係が考えられました。  
lamuda = 0:  
  - 訓練誤差: 小さい.  
  - モデルの複雑さ: 複雑になりやすい.  
  - 汎化誤差: 大きい.  

lamuda = α(中間的):  
  - 訓練誤差: ほどほど.  
  - モデルの複雑さ: ほどほど.  
  - 汎化誤差: ほどほど.  

lamuda = ∞:  
  - 訓練誤差: 最小化されない.  
  - モデルの複雑さ: 単純すぎる.  
  - 汎化誤差: 結局大きい.  

***
.ipynbファイルが開かれない時は、こちらのリンクにURLを貼ってご覧になってください。  
[nbviewer](https://nbviewer.jupyter.org/)
