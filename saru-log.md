Saru
====

## 現状

現状では簡単な四則演算ができる程度。まったく実用的ではない。

アセンブラ部分が原始的すぎるのがひとつ、開発の妨げになっているというか、
Assembler.cc を自動生成するようにすれば、コンパイル時にエラーを発見で
きるので、楽になるという目論見はある。

できるだけ初期段階でやったほうが効果は大きいから、がんばってやっつけた
い。src/core/oplist を変換すればいいだけなんで、そんなにむずかしい作業
ではない。

## 2013-06-17

nqp-cc/nqp-src/NQPCORE.setting がブートストラップだった!!
意外とこの部分のコードを C++ なりなんなりでかかないと、まともにならな
そう。。

## 2013-06-18

まあなにしろ、関数よびだしで引数がわたせるようになれば、とりあえず
fib() はもとめられそうだ。

いよいよ、ひとつの目標がたっせられるということで、非常にありがたいこと
であるよ。

## 2013-06-19

とりあえず fibonacci もとめられるようになった。Perl5 の 1.5 倍ぐらい遅
いかんじ。だけど MoarVM 自体がぜんぜん最適化されてないし、最適化オプショ
ンとかもとくにやってないんで、現状でもちょっとかえるだけでソコソコはや
いかもしれない。

まあ、速度面でいうと、生成コードの差だけって話なのだけど。
