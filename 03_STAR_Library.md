# 03_STAR_Library.md

## Purpose

本文件用于整理 User 的 STAR 故事素材。

STAR 指：

- Situation：当时的背景
- Task：需要完成的任务
- Action：自己采取的行动
- Result：结果、收获、学到的内容

本文件不是最终面试答案，也不是对外提交文档，而是用于积累可复用的职业故事素材。  
后续制作以下内容时，应优先参考本文件：

- 面试回答
- 自己PR
- 派遣先自己紹介
- 客户说明
- 技术发表
- 行为面试回答
- 职业成长总结

---

## Status Labels

本文使用以下标记：

- `[Confirmed]`：User 已明确确认的信息
- `[Inference]`：根据目前信息和常见研修 / 项目情况进行的合理推测
- `[Need Confirmation]`：需要 User 后续确认的信息
- `[Draft]`：暂定表达，后续可调整
- `[Deprecated]`：已不建议继续使用或已过时的信息

---

## How to Use This File

本文件中的 STAR 素材可以根据不同场景进行改写。

同一个经历可以用于多个问题，例如：

- 困難だったこと
- チームで工夫したこと
- 失敗から学んだこと
- 主体的に取り組んだこと
- 技術的に成長したこと
- 問題解決経験
- コミュニケーションで意識したこと

Assistant 在使用本文件时，应注意：

- 不要把 `[Inference]` 当作事实
- 面试用回答必须基于 User 最终确认
- 自己紹介中只取简短版本
- 面试回答中可以展开 Situation / Task / Action / Result
- 不要把研修课题包装成实务经验

---

# 1. STAR Candidate Overview

目前可整理的 STAR 候选素材如下：

| ID | Theme | Related Project | Main Value | Status |
|---|---|---|---|---|
| STAR-01 | Timer 状态管理问题的修正 | Arduino Timer | Bug 修正 / 状态管理 | `[Inference]` |
| STAR-02 | Timer 输入与显示不一致的改善 | Arduino Timer | 问题切分 / 動作確認 | `[Inference]` |
| STAR-03 | SQL エラーの原因切り分け | SQL / データ分析演習 | エラー調査 / 分析力 | `[Inference]` |
| STAR-04 | Git / GitHub の理解とチーム開発 | Git / GitHub | 新しいツールへの適応 | `[Inference]` |
| STAR-05 | 音楽プレーヤー発表経験 | 音楽プレーヤー | 説明力 / チーム開発 | `[Inference]` |
| STAR-06 | グループ課題での役割分担 | 自動販売機 / 音楽プレーヤー / バックソナー | チームワーク | `[Inference]` |
| STAR-07 | バックソナーでのハード / ソフト切り分け | バックソナー | 原因切り分け / 組込み基礎 | `[Inference]` |
| STAR-08 | 研究で予測誤差を考慮した工夫 | 大学院研究 | 分析力 / 改善思考 | `[Confirmed]` + `[Inference]` |
| STAR-09 | 研修を通じた成長ストーリー | 研修全体 | 学習姿勢 / 成長力 | `[Inference]` |

---

# 2. STAR-01 — Timer 状態管理問題の修正

## Related Project

- `[Confirmed]` Arduino Timer / 個人課題

## Use Cases

この STAR は以下の質問に使える：

- 困難だったことは何ですか
- 技術的に苦労した経験はありますか
- 問題をどのように解決しましたか
- 個人で工夫したことはありますか
- 組込み系の課題で学んだことは何ですか

## Situation

- `[Confirmed]` 個人課題としてタイマーを作成した
- `[Inference]` 時間設定、開始、停止、一時停止、リセットなどの機能を実装した
- `[Inference]` 実装中に、入力した時間が意図通り保持されない、または開始・停止の動作が想定通りにならない問題が発生した

## Task

- `[Inference]` タイマーとして自然に使えるように、入力値、表示、開始・停止の状態を正しく管理する必要があった
- `[Inference]` ユーザー操作に応じて、現在の状態を適切に切り替える必要があった

## Action

- `[Inference]` 現在の処理が「設定中」「計時中」「停止中」など、どの状態にあるのかを整理した
- `[Inference]` 入力処理、表示処理、開始 / 停止処理の関係を確認した
- `[Inference]` 問題が発生する操作手順を再現し、どのタイミングで状態が変わっているかを確認した
- `[Inference]` 一度に全体を修正するのではなく、動作を確認しながら少しずつ修正した

