# <i class="bi bi-menu-button-fill"></i>   Manga Tone Shaderの仕様
![Manga Tone Shaderのオブジェクト](assets/img/JP/MTS section.png)

「Manga Tone Shader」はトゥーンレンダリング向けに漫画・コミック表現を特化したトゥーンシェーダーになります。

## <i class="bi bi-exclamation-diamond-fill"></i>  特徴
一般的なトゥーンシェーダーと異なる特徴は専用のライティングによって照りの範囲ごとに色を割り当てれらるところです。

仕組みは３つのライト（キーライト・フィルライト・バックライト）にはそれぞれ赤（#ff0000）、緑（#00ff00）、青（#0000ff）の色で照らされており、照らされるそれぞれの色のみ抽出しそれぞれの範囲ごとに色や模様が映し出されています。

!!! note "補足"
	- ３つのライトは「B:ライティング」のコレクション内で作成されるライトコレクションに含まれています。
	- Manga Tone Shaderの照りの範囲はオフセット値だけでなく、ライトコレクション内の各ライトの強さによっても変化します。ライトの強さを調整してからManga Tone Shaderのオフセット値を調整することをお勧めします。
照らされた面ごとに各カラー入力を設けており、カラー入力の下にあるマテリアルの入力欄には付属の有料マテリアルをドラッグ&ドロップすることでその面に模様を映し出すことも可能です。

## <i class="bi bi-stack"></i>  Manga Tone Shaderの構成
Manga Tone Shaderは以下のような構造になっています。

![Manga Tone Shaderのレイヤー構造](assets/img/JP/MTS layer.png)

## <i class="bi bi-list-task"></i>  プロパティの一覧と効果

### プロパティの目次

  - <a href="#base-tone">ベーストーン</a>
  - <a href="#key-tone">キートーン</a>
  - <a href="#fill-tone">フィルトーン</a>
  - <a href="#back-tone">バックトーン</a>
  - <a href="#shadow">影</a>
  - <a href="#sub-outline">サブアウトライン</a>
  - <a href="#ao">AO (アンビエントオクルージョン)</a>
  - <a href="#soft-shadow-tone">ソフトシャドウトーン</a>
  - <a href="#hard-shadow-tone">ハードシャドウトーン</a>
  - <a href="#gloss">光沢</a>
  - <a href="#anisotropy">異方性</a>
  - <a href="#mat">マット</a>
  - <a href="#rim-light">リムライト</a>

<div style="display: flex !important; gap: 5px !important; align-items: flex-start !important;">

<div style="flex: 0 0 50% !important; padding: 0 !important; margin: 0 !important;">

<h3 id="nodes-image" style="margin-top: 0 !important;">ノードの実画像</h3>
<img src="/assets/img/JP/MTS%20property%20list.png" alt="Manga Tone Shaderのノード画像" style="width: 100% !important; display: block !important; margin: 0 !important; padding: 0 !important;">

</div>

<div style="flex: 0 0 50% !important; padding: 0 !important; margin: 0 !important; padding-left: 5px !important;">

<h3 id="property-list" style="margin-top: 0 !important;">プロパティ一覧</h3>

<h4 id="base-tone">ベーストーン</h4>
<ul>
<li><strong>カラー</strong>: ベースとなる色を設定します。</li>
<li><strong>マテリアル</strong>: アセットブラウザに登録されたマテリアルをドロップする欄です。</li>
</ul>

<h4 id="key-tone">キートーン</h4>
<ul>
<li><strong>カラー</strong>: キーライトが当たる部分の色を設定します。また下にある欄にマテリアルをドロップすることでマテリアルの模様を表示することもできます。</li>
<li><strong>マテリアル</strong>: アセットブラウザに登録されたマテリアルをドロップする欄です。</li>
<li><strong>キーライト オフセット</strong>: キーライトのオフセットを調整します。</li>
<img src="/assets/img/compare/key_offsets.png" alt="キーライト オフセットの比較画像">
</ul>

<h4 id="fill-tone">フィルトーン</h4>
<ul>
<li><strong>カラー</strong>: フィルライトが当たる部分の色を設定します。また下にある欄にマテリアルをドロップすることでマテリアルの模様を表示することもできます。</li>
<li><strong>マテリアル</strong>: アセットブラウザに登録されたマテリアルをドロップする欄です。</li>
<li><strong>フィルライト オフセット</strong>: フィルライトのオフセットを調整します。</li>
<img src="/assets/img/compare/fill_offsets.png" alt="フィルライト オフセットの比較画像">
</ul>

<h4 id="back-tone">バックトーン</h4>
<ul>
<li><strong>カラー</strong>: バックライトが当たる部分の色を設定します。また下にある欄にマテリアルをドロップすることでマテリアルの模様を表示することもできます。</li>
<li><strong>マテリアル</strong>: アセットブラウザに登録されたマテリアルをドロップする欄です。</li>
<li><strong>バックライト オフセット</strong>: バックライトのオフセットを調整します。</li>
<img src="/assets/img/compare/back_offsets.png" alt="バックライト オフセットの比較画像">
</ul>

