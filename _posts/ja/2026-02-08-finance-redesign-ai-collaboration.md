---
layout: post
title: "家計簿Webアプリ再設計: AI分業を実務に落とし込む"
date: 2026-02-08
categories: [project]
tags: [finance, ui-ux, portfolio, ai-collaboration, codex, gemini, antigravity]
lang: ja
---

# 家計簿Webアプリ再設計: AI分業を実務に落とし込む

## プロジェクト概要
今回は、バックエンドAPIとデータ構造を変更せず、家計簿WebアプリのUIを再設計しました。  
狙いは見た目の改善だけでなく、**再利用可能なAI協業プロセス**を作ることです。

## この事例の価値
- 1つのモデルに全工程を任せると品質が不安定になりやすい。
- 本件ではAIを役割で分離しました。
  - **Gemini 3 Pro**: デザイン提案・方向性比較
  - **Codex**: 最小差分での実装反映
  - **Antigravity (+ Nano Banana 2)**: ワークフロー運用・視覚素材整備
- その結果、手戻りを減らし、品質の再現性を高められました。

## AI分業の判断基準
### 1) Gemini 3 Pro（提案フェーズ）
- 情報設計、視線誘導、トーン統一の案出しに強い。
- 実装前に複数案を短時間で比較可能。

### 2) Codex（実装フェーズ）
- 採用案（C案+A案ハイブリッド）のみを反映。
- 制約: API/データ構造は変更しない。
- コード差分を小さく保ち、390pxモバイル崩れも検証。

### 3) Antigravity（運用フェーズ）
- 手順のオーケストレーションと素材管理を担当。
- Nano Banana 2を含む視覚資料をポートフォリオ向けに整理。

## 実行プロセス
1. 再設計の範囲と制約を固定
2. Gemini 3 Proで複数のデザイン案を生成
3. 最終方針を選定（C案+A案）
4. Codexで最小差分実装
5. デスクトップ/モバイルの画面キャプチャ作成
6. GitHub Pages公開 + Notionへプロジェクト同期

## 成果
- 情報の優先順位が明確化され、視認性が向上
- 390pxモバイル表示でレイアウト崩れなし
- ポートフォリオ用スクリーンショットを2種作成
- 次案件にも転用できるAI分業手順を確立

## スクリーンショット
![Finance redesign desktop](/images/portfolio/finance-redesign-desktop-2026-02-08.png)
![Finance redesign mobile](/images/portfolio/finance-redesign-mobile-2026-02-08.png)

## ソースリポジトリ
- ワークスペース: [INO95/moltbot-workspace-202602](https://github.com/INO95/moltbot-workspace-202602)
- ブログ: [INO95/ino95.github.io](https://github.com/INO95/ino95.github.io)

## 実務的な示唆
この事例の本質は「UI改善」だけではなく、**モデルの得意領域に合わせた分業設計**です。  
設計・実装・運用を分離し、制約を守りながら品質を上げる実践例として再現性があります。