## Result

- `[Inference]` タイマーの動作がより自然になった
- `[Inference]` 入力、表示、内部状態を合わせて考える重要性を理解した
- `[Inference]` 組込み系の課題では、状態管理が非常に重要であることを学んだ
- `[Need Confirmation]` 最終的にどの機能が完成したか
- `[Need Confirmation]` 具体的にどの問題を解決したか

## Japanese Answer Draft

> 個人課題でタイマーを作成した際に、開始や停止、時間設定などの状態管理でうまく動かない部分がありました。  
> 最初は表示だけを見ていましたが、入力処理、表示処理、内部状態の関係を整理する必要があると考え、どの操作の時に状態が変わっているかを確認しました。  
> そのうえで、処理を一つずつ確認しながら修正し、想定に近い動作になるように改善しました。  
> この経験から、組込み系の課題では、機能を作るだけでなく、状態の流れを整理して考えることが重要だと学びました。

## Short Version

> 個人課題のタイマーでは、開始・停止や時間設定の状態管理に苦労しました。  
> 入力、表示、内部状態の関係を確認しながら修正し、状態管理の重要性を学びました。

## Risk Notes

- `[Need Confirmation]` 実際に「状態管理」という言葉で説明できるほど理解しているか確認
- `[Need Confirmation]` 面接で聞かれた場合、どの変数や処理を見直したか説明できる準備が必要
- `[Inference]` 自己紹介では短く触れる程度が安全

---

# 3. STAR-02 — Timer 入力と表示不一致の改善

## Related Project

- `[Confirmed]` Arduino Timer / 個人課題

## Use Cases

この STAR は以下の質問に使える：

- 改善した経験はありますか
- 不具合をどのように直しましたか
- 動作確認で意識したことは何ですか
- ユーザー目線で考えた経験はありますか

## Situation

- `[Confirmed]` 個人課題でタイマーに取り組んだ
- `[Inference]` 時間を入力しても、表示がすぐにリセットされる、または開始操作との連動が不自然になる問題があった
- `[Inference]` ユーザー操作としては、時間を入力した時点で設定が完了し、その後すぐ開始できる状態が望ましかった

## Task

- `[Inference]` 入力された時間を正しく保持し、表示にも反映させる必要があった
- `[Inference]` 操作した人が違和感なく使える動作に改善する必要があった

## Action

- `[Inference]` 入力直後の値がどの処理で変更されているか確認した
- `[Inference]` 表示上の値と内部で保持している値を分けて考えた
- `[Inference]` 開始操作をした時に、すでに設定された時間から計時が始まるように処理を見直した
- `[Inference]` 実際に入力操作を繰り返しながら、想定通り表示されるか確認した

## Result

- `[Inference]` 入力した時間が設定値として扱われるようになり、操作の流れが自然になった
- `[Inference]` ユーザー操作を想定しながら実装する重要性を学んだ
- `[Need Confirmation]` 最終的に改善できたか
- `[Need Confirmation]` どの程度自分で原因を特定したか

## Japanese Answer Draft

> タイマーの課題では、入力した時間が表示された後、すぐにリセットされてしまうような動作がありました。  
> 操作する側から見ると、時間を入力した時点で設定が完了し、そのまま開始できる方が自然だと考えました。  
> そこで、入力された値がどこで変更されているかを確認し、表示されている値と内部で保持している値の関係を見直しました。  
> この経験を通じて、単に機能を動かすだけでなく、使う人にとって自然な流れになっているかを考える必要があると学びました。

## Short Version

> タイマー課題では、入力した時間が正しく保持されない問題がありました。  
> 入力値と表示、内部状態の関係を確認しながら修正し、ユーザー操作を意識する重要性を学びました。

## Risk Notes

- `[Need Confirmation]` 実際の問題内容と表現が一致しているか確認
- `[Inference]` 面接で使う場合、「どのように確認したか」を具体化すると強くなる

---

# 4. STAR-03 — SQL エラーの原因切り分け

## Related Project

- `[Confirmed]` SQL / データ分析演習

## Use Cases

この STAR は以下の質問に使える：

- エラー対応経験はありますか
- 困難だったことは何ですか
- 問題の原因をどう調べましたか
- データ分析で学んだことは何ですか

## Situation

