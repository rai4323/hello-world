---
layout: page
title: "software Eng. lecture note"
permalink: /docs/softwareEng2025
---
# ソフトウェア工学のまとめ

ソフトウェアについて、実社会で利用されるソフトウェアは規模が大きくその内容も複雑である。それに伴い、開発の効率性や保守性が求められる。また、IT化に伴いIT人材の不足も問題になっている。さらに、様々なソフトウェアの普及に伴いソフトウェアが想定しない方法で利用されるという問題も発生している。  
ソフトウェアライフサイクルとはソフトウェアの誕生から開発を経て廃止までに至る全ての工程のことを指す。要件定義の段階では、システムの目的や機能、構成、スケジュールなど開発の際に考慮すべき事項を事細かに定義する。その後、要件定義の内容を基に設計を行ったりWBSの作成を行ったりする。WBSとはプロジェクトの作業を階層的に細分化したものであり、作業の洗い出しやスコープを分かりやすくすることが出来る。設計段階が終了した後は制作段階に入る。制作には自社で開発を行う内製や外部に委託する調達などの形態がある。調達については海外の安価な労働力を利用するオフショア開発という形態もある。プロジェクトは大きく有期性と独自性の2種類に分けられる。ソフトウェア開発は独自性のプロジェクトに属する。また、プロジェクトにはフォアキャスティングとバックキャスティングという視点がある。フォアキャスティングは、作業内容に着目しながらプロジェクトを進行していく。目標を明確に決定しないため成果物が目標と食い違う可能性がある。一方でバックキャスティングでは成果物に着目しながらプロジェクトを進行していく。目標を明確に決定するため、フォアキャスティングのように成果物と目標との間に食い違いが生じる可能性が少ない。プロジェクトを実行する際には目標に対する具体的なタスク等をあらかじめ考えることが必要である。  
ソフトウェア分析について、ソフトウェアの評価指標としてコードの行数や容量などが利用される。ソフトウェアの品質に関する1つの指標としてのバグはコード1行当たりのバグ数であるバグ発生率で表される。ソフトウェアの規模を評価する指標としてファンクションポイント法がある。  
主な開発手法として、ウォーターフォール開発やアジャイル開発などが挙げられる。ウォーターフォール開発では、前工程が全て完了してから次の工程に進む。アジャイル開発では機能を分割して繰り返し開発を行う。この手法では、修正を行いやすく柔軟な開発が可能である。  
コーディングを行う際には、1行の文字数を79文字以内にすることや、文を改行する際は縦に揃えること、インデントを半角スペース4つ分とすること、1つの文ごとに改行することなど様々なルールが存在する。  
バージョン管理には主にgitを利用する。gitを利用するとバージョンを容易に管理することができ、例えば過去のバージョンに戻ったり、他者と資源を共有しながら開発を行ったりすることが出来る。ファイルに対する何らかのアクションを記録するための操作をコミットと呼ぶ。ローカルレポジトリでは、まずワークツリー内で変更を行い、変更したファイルをステージングエリアに追加してその後コミットを行う。ローカルレポジトリからリモートレポジトリに対する同期はpush、リモートレポジトリからローカルレポジトリに対する同期はpullによって行う。現在の作業からの分岐をブランチと呼ぶ。
GitHubではリモートレポジトリをcloneすることでローカルレポジトリを作成することが出来る。  
CIとはContinuous Integrationの略であり自動的にビルドやテストを行うことで開発の生産性を向上させることが出来る。
CDとはContinuous Deliveryの略であり自動的にデプロイを行うことが出来る。
具体的な流れとして、何らかの操作がトリガーとなって定義されたワークフローが立ち上がる。その後、ビルドを行いテストを実行する。テスト後はデプロイをして、デプロイ後に動作確認を行う。その後はモニタリングを続ける。