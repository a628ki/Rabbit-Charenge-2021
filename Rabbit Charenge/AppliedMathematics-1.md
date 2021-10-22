# ラビットチャレンジ　レポート　応用数学

## 第一章 線形代数

1. スカラーとベクトルの違い
   - スカラー
      - いわゆる普通の数
      - 四則演算が可能
      - ベクトルに対する係数になれる
   - ベクトル
     - 「大きさ」と「向き」を持つ
     - 矢印で図示される
     - スカラーのセットで表示される

2. 行列

   - 行列とは

     - スカラーを表にしたもの
     - ベクトルを並べたもの

   - 計算方法
     - 行列とベクトルの積

      > 例題
      > <img src="https://latex.codecogs.com/gif.latex?\left(\begin{array}{cc}&space;6&space;&&space;4&space;\\&space;3&space;&&space;5&space;\end{array}\right)&space;\quad&space;\left(\begin{array}{c}&space;1&space;\\&space;2&space;\\&space;\end{array}\right)&space;\quad&space;=\left(\begin{array}{c}&space;14&space;\\&space;13&space;\end{array}\right)&space;\quad" />
      - 行列の積
      > 方法
      > <img src="https://latex.codecogs.com/gif.latex?\left(\begin{array}{ccc}&space;a_{11}&space;&&space;a_{12}&space;&&space;a_{13}&space;\\&space;a_{21}&space;&&space;a_{22}&space;&&space;a_{23}&space;\\&space;a_{31}&space;&&space;a_{32}&space;&&space;a_{33}&space;\end{array}\right)&space;\quad&space;\left(\begin{array}{ccc}&space;b_{11}&space;&&space;b_{12}&space;&&space;b_{13}&space;\\&space;b_{21}&space;&&space;b_{22}&space;&&space;b_{23}&space;\\&space;b_{31}&space;&&space;b_{32}&space;&&space;b_{33}&space;\end{array}\right)&space;\quad&space;=\left(\begin{array}{ccc}&space;a_{11}b_{11}&space;&plus;&space;a_{12}b_{21}&space;&plus;a_{13}b_{31}&space;&&space;a_{11}b_{12}&space;&plus;&space;a_{12}b_{22}&space;&plus;a_{13}b_{32}&space;&&space;a_{11}b_{13}&space;&plus;&space;a_{12}b_{23}&space;&plus;a_{13}b_{33}&space;\\&space;a_{21}b_{11}&space;&plus;&space;a_{22}b_{21}&space;&plus;a_{23}b_{31}&space;&&space;a_{21}b_{12}&space;&plus;&space;a_{22}b_{22}&space;&plus;a_{23}b_{32}&space;&&space;a_{21}b_{13}&space;&plus;&space;a_{22}b_{23}&space;&plus;a_{23}b_{33}&space;\\&space;a_{31}b_{11}&space;&plus;&space;a_{32}b_{21}&space;&plus;a_{33}b_{31}&space;&&space;a_{31}b_{12}&space;&plus;&space;a_{32}b_{22}&space;&plus;a_{33}b_{32}&space;&&space;a_{31}b_{13}&space;&plus;&space;a_{32}b_{23}&space;&plus;a_{33}b_{33}&space;\end{array}\right)&space;\quad" />

      > 例題
      ><img src="https://latex.codecogs.com/gif.latex?\left(\begin{array}{cc}&space;2&space;&&space;1&space;\\&space;4&space;&&space;1&space;\end{array}\right)&space;\quad&space;\left(\begin{array}{cc}&space;1&space;&&space;3&space;\\&space;3&space;&&space;1&space;\end{array}\right)&space;\quad&space;=\left(\begin{array}{cc}&space;2*1&plus;1*3&space;&&space;2*3&space;&plus;&space;1*1&space;\\&space;4*1&space;&plus;&space;1*3&space;&&space;4*3&space;&plus;&space;1*1&space;\end{array}\right)&space;\quad&space;=\left(\begin{array}{cc}&space;5&space;&&space;7&space;\\&space;7&space;&&space;13&space;\end&space;{array}&space;\right)&space;\quad" />