- `[Confirmed]` 研修で SQL に取り組んだ
- `[Inference]` SQL 実行時に、構文エラーや期待値と異なる結果が発生した
- `[Inference]` コピーした SQL 内の不可視文字、カラム名、JOIN 条件、GROUP BY などが原因候補だった可能性がある

## Task

- `[Inference]` エラー内容を確認し、原因を特定して正しい結果を得る必要があった
- `[Inference]` グループ課題の場合、結果をメンバーと共有できる状態にする必要があった

## Action

- `[Inference]` エラーメッセージを確認した
- `[Inference]` SQL 文を一度に見るのではなく、部分ごとに分けて確認した
- `[Inference]` カラム名、テーブル名、JOIN 条件、集計条件を確認した
- `[Inference]` 不可視文字や全角 / 半角の違いなど、見た目では分かりにくい原因も確認した
- `[Need Confirmation]` 実際に行った確認手順

## Result

- `[Inference]` エラー原因を特定し、SQL を修正できた
- `[Inference]` エラー対応では、メッセージを読むことと、原因を分けて考えることが重要だと学んだ
- `[Inference]` データ分析では、クエリだけでなく、結果が正しいか確認する姿勢が必要だと学んだ
- `[Need Confirmation]` 実際にどのエラーを解決したか

## Japanese Answer Draft

> SQLの演習では、クエリを実行した際にエラーが出たり、期待した結果にならなかったりすることがありました。  
> その際には、エラーメッセージを確認し、SQL文を一部分ずつ分けて見直しました。  
> また、カラム名やJOIN条件だけでなく、コピーした文の中に見えにくい文字が含まれていないかも確認しました。  
> この経験から、エラーが出た時に慌てて全体を直すのではなく、原因を一つずつ切り分けることが重要だと学びました。

## Short Version

> SQLの演習では、エラーが出た際にSQL文を部分ごとに確認し、原因を切り分けながら修正しました。  
> この経験から、エラー対応では原因を一つずつ確認する姿勢が重要だと学びました。

## Risk Notes

- `[Need Confirmation]` 実際に不可視文字が関係したか確認
- `[Need Confirmation]` 面接で使うなら、具体的な SQL エラー名や内容を補足した方がよい
- `[Inference]` SQL 経験は実務ではなく研修経験として表現する

---

# 5. STAR-04 — Git / GitHub の理解とチーム開発

## Related Project

- `[Confirmed]` Git / GitHub Team Development

## Use Cases

この STAR は以下の質問に使える：

- 新しいツールを学んだ経験はありますか
- チーム開発で意識したことはありますか
- 分からないことをどう理解しましたか
- Git / GitHub の経験はありますか

## Situation

- `[Confirmed]` 研修で Git / GitHub を学習した
- `[Inference]` グループ課題で branch、commit、push、pull、merge、Pull Request などを扱った
- `[Inference]` 最初は local branch、remote branch、main、Pull Request、merge の関係が分かりにくかった

## Task

- `[Inference]` 自分の作業を正しく GitHub に反映する必要があった
- `[Inference]` グループメンバーの作業を main に取り込む流れを理解する必要があった
- `[Inference]` チーム開発でファイルや作業履歴を管理する必要があった

## Action

- `[Inference]` git status で現在の状態を確認した
- `[Inference]` add、commit、push の流れを整理した
- `[Inference]` branch と main の役割を確認した
- `[Inference]` Pull Request が main に変更を取り込むための確認プロセスであることを理解した
- `[Inference]` GitHub 画面上で merge の流れを確認した

## Result

- `[Inference]` Git / GitHub の基本的な流れを理解した
- `[Inference]` チーム開発では、作業内容だけでなく、変更をどう共有・統合するかが重要だと学んだ
- `[Inference]` branch を分けて作業する意味を理解した
- `[Need Confirmation]` 実際に Pull Request 作成や merge を担当したか

## Japanese Answer Draft

> 研修ではGit/GitHubを使ったグループ開発も経験しました。  
> 最初は、branch、main、Pull Request、merge の関係が分かりにくい部分がありました。  
> そのため、git status で現在の状態を確認しながら、add、commit、push の流れを一つずつ整理しました。  
> また、Pull Request は変更を main に取り込むための確認プロセスだと理解し、チーム開発では作業内容だけでなく、変更の共有方法も重要だと学びました。

## Short Version

> Git/GitHubでは、branchを使った作業やPull Requestの流れを学びました。  
> 最初は分かりにくい部分もありましたが、実際に操作しながらチーム開発での基本的な使い方を理解しました。

