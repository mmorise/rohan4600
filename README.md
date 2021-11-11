# ROHAN4600：テキスト音声合成に向けた大規模日本語コーパス

## ROHAN4600とは
コーパス文の課題生成システムが提示した条件を満たす文章を人間が作成することで，常用漢字と読みを全て含み，出現頻度の低いモーラもカバーした4600文章からなる日本語のテキストコーパスです．4600文は，後述する22のサブセットから構成されており，サブセット単位で全モーラを最低2回含みます．なお，ここでの全モーラとは，Sinsyの日本語でサポートするモーラと定義します．

## サブセットの構成
- ENDSIVILLE400：エントロピー最大化を目的とした400文のサブセット
- MIDDLE1600: 23～33モーラの範囲の文章で構成される200文×8のサブセット
- SHORT800: 23モーラ以下の文章で構成される200文×4のサブセット
- LONG800: 33モーラ以上の文章で構成される200文×4のサブセット
- GUEST1000: 外部協力者により生成された200文×5のサブセット．GUEST1000_1～4はMIDDLE1600と同様．GUEST1000_5のみモーラ数制限無し．

## 1サブセットの目安
- ENDSIVILLE400を除き，前半100文をですます調を中心に，後半100文をだ・である調を中心に作文している．台詞的なものなどは判断が難しいのであくまでも目安である．
- 前半・後半それぞれ疑問文が5文章ずつ含まれる．
- 文語的・口語的表現については特に制約は設けていない．

## 全サブセットと平均モーラ数・拡張エントロピーのデータ
- 0001～0400: ENDSIVILLE400：平均27.79モーラ，22.96 bit
- 0401～0600: MIDDLE1600_1：平均27.98モーラ，22.47 bit
- 0601～0800: MIDDLE1600_2：平均27.95モーラ，22.51 bit
- 0801～1000: MIDDLE1600_3：平均27.76モーラ，22.47 bit
- 1001～1200: MIDDLE1600_4：平均28.02モーラ，22.47 bit
- 1201～1400: MIDDLE1600_5：平均28.18モーラ，22.49 bit
- 1401～1600: MIDDLE1600_6：平均27.90モーラ，22.48 bit
- 1601～1800: MIDDLE1600_7：平均28.05モーラ，22.51 bit
- 1801～2000: MIDDLE1600_8：平均28.10モーラ，22.49 bit
- 2001～2200: SHORT800_1：平均17.83モーラ，22.45 bit
- 2201～2400: SHORT800_2：平均17.87モーラ，22.46 bit
- 2401～2600: SHORT800_3：平均18.01モーラ，22.43 bit
- 2601～2800: SHORT800_4：平均18.06モーラ，22.43 bit
- 2801～3000: LONG800_1：平均37.83モーラ，22.41 bit
- 3001～3200: LONG800_2：平均37.95モーラ，22.40 bit
- 3201～3400: LONG800_3：平均37.85モーラ，22.41 bit
- 3401～3600: LONG800_4：平均37.91モーラ，22.41 bit
- 3601～3800: GUEST1000_1：平均28.05モーラ，22.60 bit
- 3801～4000: GUEST1000_2：平均27.90モーラ，21.95 bit
- 4001～4200: GUEST1000_3：平均27.90モーラ，21.94 bit
- 4201～4400: GUEST1000_4：平均27.82モーラ，21.85 bit
- 4401～4600: GUEST1000_5：平均27.41モーラ，21.86 bit

4600文全てで計算すると，平均モーラ数が27.91，拡張エントロピーが22.83 bitです．

## 補足情報
- 数詞は「〇月，〇時間，〇年，〇匹，〇個，〇秒」について1～10まで含めている．

## GUEST1000の協力者様
- 3601～3800: nakak様
- 3801～4000: 女郎蜘蛛魅冴（じょろうぐも　みさえ）様
- 4001～4200: にゃーちゃん様
- 4201～4400: きつね様
- 4401～4600: 匿名希望様

## ライセンスはパブリックドメインです．
[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png "CC0")](http://creativecommons.org/publicdomain/zero/1.0/deed.ja)