3. 単位行列と逆行列
     - 単位行列

       - かけてもかけられても相手が変化しない行列
        > <img src="https://latex.codecogs.com/gif.latex?\boldsymbol{I}&space;=&space;\left(\begin{array}{ccc}&space;1&space;&&space;&&space;\\&space;&&space;1&space;&&space;\\&space;&&space;&&space;...&space;\end{array}\right)&space;\quad" /> 
        
        > 例
        ><img src="https://latex.codecogs.com/gif.latex?\left(\begin{array}{cc}&space;1&space;&&space;0&space;\\&space;0&space;&&space;1&space;\end{array}\right)&space;\quad&space;\left(\begin{array}{cc}&space;2&space;&&space;3&space;\\&space;1&space;&&space;9&space;\end{array}\right)&space;\quad&space;=&space;\left(\begin{array}{cc}&space;2&space;&&space;3&space;\\&space;1&space;&&space;9&space;\end{array}\right)&space;\quad"/>

     - 逆行列
       - 任意の行列Aについて<img src="https://latex.codecogs.com/gif.latex?AY=YA=I"/>となるような行列Yを逆行列と言い、<img src="https://latex.codecogs.com/gif.latex?A^{-1}"/>で表す。
       - 求め方
(1) 掃き出し法
           行基本変形を行い階段行列を作成することで求める。
           > 例)
           ><img src="https://latex.codecogs.com/gif.latex?\left(\begin{array}{cc}&space;1&space;&&space;4&space;\\&space;2&space;&&space;6&space;\end{array}\right)&space;\quad&space;\left(\begin{array}{cc}&space;x_{1}&space;\\&space;x_{2}&space;\end{array}\right)&space;\quad&space;=&space;\left(\begin{array}{cc}&space;7&space;\\&space;10&space;\end{array}\right)&space;\quad"/>
            >という式を下記のように変形する
            <img src="https://latex.codecogs.com/gif.latex?\left(\begin{array}{cc}&space;1&space;&&space;4&space;\\&space;2&space;&&space;6&space;\end{array}\right)&space;\quad&space;\left(\begin{array}{cc}&space;x_{1}&space;\\&space;x_{2}&space;\end{array}\right)&space;\quad&space;=&space;\left(\begin{array}{cc}&space;1&space;&&space;0&space;\\&space;0&space;&&space;1&space;\end{array}\right)&space;\quad&space;\left(\begin{array}{cc}&space;7&space;\\&space;10&space;\end{array}\right)&space;\quad"/>
            
            > 左右の係数に同じ行基本変形を行うと下記の通り計算できる。
            ><img src="https://latex.codecogs.com/gif.latex?\left(\begin{array}{cc|cc}&space;1&space;&&space;4&space;&&space;1&space;&&space;0&space;\\&space;2&space;&&space;6&space;&&space;0&space;&&space;1&space;\end{array}\right)&space;\quad"/>

            >→2行目を1/2倍
        <img src="https://latex.codecogs.com/gif.latex?\left(\begin{array}{cc|cc}&space;1&space;&&space;4&space;&&space;1&space;&&space;0&space;\\1&space;&&space;3&space;&&space;0&space;&&space;1/2&space;\end{array}\right)&space;\quad"/>
        
            >→ 1行目に2行目の-1倍を加える
        <img src="https://latex.codecogs.com/gif.latex?\left(\begin{array}{cc|cc}&space;0&space;&&space;1&space;&&space;1&space;&&space;-1/2&space;\\&space;1&space;&&space;3&space;&&space;0&space;&&space;1/2&space;\end{array}\right)&space;\quad"/>
        
            > → 2行目に1行目の-3倍を加える
        <img src="https://latex.codecogs.com/gif.latex?\left(\begin{array}{cc|cc}&space;0&space;&&space;1&space;&1&space;&&space;-1/2&space;\\&space;1&space;&&space;0&space;&&space;-3&space;&&space;2&space;\end{array}\right)&space;\quad"/>
       
            >→1行目と2行目を入れ替える
        <img src="https://latex.codecogs.com/gif.latex?\left(\begin{array}{cc|cc}&space;1&space;&&space;0&space;&-3&space;&&space;2&space;\\&space;0&space;&&space;1&&space;-1/2&space;&&space;1&space;\end{array}\right)&space;\quad"/>
        
            > 逆行列は
        <img src="https://latex.codecogs.com/gif.latex?\left(\begin{array}{cc}&space;-3&space;&&space;2&space;\\&space;-1/2&space;&&space;1&space;\end{array}\right)&space;\quad"/>

            (2) 逆行列の公式

            > <img src="https://latex.codecogs.com/gif.latex?\boldsymbol{A}&space;=&space;\left(\begin{array}{cc}&space;a&space;&&space;b\\&space;c&space;&&space;d&space;\end{array}\right)&space;\quad"/>
            > とする

            > - ad-bc ≠ 0のとき
            ><img src="https://latex.codecogs.com/gif.latex?\boldsymbol{A}^{-1}&space;=&space;\frac{1}{ad-bc}\left(\begin{array}{cc}&space;d&space;&&space;-b\\&space;-c&space;&&space;a&space;\end{array}\right)&space;\quad"/>
            > - ad-bc = 0のとき
            > 逆行列は存在しない。