## Risk Notes

- `[Need Confirmation]` merge を実施したか、見ただけか確認
- `[Need Confirmation]` conflict 対応経験があるか確認
- `[Inference]` Git 経験は「基礎を学んだ」と表現するのが安全

---

# 6. STAR-05 — 音楽プレーヤー発表経験

## Related Project

- `[Confirmed]` 音楽プレーヤー / グループ課題

## Use Cases

この STAR は以下の質問に使える：

- 発表経験はありますか
- チームで成果物を説明した経験はありますか
- 分かりやすく説明するために工夫したことはありますか
- グループ課題で担当したことは何ですか

## Situation

- `[Confirmed]` グループ課題として音楽プレーヤーに取り組んだ
- `[Inference]` 発表時にモニター出力や動作内容を説明した可能性がある
- `[Inference]` 機能の動作順序に沿って説明する必要があった

## Task

- `[Inference]` 自分が担当した部分、または説明担当となった部分を聞き手に分かりやすく伝える必要があった
- `[Inference]` ログやモニター出力を見ながら、各機能が何を表しているか説明する必要があった

## Action

- `[Inference]` 出力内容の順序に沿って説明を整理した
- `[Inference]` 各機能の役割を短く説明できるようにした
- `[Inference]` 発表時間に収まるように説明を調整した
- `[Inference]` グループメンバーの発表内容と重複しすぎないようにした

## Result

- `[Inference]` 自分の担当部分や出力内容を説明する経験を得た
- `[Inference]` 実装だけでなく、動作を他人に伝えることの重要性を学んだ
- `[Inference]` 発表では、機能を順番に説明すると聞き手が理解しやすいと学んだ
- `[Need Confirmation]` 実際に発表した内容
- `[Need Confirmation]` 発表後の反応

## Japanese Answer Draft

> グループ課題の音楽プレーヤーでは、発表時に動作内容を説明する機会がありました。  
> その際、単に機能名を並べるのではなく、モニター出力の順番に沿って、それぞれの操作がどのような動作につながるのかを説明するようにしました。  
> この経験を通じて、実装した内容を自分だけが理解しているだけではなく、相手に分かりやすく伝えることも重要だと学びました。

## Short Version

> 音楽プレーヤーの課題では、モニター出力の流れに沿って動作内容を説明する経験をしました。  
> 実装内容を分かりやすく伝えることの重要性を学びました。

## Risk Notes

- `[Need Confirmation]` 本当にモニター出力を担当したか確認
- `[Need Confirmation]` 発表で説明した具体的な機能名
- `[Inference]` 発表経験は自己紹介で使いやすいが、具体性を確認する必要がある

---

# 7. STAR-06 — グループ課題での役割分担

## Related Projects

- `[Confirmed]` 自動販売機
- `[Confirmed]` バックソナー
- `[Confirmed]` 音楽プレーヤー

## Use Cases

この STAR は以下の質問に使える：

- チームで取り組んだ経験はありますか
- グループ作業で意識したことは何ですか
- メンバーと協力した経験はありますか
- チーム開発で難しかったことは何ですか

## Situation

- `[Confirmed]` 研修で複数のグループ課題に取り組んだ
- `[Inference]` メンバーごとに担当範囲を分けて作業した
- `[Inference]` 自分の作業だけでなく、他メンバーの進捗や全体の動作も意識する必要があった

## Task

- `[Inference]` 限られた時間の中で、グループとして成果物を完成させる必要があった
- `[Inference]` 自分の担当部分を進めつつ、全体として動く状態にする必要があった
- `[Inference]` 発表や動作確認に向けて、メンバー間で内容を合わせる必要があった

## Action

- `[Inference]` メンバーと相談しながら役割分担を行った
- `[Inference]` 自分の担当部分を確認しながら進めた
- `[Inference]` 実装後に動作確認を行った
- `[Inference]` 不明点や問題があった場合、メンバーに相談した
- `[Need Confirmation]` User が具体的にどのようにチームへ貢献したか

## Result

- `[Inference]` グループ課題を通じて、チームで成果物を作る経験を得た
- `[Inference]` 役割分担だけでなく、全体の動作を合わせることの重要性を学んだ
- `[Inference]` 不明点を早めに確認することの重要性を理解した
- `[Need Confirmation]` 完成度
- `[Need Confirmation]` User の具体的な貢献

