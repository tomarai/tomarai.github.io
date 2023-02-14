---
layout: post
title: 活躍しそうな打者を探そう (2023年)
author: tomarai
date: 2023-02-18
tags: [Baseball]
---

本記事では以下の 2 点に着目して今年活躍しそうな野手を探します

* Direction: pull の exit vel. (引っ張った打球の速度)
* Swing/Take の Chase の Run Value (ボールゾーンの球の成績)

今回，この 2 点に着目した理由はマインドセットによって成績が改善できる可能性が高いと考えたからです

* pull の exit vel. を上げるのは身体，技術的成長が必要
* pull の exit vel. が速い選手が pull の割合を上げるのは戦略依存 ([Alex Bregman’s Triumphant Non-Adjustment](https://blogs.fangraphs.com/alex-bregmans-triumphant-non-adjustment/))
* Swing/Take において Chase の Run Value の低下はボール球の空振りが引き起こす
* Swing% を下げることで Chase の Run Value を上げる例が指摘されている ([Mariners Hold Onto Their Utility Knife, Extend Dylan Moore](https://blogs.fangraphs.com/mariners-hold-onto-their-utility-knife-extend-dylan-moore/))

これらの情報から pull の exit vel. が上位のプレイヤーが pull の割合をあげて
Swing% を減らすことで成績を向上させることを試みるのではないかと推測しての予想です

データは [baseballsavant](https://baseballsavant.mlb.com) と
[fangraphs](https://fangraphs.com) から取得しています

## xwOBA と pull の exit vel. 及び chase の run value の関係

昨年 PA 100 以上を記録した選手について

* 昨年の xwOBA
* 昨年の chase の run value
* 過去 3 年間分の pull の exit vel.

を集計しました

下の図は xwOBA と pull の exit vel. の散布図です．
相関係数は 0.57 となりました

pull の exit vel. が全体の exit vel. を底上げすることを考えればこのデータは直感と齟齬がないと思います


![](/assets/img/figures/xwoba_pull_exit_vel.png)

次に xwOBA と chase の run value の散布図です．
相関係数は 0.53 です

pull の exit vel. と比較すると，chase の run value の向上が xwOBA を底上げするというよりは低い chase の run value が xwOBA と低下させる傾向がありそうです

![](/assets/img/figures/xwoba_chase.png)

これらのデータを踏まえて，今回は

* pull の exit vel. が上位 20 percentile
  - pull% を上げるという主体的な行動で向上の可能性あり
* Chase の run value が下位 20 percentile 
  - Swing% を下げるという主体的な行動で向上の可能性あり

の2つを満たす選手に着目します


### pull の exit vel. が 20 percentile 以上かつ chase の run value が下位 20 percentile のプレイヤー

pitch percent は全体のイベント (投球) の中で打球が引っ張り方向に飛んだ割合です <br>
以下の 9 人のプレイヤーがリストアップされました <br>
トッププロスペクトから FA の選手までさまざまです

Name | age | Swing % | xwOBA | exit vel. | pitch percent | chase |
--- | --- | --- | --- | --- | --- | --- |
*Oneil Cruz* | 24 | 40.6% | 0.304 | 96.1 | 5.9 | 4
*Jose Miranda* | 24 | 51.5% | 0.317 | 92.0 | 8.2 | 4
*Matt Vierling* | 25 | 44.2% | 0.327 | 91.9 | 5.4 | 4
*Jake Burger* | 26 | 54.0% | 0.318 | 95.4 | 6.3 | 1
*Trevor Larnach* | 26 | 41.4% | 0.322 | 93.5 | 5.3 | 3
*Eric Haase* | 29 | 51.4% | 0.302 | 94.0 | 6.6 | 0
*Teoscar Hernández* | 30 | 48.9% | 0.351 | 94.2 | 6.5 | 4
Tyler Naquin | 31 | 57.7% | 0.317 | 92.2 | 6.6 | 3
Kyle Garlick | 31 | 48.7% | 0.305 | 91.9 | 7.7 | 2

これ以上 pull の割合をあげるのが難しそうな Miranda や
既に Swing% が低い Oneil Cruz がどう成長していくか楽しみです

pull の割合を上げられれば全体の平均 exit vel. を上げられそうな Vierling や
Swing% の改善の余地がある Burger は今年は期待できるのではないでしょうか

Teoscar Hernández は Dylan Moore のアプローチを変化させた Mariners でどういった変化が見込めるかに注目しています

### 各指標 Top 5 のプレイヤー

Chase の run value, pull の exit vel. の　Top 5 を確認します <br>
これによって，好打者との関連を感覚的に把握することを目的とします

#### Chase の run value Top 5

Name | Swing % | xwOBA | exit vel. | pitch percent | chase |
--- | --- | --- | --- | --- | --- |
Juan Soto | 35.3% | 0.401 | 92.3 | 4.8 | 35
Alex Bregman | 40.3% | 0.35 | 90.8 | 8.6 | 32
Brandon Nimmo | 43.7% | 0.342 | 90.7 | 5.0 | 30
Kyle Schwarber | 40.3% | 0.375 | 94.5 | 5.7 | 29
Steven Kwan | 37.7% | 0.312 | 86.9 | 5.4 | 28

Bregman は先の記事で指摘されている通り，pull% が高く chase の run value が高いです <br>
打席でのアプローチによって成績を向上させている代表的なプレイヤーと言えるでしょう <br>
Kwan も iso が控えめながらも高い BB% を記録する原動力になっていることがわかります

#### pull の exit vel. Top 5

Name | xwOBA | exit vel. | pitch percent | chase |
--- | --- | --- | --- | --- |
Aaron Judge | 0.463 | 97.3 | 6.0 | 25
Giancarlo Stanton | 0.351 | 96.7 | 5.0 | 10
Yordan Alvarez | 0.462 | 96.6 | 6.1 | 17
Oneil Cruz | 0.304 | 96.1 | 5.9 | 4
Vladimir Guerrero Jr. | 0.348 | 95.9 | 7.5 | 14

こちらもスタープレイヤーが並びます <br>
ここにも Oneil Cruz が入ってくるのはさすがトッププロスペクトと言うほかないですね

## Conclusion

今回は打席でのマインドセットによって xwOBA を向上できると期待される数値に着目して，
今後活躍が期待される選手をリストアップしました

Oneil Cruz のようなトッププロスペクトも今後期待できるような要素が残っていることが明らかになり，
これらの選手がどう打席でのアプローチを変えていくかにも注目です