4. 固有値と固有ベクトル

   - 固有値、固有ベクトル
    ある行列Aについて以下の式が成り立つような特殊なベクトルxと右辺の係数λがある。
    <img src="https://latex.codecogs.com/gif.latex?Ax=\lambda&space;x"/>
    行列Aとその特殊なベクトルxの積はただのスカラーの数λとその特殊なベクトルxの値と同じになる。
    この特殊なベクトルxとその係数λをそれぞれ行列$A$に対する固有ベクトル、固有値という。
  
   - 固有値、固有ベクトルの求め方
     - 求め方
     >  <img src="https://latex.codecogs.com/gif.latex?Ax=\lambda&space;x"/> より
     > <img src="https://latex.codecogs.com/gif.latex?(A-\lambda&space;I)x=0"/>　…①
     > x≠0　であるので①式に値を代入する。
     - 例題
     ><img src="https://latex.codecogs.com/gif.latex?\left(\begin{array}{ccc}&space;3&space;&&space;2&space;&&space;0&space;\\&space;0&space;&&space;2&space;&&space;0&space;\\&space;0&space;&&space;0&space;&&space;1&space;\end{array}\right)&space;\quad"/> 
     > の固有値、固有ベクトルを求めよ。
     - 回答
     > <img src="https://latex.codecogs.com/gif.latex?Ax=\lambda&space;x"/> より
     > <img src="https://latex.codecogs.com/gif.latex?(A-\lambda&space;I)x=0"/>
     > <img src="https://latex.codecogs.com/gif.latex?x\neq&space;0"/>　であるので
     ><img src="https://latex.codecogs.com/gif.latex?|A-\lambda&space;I|=0"/>
     ><img src="https://latex.codecogs.com/gif.latex?\left|\begin{array}{ccc}&space;3-&space;\lambda&space;\&space;&&space;2&space;&&space;0&space;\\&space;0&space;&&space;2-\lambda&space;&&space;0&space;\\&space;0&space;&&space;0&space;&&space;1-\lambda&space;\end{array}\right|&space;=&space;0\quad"/>
     ><img src="https://latex.codecogs.com/gif.latex?(3-\lambda&space;)(2-\lambda&space;)(1-\lambda&space;)=0"/> よって
     >λ=3,2,1 
     >λ=3の時
     ><img src="https://latex.codecogs.com/gif.latex?\left(\begin{array}{ccc}&space;3&space;&&space;2&space;&&space;0&space;\\&space;0&space;&&space;2&space;&&space;0&space;\\&space;0&space;&&space;0&space;&&space;1&space;\end{array}\right)\quad&space;\left(\begin{array}{cc}&space;x_{1}&space;\\&space;x_{2}&space;\\&space;x_{3}&space;\end{array}\right)&space;\quad&space;=&space;3&space;\left(\begin{array}{cc}&space;x_{1}&space;\\&space;x_{2}&space;\\&space;x_{3}&space;\end{array}\right)&space;\quad"/>
     
     ><img src="https://latex.codecogs.com/gif.latex?x_{1}&space;=&space;t"/> とすると
     ><img src="https://latex.codecogs.com/gif.latex?x_{2}&space;=&space;0">
     ><img src="https://latex.codecogs.com/gif.latex?x_{3}&space;=&space;0">
     >よってλ=3のとき
     <img src="https://latex.codecogs.com/gif.latex?x=\left(\begin{array}{cc}&space;1&space;\\&space;0&space;\\&space;0&space;\end{array}\right)&space;\quad"/>
        の定数倍となる。
     >λ=2の時、λ=1の時も同様にして解くと
     >λ=2のとき
     <img src="https://latex.codecogs.com/gif.latex?x=\left(\begin{array}{cc}&space;2&space;\\&space;-1&space;\\&space;0&space;\end{array}\right)&space;\quad"/>
        の定数倍、
     >λ=1のとき
     <img src="https://latex.codecogs.com/gif.latex?x=\left(\begin{array}{cc}&space;0&space;\\&space;0&space;\\&space;1&space;\end{array}\right)&space;\quad"/>
        の定数倍となる。