## Japanese Answer Draft

> 研修のグループ課題では、メンバーと役割分担をしながら作業を進めました。  
> 自分の担当部分を進めるだけでなく、最終的に全体として動くように、メンバーと相談しながら確認することを意識しました。  
> この経験を通じて、チーム開発では、自分の作業範囲だけでなく、他の部分とのつながりや、早めに相談することが重要だと学びました。

## Short Version

> グループ課題では、メンバーと役割分担をしながら作業を進めました。  
> 自分の担当部分だけでなく、全体として動作することを意識する必要があると学びました。

## Risk Notes

- `[Need Confirmation]` “役割分担”の具体例を確認
- `[Need Confirmation]` User が主導したのか、担当者の一人だったのか確認
- `[Inference]` 面接で使う場合、具体的なエピソードが必要

---

# 8. STAR-07 — バックソナーでのハード / ソフト切り分け

## Related Project

- `[Confirmed]` バックソナー / グループ課題

## Use Cases

この STAR は以下の質問に使える：

- 原因切り分けの経験はありますか
- 組込み系の課題で学んだことは何ですか
- ハードウェアとソフトウェアの違いを意識した経験はありますか
- 動作確認で工夫したことはありますか

## Situation

- `[Confirmed]` グループ課題でバックソナーに取り組んだ
- `[Inference]` センサー値や出力が想定通りにならない場面があった可能性がある
- `[Inference]` 問題の原因が配線やセンサーなどのハードウェア側か、判定条件などのソフトウェア側かを確認する必要があった

## Task

- `[Inference]` 想定通り動作しない原因を切り分ける必要があった
- `[Inference]` センサー入力値を確認し、それに応じた出力が正しく行われているか判断する必要があった

## Action

- `[Inference]` センサー値や出力状態を確認した
- `[Inference]` 配線や電源状態を確認した
- `[Inference]` ソフトウェア側のしきい値や条件分岐を確認した
- `[Inference]` ハードウェアとソフトウェアを分けて原因を考えるようにした
- `[Need Confirmation]` 実際に User が行った確認内容

## Result

- `[Inference]` 組込み系では、問題がソフトウェアだけでなくハードウェア側にある可能性も考える必要があると学んだ
- `[Inference]` センサー値を確認しながら制御条件を調整する考え方を学んだ
- `[Need Confirmation]` 実際に問題を解決したか
- `[Need Confirmation]` どのような調整を行ったか

## Japanese Answer Draft

> バックソナーの課題では、センサーの値に応じて出力を変える処理に取り組みました。  
> 動作が想定通りにならない場合、ソフトウェアの条件だけを見るのではなく、配線やセンサー値などハードウェア側の可能性も確認する必要がありました。  
> この経験を通じて、組込み系の課題では、ハードウェアとソフトウェアの両方を意識して原因を切り分けることが重要だと学びました。

## Short Version

> バックソナーの課題では、センサー値に応じた出力制御を扱いました。  
> 動作確認を通じて、ハードウェアとソフトウェアの両方を意識して原因を切り分ける重要性を学びました。

## Risk Notes

- `[Need Confirmation]` 実際にセンサー値や配線確認を行ったか
- `[Need Confirmation]` User が担当した部分か、グループ全体の経験か
- `[Inference]` 詳細が曖昧な場合、自己紹介では短く触れる程度が安全

---

# 9. STAR-08 — 研究で予測誤差を考慮した工夫

## Related Project

- `[Confirmed]` 大学院研究

## Use Cases

この STAR は以下の質問に使える：

- 研究で工夫した点は何ですか
- 自分で考えて改善した経験はありますか
- 分析力を活かした経験はありますか
- 論理的に考えた経験はありますか

## Situation

- `[Confirmed]` 大学院で LSTM を使った株価予測と売買戦略について研究した
- `[Confirmed]` 単に予測精度を見るだけではなく、予測誤差に応じて売買基準を調整する方法を検討した

## Task

- `[Inference]` 予測結果をそのまま使うのではなく、実際の売買判断にどう活用するかを考える必要があった
- `[Inference]` 予測精度だけでなく、誤差や実用面を考慮する必要があった

## Action

- `[Inference]` LSTM による予測結果を確認した
- `[Inference]` 予測誤差を考慮し、売買判断の基準を調整する方法を検討した
- `[Inference]` 単純な精度評価だけでなく、予測結果をどのように判断へつなげるかを考えた
- `[Need Confirmation]` 実際に使用した評価指標
- `[Need Confirmation]` 実験手順
- `[Need Confirmation]` 成果や結論

