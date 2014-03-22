ALIASING
========

概要
----

ダウンサンプリングしたときにエイリアシングが起きるといいます。

倍速再生するためにサンプル数を減らした場合も同じでしょうか。サンプル数を減らしただけで、サンプリング周波数はそのままです。

原音
----

チャンネル数       |        2
サンプリング周波数 | 44.1 kHz

原音の周波数スペクトルです。
横軸は[十二平均律](http://ja.wikipedia.org/wiki/平均律)です。

| ![左チャンネル](http://purasi-bo.me/image/aliasing/base.d/left.gif) | ![右チャンネル](http://purasi-bo.me/image/aliasing/base.d/right.gif) |

倍速化
------

奇数番だけ取ってサンプル数を半分にしました。サンプリング周波数はそのままです。

そのまま倍速化しているものと、11.025 kHz で Low Pass Filter してから倍速化しているものとを比べます。

振幅は 3000 で正規化しています。

[speed up](speed_up.md)

LPF
---

Low Pass Filterが効いているかどうかを確認するために比べます。

[lpf](lpf.md)

ダウンサンプリング
------------------

ダウンサンプリングしたときにエイリアシングがおきるかどうかを確認します。

[down sampling](down_sampling.md)
