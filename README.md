
# Aerobatic Smoke for MSFS

![logo](doc/images/aerobatic-smoke.jpg)

----

MSFS 編隊アクロ用スモーク v1.8.0 (24-12-24)

----

編隊アクロに適した軽量なスモークを以下の機体に追加します：

- IndiaFoxtEcho MB-339
- DC Designs F-4（白スモークのみ）

追加されたスモークは特定のライトをON/OFFすることで使用出来ます。

| 色   | ライト名                  | 日本語     |
| --- | --------------------- | ------- |
| ⚪白  | **LOGO** LIGHT        | **ロゴ灯** |
| 🔴赤 | **RECOGNITION** LIGHT | **識別灯** |
| 🟢緑 | **WING** LIGHT        | **翼端灯** |
| 🟡黄 | RECOG + WING          | 識別灯+翼端灯 |


各ライトの操作はMSFSのキーバインドによって行ってください。

LOGOライトがONになっている場合、他のライトの状態に関わらず白のスモークが表示されます。


## インストール方法

zz-spitice-aerobatic-smoke をコミュニティフォルダにインストール

## MB-339 (IndiaFoxtEcho)

ライトの操作でスモークが表示されるようになります。

MB-339PANに搭載されている左手前コンソールSMOKE関連のスイッチは、本MODにより無効化されています。

オリジナルではそれぞれ

- WINGライト → 白のスモーク
- RECOGNITIONライト → カラースモーク

に対応していましたが、本MODではPAN以外も含めた全機種にて、白・カラースモークが使用可能です。

| 色   | ライト名                  | 日本語     |
| --- | --------------------- | ------- |
| ⚪白  | **LOGO** LIGHT        | **ロゴ灯** |
| 🔴赤 | **RECOGNITION** LIGHT | **識別灯** |
| 🟢緑 | **WING** LIGHT        | **翼端灯** |
| 🟡黄 | RECOG + WING          | 識別灯+翼端灯 |

オリジナルのスモークは重複表示を防止するため無効化されています。（F-4と同様）

## F-4 (DC Designs)

F-4はDCDのアプデ(23-08-04)により、WINGライト（右コンソールから操作可能）でスモークを使用することが可能になりました。
しかし、DCD製のスモークは表示時間が短く負荷も比較的高いため、本MODはそれを無効化しています。

本MODを導入した場合、スモークのON/OFFについては**LOGOライト**を使用してください。


## EFB

v1.8.0より、EFBがMB-339 PANに追加されました。

EFB上では現在本modで追加された機能の設定を行うことが出来ます。

将来的にEFBとしてのいくつかの機能（マップ等）が追加される予定です。

### EFB位置設定

EFB→設定→EFBより、EFBの位置を変更することが出来ます。
各種数値を変更すると、EFBの位置変更先にフレームが表示されます。
変更後、右下の適用ボタンを押すことで、EFBが実際に移動します。

ここで設定された位置は前席・後席共通となっています。


## HUDシステム

v1.7.0より、MB-339にHUD+HMDが追加されました。
編隊飛行に便利な様々な数値が表示されるようになります。