<h4 id="shadow">影</h4>
<p>影の表現に関する設定です。</p>
<ul>
<li><strong>カラー</strong>: シャドウの色を設定します。</li>
<li><strong>マテリアル</strong>: アセットブラウザに登録されたマテリアルをドロップする欄です。</li>
<li><strong>シャドウ不透明度</strong>: 影の不透明度を調整します。</li>
<img src="/assets/img/compare/shadow_oppacity.png" alt="シャドウ不透明度の比較画像">
<li><strong>輝度</strong>: 影の輝度を調整します。</li>
<img src="/assets/img/compare/shadow_strong.png" alt="影の輝度の比較画像">
<li><strong>コントラスト</strong>: 影のコントラストを調整します。</li>
<img src="/assets/img/compare/shadow_contrast.png" alt="シャドウのコントラストの比較画像">
</ul>

<h4 id="sub-outline">サブアウトライン</h4>
<p>影のサブアウトラインに関する設定です。</p>
<ul>
<li><strong>カラー</strong>: オブジェクトの内側の輪郭色を設定します。</li>
<li><strong>マテリアル</strong>: アセットブラウザに登録されたマテリアルをドロップする欄です。</li>
<li><strong>不透明度</strong>: サブアウトラインの不透明度を調整します。</li>
<img src="/assets/img/compare/sub_outline_opacity.png" alt="サブアウトライン不透明度の比較画像">
<li><strong>サイズ</strong>: サブアウトラインのサイズを調整します。</li>
<img src="/assets/img/compare/sub_outline_size.png" alt="サブアウトラインのサイズの比較画像">
<li><strong>影のサイズ</strong>: 影のサイズを調整します。</li>
<img src="/assets/img/compare/sub_outline_shadow size.png" alt="影のサイズの比較画像">
</ul>

<h4 id="ao">AO (アンビエントオクルージョン)</h4>
<p>アンビエントオクルージョンに関する設定です。</p>
<ul>
<li><strong>不透明度</strong>: AO の不透明度を調整します。</li>
<img src="/assets/img/compare/AO_opacity.png" alt="AO不透明度の比較画像">
<li><strong>シャドウ不透明度</strong>: AO のシャドウ不透明度を調整します。</li>
<img src="/assets/img/compare/AO_shadow_opacity.png" alt="AOシャドウ不透明度の比較画像">
<li><strong>マスク</strong>: AOの影を描画する範囲をマスクで設定します。下に付随する画像選択欄から新規のボタンを押すことで白黒のテクスチャを作成できます。</li>
<img src="/assets/img/compare/AO_mask.png" alt="AOマスクの比較画像">
<li><strong>ソフトハードスイッチ</strong>: ソフトシャドウとハードシャドウの切り替えを調整します。</li>
<img src="/assets/img/compare/soft_hard_switch.png" alt="ソフトハードスイッチの比較画像">
</ul>

<h4 id="soft-shadow-tone">ソフトシャドウトーン</h4>
<ul>
<li><strong>ソフト強度</strong>: ソフトシャドウの強度を調整します。</li>
<img src="/assets/img/compare/soft_strong.png" alt="ソフト強度の比較画像">
</ul>

<h4 id="hard-shadow-tone">ハードシャドウトーン</h4>
<ul>
<li><strong>ハード強度</strong>: ハードシャドウの強度を調整します。</li>
<img src="/assets/img/compare/hard_strong.png" alt="ハード強度の比較画像">
</ul>

<h4 id="gloss">光沢</h4>
<p>光沢の表現に関する設定です。</p>
<ul>
<li><strong>カラー</strong>: 光沢の色を設定します。</li>
<li><strong>マテリアル</strong>: アセットブラウザに登録されたマテリアルをドロップする欄です。</li>
<li><strong>不透明度</strong>: 光沢の不透明度を調整します。</li>
<img src="/assets/img/compare/gloss_opacity.png" alt="光沢不透明度の比較画像">
<li><strong>輝度</strong>: 光沢の輝度を調整します。</li>
<img src="/assets/img/compare/gloss_strong.png" alt="光沢の輝度の比較画像">
<li><strong>コントラスト</strong>: 光沢のコントラストを調整します。</li>
<img src="/assets/img/compare/gloss_contrast.png" alt="光沢のコントラストの比較画像">
<li><strong>広がり</strong>: 光沢の広がりを調整します。</li>
<img src="/assets/img/compare/gloss_spread.png" alt="光沢の広がりの比較画像">
<li><strong>オフセットX</strong>: 光沢のX軸オフセットを調整します。</li>
<img src="/assets/img/compare/gloss_offsets_x.png" alt="光沢のオフセットXの比較画像">
<li><strong>オフセットZ</strong>: 光沢のZ軸オフセットを調整します。</li>
<img src="/assets/img/compare/gloss_offsets_z.png" alt="光沢のオフセットZの比較画像">
</ul>

