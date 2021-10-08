# ROHAN4600：大規模日本語テキストコーパス（仮）

## ROHAN4600とは
コーパス文の課題生成システムが提示した条件を満たす文章を人間が作ることで，ある程度クオリティが統一した文章を作ろうという試みです．システムは常用漢字と読みを全て含み，出現頻度の低いモーラもカバーするように各文章の条件を設定します．その条件を満足するように作文を続けていけば，いずれ良いコーパスが出来上がるはずです．

## 文章のフォーマット
- 基本的には最初の100文章を見ればイメージは掴めると思います．
- 漢字は半角括弧で読みを入れてください（例えば「勝(か)つ」）．
- 作成した文章後，半角「,」を入れて全角カタカナで文章を入れてください．
- 1文章（4600_xxxx）の中で「。」を使うのは避けましょう．2文章とカウントされてしまいます．
- カタカナ部分は「を」は「お」，「〇〇へ」は「〇〇え」，「〇〇は」は「〇〇わ」と読みに忠実に入力してください．
- 文章は一度朗読し，読みやすいかを評価してから確定しましょう．
- 同じ名詞を多用するのは控えましょう．
- ポリコレには配慮し炎上を避ける文章にしよう．
- 文体のバリエーションを増やすためセリフ的なものを入れても構いません．「だ・である」については平叙文以外であれば砕けた表現でも良いことにします．
- 文章の時制は自由です．現在形・過去形などバリエーションを増やしましょう．
- 「ヌィ」などは現在のところ対応する音素が無いので，「ヌイ」にするか使わないかの選択をお願いします（新たな音素を提案するのは今のところやる予定がありません）．一般的な日本語のモーラと条件にしている特殊なモーラのみが対象です．

## 条件の修正
文章のモーラ数はばらつかせたほうが良いという指摘があったため，中盤から意図的にモーラ数の条件を長文・短文になるよう修正します．現状ご協力頂いている皆様分に影響はせず，作者の分で調整します．
- 1601～1800: 23モーラ以下で平均18モーラ．23モーラ以下
- 1801～2000: 33モーラ以上で平均38モーラ．33モーラ以上
- 2001～2200: 23モーラ以下で平均18モーラ．23モーラ以下
- 2201～2400: 33モーラ以上で平均38モーラ．33モーラ以上
- 2401～2600: 23モーラ以下で平均18モーラ．23モーラ以下（「セリフ」的な表現）
- 2601～2800: 33モーラ以上で平均38モーラ．33モーラ以上（「セリフ」的な表現）
- 2801～3000: 23モーラ以下で平均18モーラ．23モーラ以下（「セリフ」的な表現）
- 3001～3200: 33モーラ以上で平均38モーラ．33モーラ以上（「セリフ」的な表現）

「セリフ的」については，目安であり厳密に切り分けない（最後にシャッフルする予定）

## 200文章毎のコンセプト（似たような文章とならないようにする工夫）．リポジトリ管理者用で当分はモーラ出現率を優先する．
以下の条件を入れるとエントロピーが下がるので，どこまで入れるか，エントロピー最大化を意識するかを考えています．
色々考えた結果，モーラカバー率を優先することにしたので，コンセプト変更．
- 0001～0800: 100文章単位でモーラ出現頻度をチェックし，不足モーラを優先的に入れながら作文
- 0801～1600: 上記と同様だが，「セリフ」的な表現を中心に構成
- 1601～2400: 0001～0800をベースにモーラ数の条件を変更（短文，長文リストのため18以下と33以上のみで構成）
- 2401～3200: 1601～2400と同様だが，「セリフ」的な表現を中心に構成
- 3201～3600: そこまでの完成度を見て不足分を補う調整項

数詞について少しずつ入れます．以下の〇に1～10まで入れたものが達成済み．
- 〇月，〇時間，〇年，〇匹，〇個，〇秒は達成済み．
- 〇粒は現在調整中
- 「〇つ」は常用漢字の範囲なので自動的に入るはず．

