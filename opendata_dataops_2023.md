# DataOpsを活用したオープンデータ利活用に関する報告書

Version：0.1  
公開日：2024年xx月xx日  
著者：C3Lab

![](media/image1.png)
![](media/image2.png)　By C3Lab

このドキュメントの内容物は [クリエイティブ・コモンズ 表示 4.0 ライセンス](http://creativecommons.org/licenses/by/4.0/deed.ja) [^1]の下に提供されています。

<div style="page-break-before:always"></div>

## 目次

[**１ はじめに**](#１-はじめに)  

[１-１ 本報告書の位置づけ](#本報告書の位置づけ)  
[１-２ 背景](#背景)  

[**２ 検証イベント実施内容**](#２-検証イベント実施内容)  

[２-１ オープンデータDataOps検証イベント](#オープンデータdataops検証イベント)  
[２-２ 検証イベント詳細](#検証イベント詳細)  
[２-３ イベントにて実施したアンケート結果](#イベントにて実施したアンケート結果)  

[**３ 考察**](#３-考察)  

[**４ まとめ**](#４-まとめ)  

[**５ 今後の展望**](#５-今後の展望)  

## **１ はじめに**

### **本報告書の位置づけ**
2022年度版の「[DataOpsを活用したオープンデータ利活用に関する報告書](opendata_dataops.md)」（以下、2022年度報告書）で提案したDataOpsプロセスのオープンデータ利活用への有効性を証明する為、各プロセスにおける作業を体験する開発イベントを開催した。  
本報告書は開発イベントで得た成果や課題を元に、有効性の確認と改善案をとりまとめたものである。

### 背景
2022年度報告書ではオープンデータ利活用の阻害要因として以下の問題を挙げた。
- 必要なデータが探しづらい
- 必要なデータが公開されていない
- オープンデータの認知度が低い
- 利用者のニーズが解らない

この阻害要因を解消する為の手法としてDataOpsの概念に焦点を当てている。

#### DataOpsとは
ガートナー社の定義[^2]によると「組織全体のデータ管理者とデータ利用者の間のコミュニケーションの向上と、データフローの統合と自動化の改善に焦点を当てた共同作業によるデータ管理の手法」と定義している。DataOpsの概念を利用することで、利用者が必要なタイミングで信頼できるデータや分析結果を入手可能となり、データの利用者と提供者が協調することでプロセス、ツール環境や組織文化の継続的な改善が期待できる。  

この概念を利用することでこれらの阻害要因を解消することが可能であるという仮説に基づき、DataOpsのプロセスを提案した。  

以下の図は、提案したDataOpsのプロセス図とその内容である。

![](media/image54.png)

※各ステークホルダーやユースケースの詳細については[2022年度報告書](opendata_dataops.md)を参照  

この提案の有効性については検証中であり、有効性の確認の為、イベントを行うこととした。

## ２ 検証イベント実施内容

### **オープンデータDataOps検証イベント**
検証イベントとして以下のイベントを実施した。  
- Social Hack Day #56 2023年12月16日開催
- Social Hack Day #57 2024年01月20日開催
- Social Hack Day #58 2024年02月17日開催
- オープンデータ・デイ in 沖縄 2024年03月開催
- Code for Japan+TIS スマートシティイベント 2024年03月開催

### **検証イベント詳細**

#### **Social Hack Day #56**  (イベント詳細：[Social Hack Day #56 イベントレポート](event/event_report_20231216.md))  

##### 概要
データ利用者がオープンデータをデータの可視化に活用することを前提とした時、データ利用者の観点で、データを有効に活用するにはどのような構成とすべきかをデータ提供者のプロセスである「データの収集蓄積」を通して議論し、このプロセスの有効性を確認する。

##### 成果  
<table border="1">
  <thead>
    <tr style="text-align:center">
      <th width="600px" rowspan="2">成果</th>
      <th colspan="8">関連するDataOpsプロセス</th>
    </tr>
    <tr>
      <th style="writing-mode: tb-rl;">課題抽出</th><th style="writing-mode: tb-rl;">計画</th><th style="writing-mode: tb-rl;">データの収集蓄積</th><th style="writing-mode: tb-rl;">データの公開</th><th style="writing-mode: tb-rl;">データの取得</th><th style="writing-mode: tb-rl;">データの処理</th><th style="writing-mode: tb-rl;">データの活用</th><th style="writing-mode: tb-rl;">フィードバック</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>国の制度関連の取り組みを行っているプロジェクトでDataOpsの概念を組み込んでいきたいという意見が上がった</td>
      <td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td>自治体がオープンデータを提供するプロセスを体験することで、作業量等の観点から自治体職員が手作業でデータ加工を行うのは現実的ではないということを実感した</td>
      <td></td><td></td><td>○</td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td>オープンデータ提供者にとって生成系AIによるレビューが有効な手段であることを実感できた</td>
      <td></td><td></td><td>○</td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td>フィードバックをトリガーとしてDataOpsプロセスの課題抽出・計画・データの公開・取得・活用の要素を満たす機能を有しているCKAN拡張機能（ckanext-feedback）をイベント参加者が実際に体験することでDataOpsプロセスにおける善循環サイクルへの理解を促進できた</td>
      <td>○</td><td>○</td><td></td><td>○</td><td>○</td><td></td><td>○</td><td>○</td>
    </tr>
    <tr>
      <td>博物館では所蔵品のデータの提供を積極的に実施している為、カルチャーの領域でも活用してみたいという意見が上がった</td>
      <td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td>ChatGPTを使ってデータ構造についてレビューを実施したところ問題点と改善に関するアイデアを検討してくれた</td>
      <td></td><td></td><td>○</td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td>ChatGPTによる可視化は細かい要求に対しても適切にデータを生成してくれる為、データ利用者にとって活用できるツールであることを実感した</td>
      <td></td><td></td><td></td><td></td><td></td><td></td><td>○</td><td></td>
    </tr>
  </tbody>
</table>

##### 課題  
<table border="1">
  <thead>
    <tr style="text-align:center">
      <th width="600px" rowspan="2">課題</th>
      <th colspan="8">関連するDataOpsプロセス</th>
    </tr>
    <tr>
      <th style="writing-mode: tb-rl;">課題抽出</th><th style="writing-mode: tb-rl;">計画</th><th style="writing-mode: tb-rl;">データの収集蓄積</th><th style="writing-mode: tb-rl;">データの公開</th><th style="writing-mode: tb-rl;">データの取得</th><th style="writing-mode: tb-rl;">データの処理</th><th style="writing-mode: tb-rl;">データの活用</th><th style="writing-mode: tb-rl;">フィードバック</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>オープンデータがPDFで公開されている為、データ利用者は扱いづらい</td>
      <td></td><td></td><td>○</td><td>○</td><td></td><td>○</td><td>○</td><td></td>
    </tr>
    <tr>
      <td>自動化して効率的にデータの整形を行いたい</td>
      <td></td><td></td><td>○</td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td>自治体側がファイルに変更を加えた際、その変更がデータ利用時に大きな障害になってしまう場合がある為（想定外の項目が追加されている等）、相互のコミュニケーションが必要だと感じた</td>
      <td></td><td></td><td>○</td><td></td><td></td><td></td><td>○</td><td></td>
    </tr>
    <tr>
      <td>以下の理由から初めにフォーマットを用意しておく必要性を実感した<br>● 地域ごとにフォーマットが異なる<br>● 半角全角、記号などの統一が行われていない<br>● 自治体がオープンデータに加えた工夫で、かえって扱いにくいデータ形式になってしまっている</td>
      <td></td><td></td><td>○</td><td></td><td></td><td>○</td><td>○</td><td></td>
    </tr>
    <tr>
      <td>大元のデータが更新されると、リンクが無効になってしまう問題が発生したため、データ更新の際、何かアナウンスがあるべきだと感じた</td>
      <td></td><td></td><td></td><td>○</td><td>○</td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td>文化資源の領域のオープンデータも利活用したいという意見があったが、オープンデータの認知度や法整備などの課題がある</td>
      <td></td><td>○</td><td></td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td>ChatGPTが出してくれたデータ構造は細かく、確かに正しいが項目が大量になってしまうためデータ作成のコストがかかる</td>
      <td></td><td></td><td>○</td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td>CKANにオープンデータを公開するにあたりバージョンを意識する必要があるが、有識者のサポートが必要になる可能性が高い</td>
      <td></td><td></td><td></td><td>○</td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td>ChatGPTによる可視化はデータ利用者にとって活用できるツールではあるが、指示文のちょっとしたニュアンスの違いで結果が変わってしまうこともある為、必ず結果が確かなものかを確認する必要がある</td>
      <td></td><td></td><td></td><td></td><td></td><td></td><td>○</td><td></td>
    </tr>
  </tbody>
</table>

#### **Social Hack Day #57**  (イベント詳細：[Social Hack Day #57 イベントレポート](event/event_report_20240120.md))  

##### 概要  
[Social Hack Day #56](#social-hack-day-56-social-hack-day-56-イベントレポート)で議論したデータの収集蓄積プロセス及びフィードバックプロセスの有効性を確認した。  

データの収集蓄積プロセスは、データ利用者がデータを有効に活用する為のデータ構造に関して継続議論した。  

フィードバックプロセスは、データ提供者のモチベーションをあげる（利活用促進につなげる）ためにはどうすべきかについてデータ利用者・データ提供者それぞれの観点で議論した。  

最後にデータの収集蓄積やデータの活用プロセスに使用することを想定して開発したAssistants API UIツールのデモを実施し、意見交換を行った。

##### 成果  

<table border="1">
  <thead>
    <tr style="text-align:center">
      <th width="600px" rowspan="2">成果</th>
      <th colspan="8">関連するDataOpsプロセス</th>
    </tr>
    <tr>
      <th style="writing-mode: tb-rl;">課題抽出</th><th style="writing-mode: tb-rl;">計画</th><th style="writing-mode: tb-rl;">データの収集蓄積</th><th style="writing-mode: tb-rl;">データの公開</th><th style="writing-mode: tb-rl;">データの取得</th><th style="writing-mode: tb-rl;">データの処理</th><th style="writing-mode: tb-rl;">データの活用</th><th style="writing-mode: tb-rl;">フィードバック</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>データをどこまで構造化するべきかはユースケースによって変わる為、ニーズに合わせて変更可能な最小限の構造（名称、住所などの共通部分のみ）であるべきことがわかった</td>
      <td></td><td></td><td>○</td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td>ChatGPTを使用したデータ構造のレビューやデータの可視化の体験を通して、データの構造化や検索用としてChatGPTを活用することの将来性を実感できた</td>
      <td></td><td></td><td>○</td><td>○</td><td>○</td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td>オープンデータのニーズの収集は東京都職員の方がハッカソンや企業へのヒアリングを通して行っていることがわかった</td>
      <td>○</td><td></td><td></td><td></td><td></td><td></td><td></td><td>○</td>
    </tr>
    <tr>
      <td>オープンデータが循環している流れを可視化することで、さらにサイクルの加速が期待できるという意見があがった</td>
      <td></td><td></td><td></td><td></td><td></td><td></td><td>○</td><td></td>
    </tr>
    <tr>
      <td>オープンデータ作成支援AIの課題（以下課題表中に記載）を把握することができた</td>
      <td></td><td></td><td>○</td><td></td><td></td><td></td><td>○</td><td></td>
    </tr>
  </tbody>
</table>

##### 課題  

<table border="1">
  <thead>
    <tr style="text-align:center">
      <th width="600px" rowspan="2">課題</th>
      <th colspan="8">関連するDataOpsプロセス</th>
    </tr>
    <tr>
      <th style="writing-mode: tb-rl;">課題抽出</th><th style="writing-mode: tb-rl;">計画</th><th style="writing-mode: tb-rl;">データの収集蓄積</th><th style="writing-mode: tb-rl;">データの公開</th><th style="writing-mode: tb-rl;">データの取得</th><th style="writing-mode: tb-rl;">データの処理</th><th style="writing-mode: tb-rl;">データの活用</th><th style="writing-mode: tb-rl;">フィードバック</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>オープンデータの利用者と提供者一人一人のモチベーションをあげる仕組みが必要</td>
      <td></td><td></td><td></td><td></td><td></td><td></td><td></td><td>○</td>
    </tr>
    <tr>
      <td>データを構造化しすぎることでデータ提供者の作業コストが増加してしまう</td>
      <td></td><td></td><td>○</td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td>データ提供者とデータ利用者の間を仲介する（データを構造化する）ステークホルダが善循環のサイクルに存在しない</td>
      <td></td><td></td><td>○</td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td>オープンデータを整備する部署と公開する部署が異なる場合、フィードバックコメントを読まないことがある為、データ利用者の声がデータを整備する部署の担当者まで届かない</td>
      <td></td><td></td><td></td><td></td><td></td><td></td><td></td><td>○</td>
    </tr>
    <tr>
      <td>利用者が提供者に対して感謝の意識をもてるような仕組みが必要</td>
      <td></td><td></td><td></td><td></td><td></td><td></td><td>○</td><td>○</td>
    </tr>
    <tr>
      <td>フィードバックには報告、要望などの種類があるが、ネガティブな要素を可能な限り減らす為には「データのこの部分を修正しました」のような報告ベースのフィードバックであるべき</td>
      <td></td><td></td><td></td><td></td><td></td><td></td><td></td><td>○</td>
    </tr>
    <tr>
      <td>提供者はフィードバックとして返ってきたデータを修正する際に、責任やチェック作業にかかるコストに抵抗感を感じる恐れがある</td>
      <td></td><td></td><td>○</td><td></td><td></td><td></td><td></td><td>○</td>
    </tr>
    <tr>
      <td>DataOpsのスタートは利用者のニーズ収集から始まるため、それをサポートする仕組みが必要</td>
      <td>○</td><td></td><td></td><td></td><td></td><td></td><td></td><td>○</td>
    </tr>
    <tr>
      <td>ChatGPTを活用する上で、正しく解釈できるデータ構造とは何かについて検討する必要がある</td>
      <td></td><td></td><td>○</td><td></td><td></td><td></td><td>○</td><td></td>
    </tr>
    <tr>
      <td>欲しいデータを投票できる仕組みなど、楽にニーズを表明できる環境が必要</td>
      <td>○</td><td></td><td></td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td>オープンデータ作成支援AIに検索させる場合、検索のたびにすべてのデータを参照するのは非効率である為、必要な情報に関してはある程度の構造化が必要</td>
      <td></td><td></td><td>○</td><td></td><td></td><td></td><td></td><td></td>
    </tr>
    <tr>
      <td>オープンデータ作成支援AIを使用する際、プロンプトのテクニックや処理できるデータ件数の限界を把握する必要がある</td>
      <td></td><td></td><td>○</td><td></td><td></td><td></td><td>○</td><td></td>
    </tr>
  </tbody>
</table>

#### **Social Hack Day #58**  (イベント詳細：[Social Hack Day #58 イベントレポート](http://))  

##### 概要  

##### 成果  

##### 課題  

#### **オープンデータ・デイ in 沖縄**  (イベント詳細：[オープンデータ・デイ in 沖縄 イベントレポート](http://))  

##### 概要  

##### 成果  

##### 課題  

#### **Code for Japan+TIS スマートシティイベント**  (イベント詳細：[Code for Japan+TIS スマートシティイベント イベントレポート](http://))  

##### 概要  

##### 成果  

##### 課題  

### イベントにて実施したアンケート結果

DataOpsのプロセスがオープンデータ利活用促進につながるかの根拠を得る為、イベント参加者にアンケートを実施した。

[アンケート結果](event/survey/survey_20231216.md) 

## **３ 考察** 

※考察観点  

- 各イベントで実施した内容と成果からオープンデータ利活用プロセスの有効性に結び付く考察を記載
- 全イベントの課題から、課題解決することでオープンデータ利活用プロセスの有効性に結び付く考察を記載
- （有用なデータがあれば）アンケート結果からオープンデータ利活用プロセスの有効性に結び付く考察を記載

データ提供者とデータ利用者を仲介する役割をもつステークホルダーを定義する必要がある。

## **４ まとめ**  
※考察の内容を踏まえ、オープンデータ利活用促進への有効性を提言する

## **５ 今後の展望**  
オープンデータにDataOpsのプロセスを適用することがオープンデータの利活用促進につながることを証明した。
これを踏まえ、データ利用者/データ提供者への認知のさらなる普及、ひいては政府/自治体まで普及させることを目指し、日本のオープンデータの改善及び活用促進に寄与する。

## **参考文献**
[^1]: クリエイティブ・コモンズ・ライセンス, “クリエイティブ・コモンズ・ライセンス,” [オンライン]. Available: https://creativecommons.org/licenses/by/4.0/. [アクセス日: 16 09 2022].
[^2]: Gartner, Inc. and/or its affiliates., “Press Releases,” 11 9 2018. [オンライン]. Available: https://www.gartner.com/en/newsroom/press-releases/2018-09-11-gartner-hype-cycle-for-data-management-positions-three-technologies-in-the-innovation-trigger-phase-in-2018. [アクセス日: 29 8 2022].  