## Result

- `[Inference]` 予測精度だけでなく、実際の判断に活用する視点を得た
- `[Inference]` データを確認しながら仮説を立て、結果を検証する考え方を身につけた
- `[Inference]` 技術を現実の課題にどう応用するかを考える経験になった
- `[Need Confirmation]` 研究成果の具体的な結果

## Japanese Answer Draft

> 大学院では、LSTMを使った株価予測と売買戦略について研究しました。  
> 工夫した点は、予測精度だけを見るのではなく、予測結果の誤差も考慮して売買の基準を調整しようとした点です。  
> 予測結果をそのまま使うのではなく、実際の判断にどうつなげるかを意識して研究を進めました。  
> この経験を通じて、データを確認しながら仮説を立て、結果を検証して改善していく考え方を学びました。

## Short Version

> 研究では、LSTMを使った株価予測に取り組みました。  
> 予測精度だけでなく、誤差も考慮して実際の判断につなげる点を工夫しました。

## Risk Notes

- `[Confirmed]` 研究テーマ自体は使用可能
- `[Need Confirmation]` 技術面を深掘りされた場合に備えて、評価指標や実験内容を整理する必要あり
- `[Inference]` 派遣先自己紹介では短く、面接では詳しく使うのが適切

---

# 10. STAR-09 — 研修を通じた成長ストーリー

## Related Context

- `[Confirmed]` テクノプロデザイン社の研修
- `[Confirmed]` C言語、SQL、Git/GitHub を学習
- `[Confirmed]` グループ課題、個人課題に取り組んだ

## Use Cases

この STAR は以下の質問に使える：

- 研修で学んだことは何ですか
- 最近成長したと感じることはありますか
- 未経験分野をどう学びましたか
- 今後どのように現場で成長したいですか

## Situation

- `[Confirmed]` テクノプロデザイン社の研修で複数の技術を学習した
- `[Inference]` 最初は C言語、SQL、Git/GitHub、組込み課題など、それぞれ分からない点が多かった
- `[Inference]` 個人課題とグループ課題の両方を経験した

## Task

- `[Inference]` 基礎を理解しながら、実際の課題で手を動かす必要があった
- `[Inference]` 分からない点を放置せず、調べたり確認したりしながら進める必要があった
- `[Inference]` グループ課題では、メンバーと協力して成果物を完成させる必要があった

## Action

- `[Inference]` 課題ごとに必要な技術を確認した
- `[Inference]` エラーや不具合が出た時は、原因を切り分けながら確認した
- `[Inference]` グループ課題では、メンバーと相談しながら進めた
- `[Inference]` 発表や日報を通じて、学んだ内容を整理した

## Result

- `[Inference]` C言語、SQL、Git/GitHub、組込み基礎について理解を深めた
- `[Inference]` 実装、動作確認、改善の流れを経験した
- `[Inference]` 分からないことを確認しながら進める重要性を学んだ
- `[Inference]` 研究で得た分析思考と、研修での実装経験をつなげて説明できるようになった

## Japanese Answer Draft

> 研修では、C言語、SQL、Git/GitHubを中心に学びました。  
> 最初は分からない点も多くありましたが、課題に取り組む中で、エラーや不具合の原因を一つずつ確認しながら進めることを意識しました。  
> また、グループ課題ではメンバーと相談しながら役割分担を行い、実装や動作確認を経験しました。  
> この研修を通じて、技術の基礎だけでなく、分からない点を早めに確認し、着実に進める姿勢の重要性を学びました。

## Short Version

> 研修を通じて、C言語、SQL、Git/GitHubの基礎を学びました。  
> 課題では、実装や動作確認を行いながら、不明点を確認して進める大切さを学びました。

## Risk Notes

- `[Inference]` 全体ストーリーとして使いやすい
- `[Need Confirmation]` 具体的な一つの出来事を入れると、面接回答として強くなる
- `[Inference]` 自己紹介の締めに使いやすい

---

# 11. Question Mapping

## 困難だったことは何ですか

Recommended candidates:

1. STAR-01 — Timer 状態管理問題の修正
2. STAR-03 — SQL エラーの原因切り分け
3. STAR-04 — Git / GitHub の理解とチーム開発

## チームで取り組んだ経験はありますか

