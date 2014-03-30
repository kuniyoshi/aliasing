ALIASING
========

概要
----

ダウンサンプリングしたときにエイリアシングが起きるといいます。

倍速再生するためにサンプル数を減らした場合も同じでしょうか。サンプル数を減らしただけで、サンプリング周波数はそのままです。

原音
----

チャンネル数は`2`ですが、簡単のため左チャンネルだけ使います。

サンプリング周波数は`44.1`kHzです。

原音の周波数スペクトルです。 横軸は[十二平均律](http://ja.wikipedia.org/wiki/平均律)です。

![左チャンネル](/image/base.d/left.gif)

倍速化
------

奇数番だけ取ってサンプル数を半分にしました。サンプリング周波数はそのままです。

そのまま倍速化しているものと、`11.025`kHz で Low Pass Filter してから倍速化しているものとを比べます。

振幅は`3000`で正規化しています。

[周波数スペクトル](speed_up.md)

LPF
---

Low Pass Filterが効いているかどうかを確認するために比べます。

エッジ周波数は`1`kHz で、遷移帯域幅は`0.5`kHz です。

[周波数スペクトル](lpf.md)

ダウンサンプリング
------------------

ダウンサンプリングしたときにエイリアシングがおきるかどうかを確認します。

LPF のエッジ周波数は`11.025`kHz で遷移帯域幅は`1`kHz です。

[周波数スペクトル](down_sampling.md)
