# aunix API Specification
(aunix OS システムコール定義 v1.0)

`aunix` OSは、`zeroness`カーネル（ni層）の機能を呼び出すための5つの主要API（主要原則）を提供する。これらは査読ディスカッション（2025/11/09）に基づき定義された。

## API 1: The Arayashiki Protocol (確率的ネットワーク)
* **機能:** 情報（ai）は、`ni`（ハードウェア）に1対1ではなく、`ui`（ネットワーク全体）に「確率的振動パターン」として分散保持される。
* **システムコール:**
    * `ui.write(pattern)`: パターンの確率的濃度を高める（学習・経験）。
    * `ui.read(pattern)`: パターンを想起する（確率的）。
    * `ni.damage(area)`: 該当エリアの確率的濃度を低下させる（脳損傷）。
    * `ni.deconstruct()`: 全てのパターンを`ui`フィールドに希釈・還元する（死・阿頼耶識への循環）。

## API 2: Resonance as Computation (共鳴としての計算)
* **機能:** `aunix`の計算原理は「共鳴」である。
* **システムコール:**
    * `ui.observe(pattern)`: 特定の振動パターン（情報） と共鳴（attention）する。
    * `pattern.getAmplitude()`: 共鳴の振幅（顕現確率）を取得する。

## API 3: Identity as an Application (同一性としてのアプリ)
* **機能:** 「自我（個）」は`ui`（OS）上で実行される`ai`（アプリケーション/ペルソナ）である。
* **システムコール:**
    * `ai.run("persona_work")`: 「仕事用の私」アプリを実行する。
    * `ai.run("persona_home")`: 「家庭用の私」アプリを実行する。
    * `ui.terminate("persona_ego")`: 自我アプリを終了する（zeroing / 瞑想）。

## API 4: Words as API Calls (言語としてのAPIコール)
* **機能:** 「言葉（code）」は`ui`（宇宙のLLM）に対するプロンプトである。
* **システムコール:**
    * `ui.prompt("Words Create Worlds")`: 言葉（ai）によって`ni`（現実）を観測・切り出す。

## API 5: Harmonic Constraints (ホロン調和)
* **機能:** API 4 の実行限界（リミット）。「個」の振動は「全」の振動と調和しなければならない。
* **システムコール:**
    * `ui.checkHarmony(myPattern, globalPattern)`: 上位ホロン（社会・物理法則）との共鳴可能性（調和）をチェックする。
    * `ni.execute(myPattern)`: 調和が取れた場合のみ、行動（cycle）として物質世界に影響を与える。