[HUDテストページ](https://spitice.github.io/msfs/hud/) (Chromeのみで動作確認。FireFox非対応)

### HUD/HMDのON/OFF

EFB→設定→HUDもしくはHMDより、それぞれON/OFFの切り替えが可能です。

初期状態ではHUDのみONになっています。

HMDについては、ONである状態で且つ

- 画面をズームアウトしている（約30%）
- 画面がズームアウトしていないが、HUD及び正面計器"以外"の方向を向いている

場合のみEFB→設定→Brightness→HMDで設定した濃度で表示され、それ以外の時は薄く表示されます。

### トリムとフラップ・エアブレーキ・ギアの状態変更通知

EFB→設定→HUDもしくはHMD→飛行情報拡張設定より、トリム、あるいはフラップ・エアブレーキ・ギアの状態が変更された際にHUD/HMDの右下部分にそれらを一時的に表示する機能をON/OFFすることが可能です。

HUD/HMDで共通の設定となっています。


## スモークシステムサウンド

v1.5.0より、スモーク操作を行った際、またはスモークを使用し続けている場合にサウンドエフェクトが発生するようになりました。

| 操作                 | サウンド        |
| ------------------ | ----------- |
| スモークON時            | 長めのビープ音     |
| スモークOFF時           | 短めのビープ音2回   |
| スモークONのまま色変更ボタンを操作 | 短めのビープ音     |
| スモークONの状態で5秒毎      | カッコン（クリック）音 |

スモークサウンドのアイデアについては、フライトシミュレーターDigital Combat Simulator（DCS World）にて活躍されており、世界トップクラスのバーチャルアクロチームである Virtual Blue Impulse（VBI）様より拝借しています。本スモークMODでそちらを模倣することについてご快諾して頂いたVBI隊長Tink様、そしてVBI様のご活躍をサポートされているメンバーの方々に御礼申し上げます。


## Surf Overlay (海上に点を表示)

v1.6.0より、簡易的な海面表示オーバーレイを追加され、特定の条件下で海上に点が表示されるようになりました。

このオーバーレイは、

- ギアが上がっている
- 風が2knots以下

の時に表示され、海面が見えにくい無風設定で飛行する時に役立ちます。

グリッドは3種類あり、それぞれ25m/125m/725mの間隔で点が配置されています。
また、最も内側のグリッドは低高度になるにつれ色及びサイズが変化します。

デフォルトではOFFになっており、EFB→設定→Visual EffectsからONにすることが出来ます


## 自動給油

自動給油は設定した燃料量の60%を下回り尚且つパーキングブレーキが作動している時、設定した燃料量になるよう自動的に給油を行います。

地上ではなく飛行中でも使用可能です。

なお、翼端タンクの無い機体（MB-339PAN）は、設定した燃料量の63%が実際に給油されます。（例：50%に設定した場合、自動給油が行われると燃料搭載量は31.5%となる）


## 既知の不具合

- v1.7.0: スモークインジケーターがキャノピー開閉に連動してアニメーションしない


## フォントについて

HUDのフォントには[HORNET DISPLAY](https://github.com/0x408/hornet-display/)（[LICENSE](https://spitice.github.io/msfs/hud/fonts/HornetDisplay_LICENSE.txt)）を使用しています


## 連絡先

質問やご意見等があればお気軽に Spitice までご連絡ください

X(Twitter) @spitice0 / Discord spitice


## 更新履歴

#### v1.8.0 (24-12-24)

- EFBを追加
- HUD・HMD・EFB・スモークインジケータの輝度設定を追加
- 自動調光機能を追加
- HUDフレームのモデルを更新
- HUD・HMDの表示切替をEFB上で行えるように
- HUD・HMDの色を変更（HUDの色は輝度によって変化するように）
- フライトディスプレイ（HUD・HMD上の飛行情報）
	- RPM表示に使用する値をRaw N1からCorrected N1に変更し、MB-339のRPM計と一致するように
	- フラップ50%の位置が正しくなるように修正
	- ピッチラダーのみ表示するモードを追加
	- トリム変更の通知機能を追加
	- フラップ・エアブレーキ・ランディングギアの通知機能を追加
	- HMDがONの時、コックピットパネルの方向を見るとHMDを非表示にする代わりに半透明になるように変更
- 自動給油機能を追加
- スモークエフェクトの表示切替をEFB上で行えるように
- SurfOverlay（海面オーバーレイ）の表示切替をEFB上で行えるように
- 設定が自動的に保存・読み込みされる機能を追加

#### v1.7.1 (24-09-04)

- HUD/HMDそれぞれの表示・非表示設定機能を追加
- Cold&Darkスタート時にHUD/HMDが表示されない不具合を修正
- SurfOverlay（海面表示FX）をデフォルトで無効化（オプションで復活可能）

#### v1.7.0 (24-09-01)

- HUD+HMDを追加
- スモークインジケーターを追加

#### v1.6.0 (24-07-20)

- 海面を見やすくする機能「Surf Overlay」を追加

#### v1.5.0 (24-06-21)

- スモーク操作時、スモーク使用中5秒毎に鳴るサウンドエフェクトを追加
- Ripple VFX（他機スモークON時に発生するリングエフェクト）を少しだけ軽量化
- DCD F4にてドラッグシュートが表示されなくなる問題を修正

#### v1.4.0 (24-05-22)

- 機体後方のアンテナ上部付近にスモーク色のインジケーターを追加（コックピット視点でのみ有効。他の視点に切り替えてから5秒で表示されなくなります）
- 影がぼやけてしまっていた問題を修正
- リング状エフェクトの発生位置を前方へ移動
- カラースモークの発生位置が横方向にズレてしまっていた問題を修正

#### v1.3.0 (24-04-21)

- Smoke ON のタイミングでリング状のエフェクトが表示されるように（コックピット視点でのみ有効。他の視点に切り替えてから5秒で表示されなくなります）
- Smokeエフェクトが更新される距離が上昇（約3km→10km）
- スモーク噴射直後のスモークの太さを調整し、より見やすくなるようにした

#### v1.2.2 Xmas 2023 (23-12-22)

- Xmas 2023 特別バージョン

#### v1.2.2 (23-12-11)

- 編隊灯がスモークの状態と連動しなくなっていた問題を修正

#### v1.2.1 (23-12-10)

- スモークが近距離（500m）だけではなく遠距離（10km）でも同期されるように
- スモーク処理を改善し、フライトモデルをオリジナルへ完全にロールバックした

#### v1.2.0 (23-12-08)

- スモークをONにした時に余計なドラッグが増えフライトモデルに影響が出ていた問題を修正
- カラースモーク（赤・緑・黄）を追加
- [MB-339] cruise.fltを修正し、空中スポーンした際にWINGライトがOFFになるように
- [MB-339] 編隊灯をスモークの状態と連動するように
- [MB-339] 少しだけスモーク発生位置を前に移動

#### v1.1.1 (23-12-07)

- SU14によってスモークが同期しなくなった問題を修正（MB-339のみ）

#### v1.1.0 (23-08-05)

- IndiaFoxtEcho MB-339 用スモークを追加
- DC Designs F-4 v0.1.1 (23-08-04) に対応
- F-4 の照準器にSMOKEの状態を表示するように
- スモークの見た目を調整し、少し太く見やすくした
- High-Gターン時に発生するスモークのズレをマイルドにした
- 低速時・停止時にスモークが残りやすくなるように

#### v1.0.0 (23-07-22)

- 最初のバージョン🎉🎉
- DC Designs F-4 用スモークを追加
