# <i class="bi bi-cloud-download-fill"></i>   インストールとアンインストール方法

「3D漫画スタジオ」のアドオンをインストールする方法について説明します。

## <i class="bi bi-file-earmark-zip-fill"></i>   アドオンファイルをダウンロード

SUPERHIVE（旧：BlenderMarket）から当アドオンを購入します。
購入したら、ダウンロードのページに進むので「3D_Manga_Studios.zip」ファイルをダウンロードしてください。

## <i class="bi bi-file-earmark-zip-fill"></i>   有料マテリアルをダウンロード

SUPERHIVE（旧：BlenderMarket）には当アドオン専用の有料マテリアルを用意しております。
購入したら、ダウンロードのページに進むので「Manga Tone Shader Assets.zip」ファイルをダウンロードしてください。
ファイル内には日本語、英語のアセットファイルをそれぞれ用意しておりますが、マテリアルは全く同じものですので１つのファイルからご利用ください。

!!! note "ダウンロードページ"
    当アドオンの販売ページはこちら

    <i class="bi bi-arrow-up-right-circle-fill"></i>   [3D漫画スタジオ ダウンロードページ](https://superhivemarket.com/products/3d-manga-studios)

## <i class="bi bi-file-earmark-arrow-down-fill"></i>   Blenderにアドオンをインストール

### インストール方法1
1. ダウンロードした「3D_Manga_Studios.zip」ファイルを解凍せずにそのまま保存しておきます。
2. Blender を起動し、「3D_Manga_Studios.zip」ファイルを Blender のウィンドウ内にドラッグ＆ドロップします。Nパネルに「3D Manga Studios」アドオンが表示されます。
!!! note "サイドパネル（Nパネル）に表示されません💦"
    ・プリファレンスのアドオンタブの右上の検索バーから「3D Manga Studios」のアドオンを探し、チェックボックスにチェックが入っているかを確認してください。有効になっていない場合はチェックを入れてください。

    ・++n++を押すとサイドパネル（Nパネル）が3Dビューポートの右端に表示されます。他に様々なアドオンも表示されている場合はスクロールすることで出現します。


### インストール方法2
1. Blender を起動し、Blender メニューから [編集] - [プリファレンス] を選択します。
2. プリファレンスウィンドウの左側にある アドオン(Add-ons) タブをクリックします。
3. ファイルブラウザが開くので、ダウンロードしたアドオンの ZIP ファイルを選択し、「アドオンをインストール(Install Add-on)」 ボタンをクリックします。
4. インストールが完了すると、アドオンリストに当アドオンが表示されます。 チェックボックスをクリックして有効にします。
!!! note "アドオンが見つかりません💦"
    アドオンが見つからない場合は、検索バーで 「3D Manga Studios」または関連する名前を検索してください。

!!! note "サイドパネル（Nパネル）に表示されません💦"
    ・プリファレンスのアドオンタブの右上の検索バーから「3D Manga Studios」のアドオンを探し、チェックボックスにチェックが入っているかを確認してください。有効になっていない場合はチェックを入れてください。

    ・++n++を押すとサイドパネル（Nパネル）が3Dビューポートの右端に表示されます。他に様々なアドオンも表示されている場合はスクロールすることで出現します。

### Manga TOne Shaderのアセットブラウザへの登録方法
1. ダウンロードした「Manga Tone Shaders.zip」のフォルダを解凍します。
2. 解凍すると以下の構成になります。

        Manga Tone Shaders/
                ├──── ★Shader Screen tones/
                │  ├──── JP/
                │  │  └──── Screen shader tones/
                │  │      ├── Screen shader tones.blend
                │  │      └── Readme_JP.txt
                │  └──── US_UK/
                │      └──── Screen shader tones/
                │          ├── Screen shader tones.blend
                │          └── Readme_JP.txt
                ├──── ★UnShader Screen tones/
                │  ├──── JP/
                │  │  └──── Screen tones/
                │  │      ├── Screen tones.blend
                │  │      └── Readme_US_UK.txt
                │  └──── US_UK/
                │      └──── Screen tones/
                │          ├── Screen tones.blend
                │          └── Readme_US&UK.txt
                └──────── Manga Tone Shader/
                        ├── Manga Tone Shader.blend
                        ├── Readme_JP.txt
                        └── Readme_US&UK.txt

3. Blender メニューから [編集] - [プリファレンス] を選択します。
4. プリファレンスウィンドウの左側にある ファイルパスタブをクリックします。
5. 「アセットライブラリ」セクションまでスクロールし、「フォルダを開く」ボタンをクリックします。
6. 解凍したフォルダ内の「Manga Tone Shader」フォルダ内のパスを選択し、「フォルダを開く」ボタンをクリックします。
7. 左下のボタンからプリファレンスを保存して閉じてください。
8. 任意のウィンドウの隅にマウスを当てると十字型のカーソルに変化するので、その状態でクリック&ドラッグしてエリアを分割します。
9. 新しいエリアのエディタタイプを「アセットブラウザ」に変更します。

## <i class="bi bi-file-earmark-x-fill"></i>   アンインストール
1. Blender メニューから [編集] - [プリファレンス] を選択します。
2. プリファレンスウィンドウの左側にある ファイルパス(Add-ons) タブをクリックします。
3. アドオンリストから「3D Manga Studios」のアドオンを探して左側にある三角をクリックして情報設定を表示してください。情報の [インターネット] の隣にある削除ボタンをクリックしてアンインストールしてください。