以下の内容（過去のもののためナンバリングはそのまま残しています）をベースに再検討するが，モーラ出現度が確実に偏るので，随時調整．
- 1401～1600: 数詞１（〇時間，〇個，〇枚，〇本，〇冊を一～十まで＋何△（例えば「何時間」））
- 1601～1800: 数詞２（〇台，〇杯，〇人，〇匹，〇階を一～十まで＋何△）
- 1801～2000: 数詞３（〇回，〇円，〇歳，〇番，〇拍を一～十まで＋何△）
- 2001～2200: 数詞４（〇票，〇発，〇品，〇粒，〇句を一～十まで＋何△）
- 2201～2400: 数詞５（〇位，〇席，〇秒，〇分，〇時を一～十まで＋何△）
- 2401～2600: 数詞６（〇つを一～九まで＋「とお」と「いくつ」）
- 2601～2800: 古風な単語・表現
- 2801～3000: 動物等の名前（カタカナをたくさん使う）
- 3001～3200: 常用以外の漢字と読みを中心に

## 予約
- 3601～3800: nakak様
- 3801～4000: 女郎蜘蛛魅冴（じょろうぐも　みさえ）様
- 4001～4200: 協力者に感謝です（了解が得られたら協力者としてのお名前をクレジットさせて頂きます）
- 4201～4400: 協力者に感謝です（了解が得られたら協力者としてのお名前をクレジットさせて頂きます）
- 4401～4600: 協力者に感謝です（了解が得られたら協力者としてのお名前をクレジットさせて頂きます）

## 各サブセットの情報（作者・平均モーラ数・拡張エントロピー）
最終的には0001～0800，0801～1600，1601～2400，2401～3200の単位で，条件を崩さないようにシャッフルかけるので，～3200までは目安です．ついでに，過去の文章も気分で入れ替えやってますので，完成までは流動的なものとなります．
- 0001～0200: 森勢，28.07モーラ/文，22.31 bit
- 0201～0400: 森勢，28.01モーラ/文，22.29 bit
- 0401～0600: 森勢，27.98モーラ/文，22.35 bit
- 0601～0800: 森勢，28.02モーラ/文，22.46 bit
- 0801～1000: 森勢，28.00モーラ/文，22.35 bit
- 1001～1200: 森勢，27.94モーラ/文，22.39 bit
- 1201～1400: 森勢，27.96モーラ/文，22.53 bit
- 1401～1600: 森勢，27.93モーラ/文，22.62 bit
- 1601～1800: 森勢，17.95モーラ/文，22.53 bit
- 1801～2000: 森勢，37.88モーラ/文，22.47 bit
- 2001～2200: 森勢，17.93モーラ/文，22.33 bit
- 2201～2400: 森勢，37.84モーラ/文，22.41 bit
- 2401～2600: 森勢，17.93モーラ/文，22.44 bit
- 3601～3800: nakak様，28.05モーラ/文，22.60 bit
- 3801～4000: 女郎蜘蛛魅冴様，27.92モーラ/文，21.95 bit

## 作文の妥協
- 「くぅ」「ぐぅ」「でぇ」「てゃ」「てょ」「でゃ」「でょ」は特に難しいと思うので，単語として入れることは妥協しても構いませんが，何らかの形で入れるように心がけてください．
- 日本語に該当する単語がないものは上記以外でもあるので単語としては諦めます．というか日本語だと多分無理です．
- 「しぃ」と「すぃ」は音素に変換すると同じ/si/ですので，「しぃ」を「すぃ」で作っても構いません．

## 文章リストの評価
- これまで作った文章リストから，エントロピーと平均モーラで評価できます．200文章単位で評価し，一定の水準に達していなければ作り直しましょう．
- 足切りラインは，200文章で平均モーラ数が28±0.25，エントロピーが22.25 bit以上としています（ATR503文やITAコーパスよりも上を目指すため）
- エントロピーについては厳しい気がしてきたので，作者が作った文章を見ながら閾値を調整します．

## 質の高いコーパスにするために
- 常用漢字はシステムがカバーしているので，常用漢字以外も積極的に入れる
- 日本語以外のカタカナ名称を入れると，エントロピー的に有利になる

## ライセンス
パブリックドメインです．

## 協力者
クレジットさせて頂くので，パブリックドメインという条件で良ければ名乗り出て頂けたら嬉しいなぁ（希望的観測）．200文章（「です・ます」100文と「だ・である」100文のセット）作って頂いたら，平均モーラとエントロピーを評価してランキングを作ろうと思っています．
