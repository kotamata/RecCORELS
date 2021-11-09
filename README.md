# RecCORELS

### /data : 実験に使用したデータが格納
- compas_train/test.csv : https://github.com/corels/corels の訓練テストデータを使用
- compas_train.out : https://github.com/corels/corels　のタームを使用
- compas_train/test_preprocessed.csv : compas_train/test.csv に preprocess.ipynb を用いて前処理(one-hot encoding)を行なった訓練/テストデータ
- term_over1.pkl : compas_train.out に preprocess.ipynb を用いて前処理(条件を満たすデータ全体のうちラベルの割合が 50% 以上になるタームのみを抽出)を行なったターム
- term_list.pkl : term_over1.pkl に格納されているタームを python のリスト形式で保存したファイル

/code : 実験に使用したコードが格納
- RecCORELS.ipynb : CORELS を拡張してルールリストを列挙するコード
- result.ipynb : Discrepancy と Ambiguity を計算するのに使用したコード
- corels.pkl : RecCORELS.ipynb を用いて列挙したモデルを格納したファイル
