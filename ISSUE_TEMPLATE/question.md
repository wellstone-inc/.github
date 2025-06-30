name: 🐛 バグ報告
description: アプリケーションの不具合を報告します。
labels: ["bug"]
body:
  - type: markdown
    attributes:
      value: |
        ## 🐛 バグの概要

  - type: textarea
    id: bug_description
    attributes:
      label: バグの詳細
      description: 発生している問題の詳細を記載してください。
    validations:
      required: true

  - type: textarea
    id: steps
    attributes:
      label: 再現手順
      description: バグを再現するためのステップを明記してください。
    validations:
      required: true

  - type: textarea
    id: expected
    attributes:
      label: 本来期待される挙動
      description: 正常時の動作を記載してください。

  - type: textarea
    id: logs
    attributes:
      label: ログ・スクリーンショット
      description: 関連するエラーログやスクリーンショットがあれば貼ってください。

  - type: input
    id: environment
    attributes:
      label: 実行環境
      description: OS、ブラウザ、アプリバージョンなど。
