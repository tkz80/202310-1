SEEK（ログイン85年8月号掲載・MSX用 テープソフト）を実行


<環境>
MSX2以降 VRAM128k以上 MSX-DOSが起動すること
MSX0も可

<使い方>
1.以下ファイルを入れたMSX-DOS起動FDを用意
　・BLOADER.COM ・・・ *.CAS/*.BIN ファイルをVRAMへ読み込む DOSコマンド
　・SEEKのプログラムファイル（.BAS .BIN）※要修正
　・起動用 .BAT ファイル※２

　（補足）
　・プログラムファイル
　　・ファイル名：BASIC = SEEK.BAS, マシン語 = SEEK.BIN
　　・BASICは以下のとおり修正する
　　　＜修正＞ 「:DEFUSR=&HF89F:I=USR(0)」を追記する
　　　　20 SCREEN2,2,0:OPEN"GRP:"AS#1:DEFINTA-Z:DEFUSR=&HF89F:I=USR(0)

　・起動用 .BATの例
　　　BLOADER SEEK.BIN
　　　BASIC SEEK.BAS


2.MSX-DOS が起動したら、起動用 BATファイルを実行（AUTOEXEC.BAT にしてもOK）


<お断り>
・実験的にプログラムを組んでいるため、動作保証は出来かねます。
・所持していないテープソフトの動作検証はできていません。
・起動しない、途中で止まるなどが起こる可能性があります。
・予告なくプログラムの修正や削除、公開中止をすることがあります。

-----
tkz80
-----