Recommended candidates:

1. STAR-06 — グループ課題での役割分担
2. STAR-05 — 音楽プレーヤー発表経験
3. STAR-04 — Git / GitHub の理解とチーム開発

## 自分で工夫した経験はありますか

Recommended candidates:

1. STAR-02 — Timer 入力と表示不一致の改善
2. STAR-08 — 研究で予測誤差を考慮した工夫
3. STAR-01 — Timer 状態管理問題の修正

## 問題解決経験はありますか

Recommended candidates:

1. STAR-01 — Timer 状態管理問題の修正
2. STAR-03 — SQL エラーの原因切り分け
3. STAR-07 — バックソナーでのハード / ソフト切り分け

## 研究で工夫した点は何ですか

Recommended candidate:

1. STAR-08 — 研究で予測誤差を考慮した工夫

## 最近成長したと感じることは何ですか

Recommended candidates:

1. STAR-09 — 研修を通じた成長ストーリー
2. STAR-04 — Git / GitHub の理解とチーム開発
3. STAR-01 — Timer 状態管理問題の修正

---

# 12. Strongest STAR Candidates

## Most Practical for Interview

### STAR-01 — Timer 状態管理問題の修正

理由：

- 個人課題なので、自分の行動として話しやすい
- 技術的な困難と解決がある
- 新人工程師として自然
- 組込み系の基礎につながる

## Best for Teamwork

### STAR-06 — グループ課題での役割分担

理由：

- チーム開発経験として使いやすい
- 派遣先でも評価されやすい
- 報連相、相談、役割分担に展開できる

## Best for Research / Analytical Thinking

### STAR-08 — 研究で予測誤差を考慮した工夫

理由：

- 大学院研究と強く結びついている
- User の独自性が出る
- 分析力、仮説検証、改善思考を説明しやすい

## Best for Communication

### STAR-05 — 音楽プレーヤー発表経験

理由：

- 実装内容を説明する経験として使える
- 自己紹介や派遣先挨拶にも自然につなげやすい
- 技術だけでなく伝える力を示せる

---

# 13. Risk Management

## Risk 1 — Specific Facts Are Not Fully Confirmed

現在の STAR は多くが `[Inference]` を含む。

Countermeasure:

- 面接で使用する前に User が事実確認する
- `[Need Confirmation]` を埋める
- 不確かな内容は抽象度を上げる

## Risk 2 — Overclaiming

研修課題を実務経験のように話すと過剰に聞こえる。

Avoid:

- 実務で担当しました
- 主導しました
- 大きく貢献しました
- 高度な開発を行いました

Prefer:

- 研修課題で取り組みました
- 実装や動作確認を経験しました
- 基礎を学びました
- 確認しながら進めました

## Risk 3 — Too Many Stories

面接や自己紹介で複数の STAR を一度に話すと焦点がぼやける。

Countermeasure:

- 質問ごとに 1 つの STAR を選ぶ
- 自己紹介では STAR を詳細に話さない
- 面接では 1 つを深く話す

## Risk 4 — Follow-up Questions

具体的に話すほど、技術的な深掘り質問が来る可能性がある。

Countermeasure:

- 話す前に技術的な説明を準備する
- 自信がない部分は抽象度を上げる
- `[Need Confirmation]` が残っている STAR は面接本番で使わない

---

# 14. Next Update Candidates

今後追加・更新すべき内容：

- `[Need Confirmation]` Timer の最終仕様
- `[Need Confirmation]` Timer で最も苦労した Bug
- `[Need Confirmation]` SQL で実際に発生したエラー
- `[Need Confirmation]` 音楽プレーヤーで User が担当した機能
- `[Need Confirmation]` グループ課題での User の役割
- `[Need Confirmation]` バックソナーで User が担当した内容
- `[Need Confirmation]` Git / GitHub で実際に行った操作
- `[Need Confirmation]` 研究で使用した評価指標や成果

---

# 15. Revision Policy

本文件は継続的に更新する。

更新時の注意：

- 実際に確認できた内容は `[Confirmed]` に変更する
- 推測のままの内容は `[Inference]` として残す
- 面接で使う予定の STAR は、必ず User が事実確認する
- STAR は長くしすぎず、質問ごとに使いやすい形に整理する
- 同じ経験でも、自己紹介用、面接用、技術説明用で長さを変える
- 重要な更新を行った場合は `CHANGELOG.md` に記録する