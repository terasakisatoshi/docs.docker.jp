﻿.. -*- coding: utf-8 -*-
.. URL: https://docs.docker.com/engine/reference/commandline/compose_pull/
.. SOURCE: 
   doc version: 20.10
      https://github.com/docker/docker.github.io/blob/master/engine/reference/commandline/compose_pull.md
.. check date: 2022/03/06
.. ------------------------------------------------------------------

.. docker compose pull

=======================================
docker compose pull
=======================================

.. sidebar:: 目次

   .. contents:: 
       :depth: 3
       :local:

.. _compose_pull-description:

説明
==========

.. Pull service images

サービスのイメージを取得します。

.. _compose_pull-usage:

使い方
==========

.. code-block:: bash

   $ docker compose pull [SERVICE...]

.. Extended description

.. _compose_pull-extended-description:

補足説明
==========

.. Pulls an image associated with a service defined in a compose.yaml file, but does not start containers based on those images.

``compose.yaml`` ファイル内で定義されたサービスに関連するイメージを取得しますが、各イメージを元にしたコンテナ起動しません。

.. _compose_pull-options:

オプション
==========

.. list-table::
   :header-rows: 1

   * - 名前, 省略形
     - デフォルト
     - 説明
   * - ``--ignore-pull-failures``
     - 
     - 取得（pull）が失敗したイメージを無視
   * - ``--include-deps``
     - 
     - サービスと依存関係が宣言されたイメージも取得
   * - ``--no-parallel``
     - ``true``
     - 非推奨。並列取得を無効化
   * - ``--parallel``
     - ``true``
     - 非推奨。並列に複数のイメージを取得
   * - ``--quiet`` , ``-q`` 
     - 
     - 進捗情報を表示せずに取得


親コマンド
==========

.. list-table::
   :header-rows: 1

   * - コマンド
     - 説明
   * - :doc:`docker <docker>`
     - Docker CLI のベースコマンド。


.. Related commands

関連コマンド
==========

.. list-table::
   :header-rows: 1

   * - コマンド
     - 説明
   * - :doc:`docker compose biuld<compose_build>`
     - サービスの構築もしくは再構築
   * - :doc:`docker compose convert<compose_convert>`
     - compose ファイルをプラットフォーム固有の形式に変換
   * - :doc:`docker compose cp<compose_cp>`
     - サービス・コンテナとローカル・ファイルシステム間でファイルやフォルダをコピー
   * - :doc:`docker compose create<compose_create>`
     - サービス用のコンテナを作成
   * - :doc:`docker compose down<compose_down>`
     - コンテナやネットワークの停止と削除
   * - :doc:`docker compose events<compose_events>`
     - コンテナからリアルタイムにイベントを受信
   * - :doc:`docker compose exec<compose_exec>`
     - 実行中のコンテナ内でコマンドを実行
   * - :doc:`docker compose images<compose_images>`
     - 作成したコンテナが使っているイメージを一覧表示
   * - :doc:`docker compose kill<compose_kill>`
     - サービスコンテナを強制停止
   * - :doc:`docker compose logs<compose_logs>`
     - コンテナからの出力を表示
   * - :doc:`docker compose ls<compose_ls>`
     - 実行中の compose プロジェクトを一覧表示
   * - :doc:`docker compose pause<compose_pause>`
     - サービスの一時停止
   * - :doc:`docker compose port<compose_port>`
     - ポートを確保している公開ポートを表示
   * - :doc:`docker compose ps<compose_ps>`
     - コンテナを一覧表示
   * - :doc:`docker compose pull<compose_pull>`
     - サービスのイメージを取得
   * - :doc:`docker compose push<compose_push>`
     - サービスのイメージを送信
   * - :doc:`docker compose restart<compose_restart>`
     - コンテナの再起動
   * - :doc:`docker compose rm<compose_rm>`
     - 停止済みのサービス・コンテナを削除
   * - :doc:`docker compose run<compose_run>`
     - サービスを一度限りのコマンドとして実行
   * - :doc:`docker compose start<compose_start>`
     - サービスの開始
   * - :doc:`docker compose stop<compose_stop>`
     - サービスの停止
   * - :doc:`docker compose top<compose_top>`
     - 実行中のプロセスを表示
   * - :doc:`docker compose unpause<compose_unpause>`
     - サービスの一時停止を解除
   * - :doc:`docker compose up<compose_up>`
     - コンテナの作成と開始


.. seealso:: 

   docker compose pull
      https://docs.docker.com/engine/reference/commandline/compose_pull/