5. 固有値分解

   - 固有値分解とは
     ある実数を正方形にならべて作られた行列Aが固有値 <img src="https://latex.codecogs.com/gif.latex?\lambda&space;_{1},&space;\lambda&space;_{2},&space;..."/>と固有ベクトル<img src="https://latex.codecogs.com/gif.latex?v&space;_{1},&space;v&space;_{2},&space;..."/>を持ったとする。この固有値を対角線上に並べ、それ以外の成分を0とした行列
     <img src="https://latex.codecogs.com/gif.latex?\Lambda &space;=&space;\left(\begin{array}{ccc}&space;\lambda&space;_{1}&space;&&space;&&space;\\&space;&&space;\lambda&space;_{2}&space;&&space;\\&space;&&space;&&space;...&space;\end{array}\right)&space;\quad"/>
    とそれに対する固有ベクトルを並べた行列
    <img src="https://latex.codecogs.com/gif.latex?V&space;=&space;\left(\begin{array}{ccc}&space;v_{1}&space;&&space;v_{2}&space;&&space;...&space;\end{array}\right)&space;\quad"/>
    を用意したときそれらは
    <img src="https://latex.codecogs.com/gif.latex?AV&space;=&space;V\Lambda"/>
    と関係づけられる。
    従って
    <img src="https://latex.codecogs.com/gif.latex?A&space;=&space;V\Lambda&space;V^{-1}"/>
    と変形できる。このように正方形の行列を上述のような3つの行列の式に変換することを固有値分解という。この変換によって行列の累乗の計算が容易になるなどの利点がある。

6. 特異値分解

   - 特異値分解
    正方行列でない行列に対し、固有値分解と似たことを行う。
   <img src="https://latex.codecogs.com/gif.latex?Mv&space;=&space;\sigma&space;u"/>
    <img src="https://latex.codecogs.com/gif.latex?M^{T}u&space;=&space;\sigma&space;v"/>
    このような特殊な単位ベクトルがある場合、特異値分解が可能。
    <img src="https://latex.codecogs.com/gif.latex?M&space;=&space;USV^{-1}"/>

   - 特異値分解の求め方
    <img src="https://latex.codecogs.com/gif.latex?MV&space;=&space;US"/>
    <img src="https://latex.codecogs.com/gif.latex?M^{T}U&space;=&space;VS^{T}"/>
    <img src="https://latex.codecogs.com/gif.latex?M&space;=&space;USV^{-1}"/>
    <img src="https://latex.codecogs.com/gif.latex?M^{T}&space;=&space;VS^{T}U^{-1}"/>
    の積は
    <img src="https://latex.codecogs.com/gif.latex?MM^{T}&space;=&space;USV^{-1}VS^{T}U^{-1}&space;=&space;USS^{T}U^{-1}"/>
    つまり<img src = "https://latex.codecogs.com/gif.latex?MM^{T}"/>を固有値分解すれば、その左特異ベクトル(単位ベクトルから作成する)と特異値の2条が求められることがわかる。
