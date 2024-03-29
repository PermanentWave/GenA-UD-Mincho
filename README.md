# 源亜 UD明朝について
この源亜(げんあ) UD明朝は、Amazon Kindle Paperwhite/Oasis上で[BIZ UD明朝](https://github.com/googlefonts/morisawa-biz-ud-mincho)を極力適用する為に改良をしたものです。  
Kindleには \\\\Kindle\\fonts フォルダに外部フォントを配置することで、組み込み以外のフォントを使用できる機能が公式に備わっています。  
しかし、組み込み以外のフォントを使用した場合、フォントが斜体のグリフを持っていなければ標準体フォントを参照する仕様があり、これを回避するために源亜フォントを作成しました。  
PC、スマートフォン等、他の端末でも使用できますが、これらの端末は自身で標準体を斜体に見せかける機能があるため、このフォントを使用するメリットはありません。
BIZ UD明朝を使用することを推奨します。  
名前の由来は基のフォントの名前「源」と亜馬孫/亜馬生(アマゾン)、亜種の「亜」から取っています。<s>語呂が悪い。</s>  

# フォントの使い方
\\\\Kindle\\fonts フォルダに、2つの GenAUDMinchoVertical-\*\*.ttf を入れると縦書き用、 GenAUDMinchoHorizontal-\*\*.ttf を入れると横書き用がKindle上で設定できるようになります。  
不要の場合はこれらファイルを削除してください。  
書籍によっては明朝体/ゴシック体を指定している箇所があり、本文と違う書体が指定されている場合は組み込みの明朝/ゴシックフォントが読み込まれます。
これは回避できない仕様です。  
なお、これらの.ttfファイルを.ttcファイルにまとめた場合、太字・斜体フォントが動作しませんので、.ttcファイルに改変しての使用はお勧めしません。

# フォントの特徴  
標準(Regular)については、基となったBIZ UD明朝のグリフを一切変えていません。太字・斜体フォントと互換性を持たせるため、フォント名等の設定調整に留めています。  
斜体はfontforgeの機能で、標準、太字を文末方向へそれぞれ13度斜めに歪ませています。
縦書き用、横書き用で歪ませている方向が違います。  

# 更新履歴  
- ver. 3.01 (2023/03/21)  
    - 縦書きフォントの傾きを変更(13度→10度)  
    - Licenseの間違いを修正  
- ver. 3.00 (2023/03/12)  
    - 日本語フォント名を変更  
    - ヒンティングを削除  
    - OS2_Panose、TTF名の見直し  
    - 開発環境を一新  
        - Ubuntu 22.04  
        - fontforge 20220308  
        - ttfautohint 1.8.3  
        - Python 3.11  
- ver. 2.00+ (2023/03/06)
    - Boldフォントを追加
- ver. 2.00 (2022/05/22)
    - 初版  

# ライセンス
[SIL Open Font License 1.1](https://github.com/PermanentWave/GenA-Koburi-Mincho/blob/main/LICENSE_OFL.txt)のもと配布いたします。
個人利用・商用利用にかかわらず、無償で使用することができ、再配布やソフトウェアへの組み込み、改変などが可能です。  
その他利用に関する免責条項の詳細は、[SIL Open Font License 1.1](https://github.com/PermanentWave/GenA-Koburi-Mincho/blob/main/LICENSE_OFL.txt)をご確認ください。\([日本語サイトリンク](https://licenses.opensource.jp/OFL-1.1/OFL-1.1.html)\)  
本フォントを使用した事により発生した事象に対し、フォント作成者は何の責任も持ちません。自己責任でお使いください。  
「予約されたフォント名」は日本語表記では「源亜」、アルファベット表記では「GenA」とします。  
本フォントに問題がある場合はGithubのIssueまたは[Twitter](https://twitter.com/O_PermanentWave)に連絡をお願い致します。  

# 謝辞
モリサワ BIZ UD明朝/ゴシックを配布してくださっている[Google-Fonts](https://github.com/googlefonts/)様  
vmtx修正ソフトウェア[o_vmtx-fix](https://okoneya.jp/font/knowhow.html)を配布、fontforgeで源ノ明朝/源ノ角ゴシックを改変する方法について解説してくださっている[御琥祢屋](https://okoneya.jp/)様  
各グリフの表示を確認する電子書籍を公開してくださっている[wakufactory](https://wakufactory.jp/densho/font/mojitest.html)様  
この場をお借りし、感謝申し上げます。

# 参考
> [源亜こぶり明朝作成の備忘録](https://permanentwave.github.io/2021/07/24/2021-07-24-01/)  
> [fontforge Module attributes](https://fontforge.org/docs/scripting/python/fontforge.html)  
> [OS/2 — OS/2 and Windows Metrics Table](https://docs.microsoft.com/en-us/typography/opentype/spec/os2)  
> [Unicode Vertical Orientation Revision 17](https://unicode.org/Public/vertical/revision-17/VerticalOrientation-17.html)