<h4 id="anisotropy">異方性</h4>
<p>異方性シェーディングに関する設定です。</p>
<ul>
<li><strong>カラー</strong>: 髪の艶などになる部分の色を設定します。また下にある欄にマテリアルをドロップすることでマテリアルの模様を表示することもできます。</li>
<li><strong>マテリアル</strong>: アセットブラウザに登録されたマテリアルをドロップする欄です。</li>
<li><strong>不透明度</strong>: 異方性の不透明度を調整します。</li>
<img src="/assets/img/compare/anisotropy_oapcity.png" alt="異方性不透明度の比較画像">
<li><strong>輝度</strong>: 異方性の輝度を調整します。</li>
<img src="/assets/img/compare/anisotropy_strong.png" alt="異方性の輝度の比較画像">
<li><strong>コントラスト</strong>: 異方性のコントラストを調整します。</li>
<img src="/assets/img/compare/anisotropy_contrast.png" alt="異方性のコントラストの比較画像">
<li><strong>密度</strong>: 異方性の密度を調整します。</li>
<img src="/assets/img/compare/anisotropy_density.png" alt="異方性の密度の比較画像">
<li><strong>シャドウ不透明度</strong>: 異方性のシャドウ不透明度を調整します。</li>
<img src="/assets/img/compare/anisotropy_shadow_opacity.png" alt="異方性のシャドウ不透明度の比較画像">
<li><strong>シャドウコントラスト</strong>: 異方性のシャドウコントラストを調整します。</li>
<img src="/assets/img/compare/anisotropy_shadow_contrast.png" alt="異方性のシャドウコントラストの比較画像">
<li><strong>オフセットZ</strong>: 異方性のZ軸オフセットを調整します。</li>
<img src="/assets/img/compare/anisotropy_ofssets_z.png" alt="異方性のオフセットZの比較画像">
<li><strong>カメラ視点オフセット</strong>: カメラ視点からのオフセットを調整します。</li>
<img src="/assets/img/compare/anisotropy_camera_ofssets.png" alt="異方性のカメラ視点オフセットの比較画像">
</ul>

<h4 id="mat">マット</h4>
<p>質感表現を疑似的に再現するテクスチャに関する設定です。</p>
<ul>
<li><strong>カラー</strong>: AOの影を描画する範囲をマスクで設定します。下に付随する画像選択欄から新規のボタンを押すことで白黒のテクスチャを作成できます。</li>
<img src="/assets/img/compare/mat_color.png" alt="マットカラーの比較画像">
<li><strong>不透明度</strong>: マットの不透明度を調整します。</li>
<img src="/assets/img/compare/mat_opacity.png" alt="マット不透明度の比較画像">
<li><strong>輝度</strong>: マットの輝度を調整します。</li>
<img src="/assets/img/compare/mat_strong.png" alt="マットの輝度の比較画像">
<li><strong>コントラストA</strong>: マットのコントラストAを調整します。</li>
<img src="/assets/img/compare/mat_contrast_a.png" alt="マットのコントラストAの比較画像">
<li><strong>コントラストB</strong>: マットのコントラストBを調整します。</li>
<img src="/assets/img/compare/mat_contrast_b.png" alt="マットのコントラストBの比較画像">
</ul>

<h4 id="rim-light">リムライト</h4>
<p>リムライトの表現に関する設定です。</p>
<ul>
<li><strong>カラー</strong>: サブアウトラインの内側の輪郭部分の色を設定します。また下にある欄にマテリアルをドロップすることでマテリアルの模様を表示することもできます。</li>
<li><strong>マテリアル</strong>: アセットブラウザに登録されたマテリアルをドロップする欄です。</li>
<li><strong>不透明度</strong>: リムライトの不透明度を調整します。</li>
<img src="/assets/img/compare/rim_light_oapcity.png" alt="リムライト不透明度の比較画像">
<li><strong>コントラスト</strong>: リムライトのコントラストを調整します。</li>
<img src="/assets/img/compare/rim_light_contrast.png" alt="リムライトのコントラストの比較画像">
<li><strong>幅</strong>: リムライトの幅を調整します。</li>
<img src="/assets/img/compare/rim_light_width.png" alt="リムライトの幅の比較画像">
<li><strong>オフセットX</strong>: リムライトのX軸オフセットを調整します。</li>
<img src="/assets/img/compare/rim_light_offsets_x.png" alt="リムライトのオフセットXの比較画像">
<li><strong>オフセットZ</strong>: リムライトのZ軸オフセットを調整します。</li>
<img src="/assets/img/compare/rim_light_offsets_z.png" alt="リムライトのオフセットZの比較画像">
</ul>

</div>

</div>
