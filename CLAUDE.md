# CLAUDE.md

このファイルは、このリポジトリでコードを扱う際のClaude Code (claude.ai/code) へのガイダンスを提供します。

## 必須
- 回答は日本語で行ってください
- コード生成するときはCLAUDE.mdのコーディング規約に従ってください

### ファイル構造とフォルダ規約
- フォルダ名はUpperCamelCaseで間にスペースは含めないようにしてください
- 拡張子は全て小文字にしてください

### コーディングスタイル
- **スペース**: タブは使わずに半角スペース2つで代用してください
- **空行**: 空行にはスペースやタブを含めず、完全に空の行にする

## プロジェクト概要

基本的なURP（Universal Render Pipeline）設定を実演するUnity 3Dサンプルプロジェクトです。Unity 6000.1.1f1を使用し、テンプレートまたは学習リソースとして機能します。

## 主要技術
- Unity 6000.1.1f1
- Universal Render Pipeline (URP) 17.1.0
- Unity Input System 1.14.0
- C# スクリプト

## 開発コマンド

### プロジェクトを開く
- Unity Hubを開き、このプロジェクトフォルダを追加: `ClaudeCodeUnityMCPSample/`
- 必要なUnityバージョン: 6000.1.1f1

### ビルド
- Unity EditorのBuild Settingsを使用（File → Build Settings）
- デフォルトのビルドターゲットはUnityのProjectSettings経由で設定されます

### テスト
- Unity Test Framework 1.5.1を使用
- Unity のTest Runnerウィンドウからテストを実行（Window → General → Test Runner）

## アーキテクチャ注記

### レンダーパイプライン
- プロジェクトはUniversal Render Pipeline (URP)用に設定されています
- PCとモバイルプラットフォーム用の個別のレンダーアセット
- サンプルシーン用にポストプロセッシングボリュームプロファイルが設定されています

### Input System
- UnityのnewInput Systemパッケージを使用
- Input actionsは`InputSystem_Actions.inputactions`で定義されています

### スクリプト
- 最小限のスクリプト - 主にチュートリアルヘルパークラスが含まれています
- `Readme.cs`はチュートリアル情報表示用のScriptableObject構造を定義します

## 重要なファイル
- `Assets/Scenes/SampleScene.unity` - メインシーンファイル
- `Packages/manifest.json` - パッケージ依存関係
- `ProjectSettings/ProjectVersion.txt` - Unityバージョン情報
- `Assets/Settings/` - URPレンダーパイプライン設定

## 開発に関する注記
- これはカスタムコードが最小限のサンプル/テンプレートプロジェクトのようです
- 機能の大部分はUnityパッケージとURP設定に由来します
- ゲームプレイコードよりもレンダーパイプライン設定に主眼が置かれています