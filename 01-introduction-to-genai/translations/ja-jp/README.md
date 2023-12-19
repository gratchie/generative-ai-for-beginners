# 生成 AI と大規模言語モデルの紹介

[![Introduction to Generative AI and Large Language Models](../../images/01-lesson-banner.png?WT.mc_id=academic-105485-yoterada)](https://youtu.be/vf_mZrn8ibc?WT.mc_id=academic-105485-yoterada)

> *(上記の画像をクリックすると、レッスン・ビデオを表示します)*

生成 AI は、テキストや画像などのコンテンツを生成する人工知能です。この技術が素晴らしいのは、AI を誰にでも使えるようにしている所で、自然言語で書いた文章やテキスト・プロンプトだけで利用できる点です。
価値あることを成し遂げるために、Java や SQL のような言語を学ぶ必要はありません。自分の言葉で要望を伝えるだけで、AI モデルから提案が返ってきます。この技術を使えば、報告書を書いたり理解したり、アプリケーションを作成したりといったことが、わずか数秒で可能になります。その可能性と影響力は計り知れません。

このカリキュラムで、スタートアップ企業が教育分野で新たな可能性を切り開くために生成 AI をどのように利用しているか、またその応用に伴う社会的影響や、技術的な制限によって避けられない課題にどう対処しているかを詳しく見ていきます。

## レッスン内容の紹介

このレッスンでは、下記の内容について説明します。

* ビジネスシナリオの紹介: スタートアップのアイデアとミッション
* 生成 AI と、技術的な歴史背景
* 大規模言語モデルの内部動作
* 大規模言語モデルの主な機能と実用的なユースケース

## 学習目標

このレッスンを修了すると、下記を理解できます：

* 生成 AI とは何か、そして大規模言語モデルの仕組みを理解する
* 教育シナリオに重点を置き、さまざまなユース・ケースで大規模言語モデルを活用する方法を理解する

## シナリオ:　教育関連事業をターゲットにするスタートアップ企業

生成 AI は AI 技術の最高峰に位置付けられ、かつては不可能と思われていたことにも挑戦し、新たな可能性を広げています。
生成 AI モデルは様々な機能と用途で利用可能ですが、このカリキュラムでは、架空のスタートアップ企業を通じて教育分野でどのように革新していくのかを学んでいきます。この新興企業を「スタートアップ」と呼ぶことにします。
スタートアップは、教育の領域において下記の野心的な目標を持って事業を行っています。

> *世界規模で学習の利便性を高め、教育に対する平等な機会を実現し、学習者一人ひとりの要望に応える個別学習体験を提供します。*

スタートアップ・チームは、現在最も強力なツールである大規模言語モデル(LLM)を活用せず、この目標を達成する事は難しいと考えています。

生成 AI を利用すると、生徒は 24 時間いつでも問い合わせ可能なバーチャルの教師から、大量の情報や例を得られるようになり、教師も生徒の成績を評価しフィードバックするために、新しいツールが使えるようになると考えられ、現在の学習方法や指導方法に革命をもたらすと考えられています。

![モニターを見つめる5人の若い学生 -  DALLE2 による画像](../../images/students-by-DALLE2.png?WT.mc_id=academic-105485-yoterada)

まず、カリキュラム全体を通じて使用する、基本的な概念と用語を定義しましょう。

## 生成 AI はどのようにして生まれたのでしょうか？

最近発表された、生成 AI モデルは大きな注目を集めていますが、この技術は数十年にわたる開発の歴史があり、初期の研究は 1960 年代までさかのぼります。そして今、AI 技術は [OpenAI の ChatGPT](https://openai.com/chatgpt) や [Bing Chat](https://www.microsoft.com/edge/features/bing-chat?WT.mc_id=academic-105485-yoterada) のように会話能力を有するなど、人間の認知能力を持つレベルにまで達しています。また、これらのチャットシステムは、Bing の Web 検索における会話でも GPT モデルを採用しています。

AI の歴史を振り返ると、初期の AI のプロトタイプは、タイプライター式のチャットボットで、専門家集団から抽出した知識をベースに、それをコンピューターに表現していました。知識ベースによる回答は、入力テキスト内に出現するキーワードがトリガーになっていました。しかし、タイプライター式のチャットボットは、スケール・アウトが難しい事がすぐに分かりました。  

### 統計学的手法を基にした AI 技術： 機械学習

1990年代に入り、テキスト解析に統計学的手法を応用したことで、転換点が訪れました。  
これにより、データからパターンを学習できる新しいアルゴリズムが開発されました。これは「機械学習」として知られ、学習にプログラミングを必要としません。この手法を用いることで、機械は人間の言語理解を再現することが可能になります。テキストとラベルの組み合わせで訓練された統計モデルが、メッセージの意図を示す定義済みのラベルで、未知の入力テキストを分類することができるようになります。

### ニューラルネットワーク(神経回路網)と最新の仮想アシスタント

最近では、より大量のデータと、複雑な計算を処理できるハードウェアの進化が、AI 分野の研究をさらに促進し、ニューラル・ネットワークやディープラーニング・アルゴリズムと呼ばれる高度な機械学習アルゴリズムの開発につながりました。  

ニューラルネットワーク（特に再帰型ニューラルネットワーク - RNN と呼ばれる）は、自然言語処理を飛躍的に進化させ、文章中に含まれる単語の意味を、文脈を考慮して評価し、より有益な方法でテキストの意図を表現できるようになりました。

この技術は、21 世紀の初頭に登場したバーチャル・アシスタントの基盤となり、人の言葉を読み取って要求を識別し、それに応じた行動を取ることができます。例えば、事前に用意したスクリプトで応答したり、外部サービスを利用することが含まれます。

### 現在の生成 AI

このような経緯を経て、今日における生成 AI が誕生しました。これはディープラーニングのサブセットとして捉えることができます。  

![AI, ML, DL and Generative AI](../../images/AI-diagram.png?WT.mc_id=academic-105485-yoterada)

長年の AI 研究を経て、*トランスフォーマー* と呼ばれる新しいモデルのアーキテクチャが登場し、RNN の限界を越え、より長文テキストのシーケンスを入力として受け取ることができるようになりました。トランスフォーマーは、アテンションメカニズム(注意機構)を採用しており、モデルが、受け取った入力に対して異なる重み付けを行うことができます。これにより、テキスト内の単語の並ぶ順番に関わらず、最も関連性の高い情報が集中している部分に「より多くの注意を払う」ことができます。  

最近の生成 AI モデルの多くは、文章の入出力を行う「大規模言語モデル（LLMs）」とも呼ばれており、実際にこのアーキテクチャに基づいています。これらのモデルが注目される理由は、書籍、記事、ウェブサイトなど様々な情報源から、膨大なラベルなしデータとして訓練されているにも関わらず、創造性を備え文法も正しい文章を作り出すのが特筆すべき点です。したがって、これらのモデルは、機械が単に入力されたテキストを「理解」する力を飛躍的に向上させただけでなく、人間の言葉で独自の回答を作り出す力も実現しました。  

## 大規模言語モデルの仕組みを教えてください？

次の章では、さまざまな種類の生成 AI モデルについて詳しく説明しますが、その前に、OpenAI の GPT（Generative Pre-trained Transformer）モデルを中心に、大規模言語モデルがどのように機能するのかを確認しましょう。  

* **トークナイザー、テキストから数値へ**: 大規模言語モデルは、テキストを入力として受け取り、テキストを出力として生成します。ただし、統計モデルのため、テキストシーケンスよりも数値の方が、とてもうまく機能します。そこでモデルに対するすべての入力は、コア・モデルが使用する前に、トークナイザーで処理されます。トークンは文字の塊で、可変数の文字から構成されています。トークナイザーは、入力された文字列をトークン毎に分割し、トークン配列に格納する処理を行います。その後、各トークンはトークン・インデックスと結びつけられます。トークン・インデックスは元のテキストのチャンク(断片)を整数で符号化したものになります。

![トークン化の例](../../images/tokenizer-example.png?WT.mc_id=academic-105485-yoterada)

* **出力トークンの予測**: 入力として n 個のトークンを受け取ると（モデルによって n の最大値は異なります）、モデルは出力として 1 個のトークンを予測する力を持っています。この予測されたトークンは次の反復処理の入力に追加され、拡張ウィンドウ・パターンにより、ユーザーが 1 つ以上の文を回答として得られるようになります。これは、ChatGPT を試したことがある人なら、文の途中で時々処理が停止するような動きにつながる理由です。

* **選考過程、確率分布**: モデルは、現在のテキストの順番の後ろに続く文字を、確率的に可能性の高い結果に基づいて出力トークンを選びます。これは、モデルが過去の訓練に基づいて、「次に出現するトークン」の各選択肢についてどれだけの確率があるかを計算し、その全体の確率分布を推定しているからです。ただし、得られた分布から最も確率の高いトークンが必ず選ばれるとは限りません。この選択には、ある程度のランダム性が導入されており、モデルが決定的に振る舞わないようにしています。- つまり同じ入力に対して必ずしも同じ出力が得られるわけではないのです。このランダム性は、創造的な思考過程を模倣するために導入され、温度(temperature)というパラメータで調整ができます。

## スタートアップは、大規模言語モデルをどのように活用できるでしょうか？

大規模言語モデルについて、内部動作の理解が深まったところで、ビジネス・シナリオも視野に入れて、大規模言語モデルをうまく活用するための、実践的な例をいくつか見てみましょう。

大規模言語モデルが最も得意とするのは、自然言語で記述されたテキストの入力から、新しいテキストを作ることだと述べました。

しかし、具体的にどのようなテキストの入力と出力を想定しているのでしょうか？
大規模言語モデルの入力は「プロンプト」と呼ばれ、出力は「コンプリーション」と呼ばれています。これは、モデルが現在の入力に続く次のトークンを生成する仕組みを表しています。これからプロンプトの意味や、モデルを最大限に活用するための設計方法について詳しく見ていくことになりますが、とりあえず現時点では、プロンプトは以下のような要素が含まれるとお考えください：

* モデルに対して、期待する出力の種類を指定する**指示**。この指示には、場合によって具体例やその他のデータを追加で組み込むことがあります。  

    1. 記事、書籍、製品レビューなどの要約と、非構造化データから知見（インサイト）の抽出
    
    訳者追記：
    - Can you please summarize the following text for me ?
    - 以下のテキストの内容を要約していただけますか？
    
    ![Example of summarization](../../images/summarization-example.png?WT.mc_id=academic-105485-yoterada)
    
    <br>
    
    1. 記事、エッセイ、課題などのアイデアとデザインの作成

    訳者追記：
    - Please write an assignment for high school students including four open-ended questions about Louis XIV and his court. 
    - 高校生用の課題を作成します。ルイ14世と彼の宮廷について、自由に回答できる 4 つの質問を作成してください。
    
    ![Example of creative writing](../../images/creative-writing-example.png?WT.mc_id=academic-105485-yoterada)
    
    <br>

* エージェントに対して会話形式で尋ねる**質問**

    訳者追記：
    - Who is Louis XIV and why he is an important historical character?
    - ルイ14世はどういう人で、なぜ彼は歴史的に重要な人物なのですか？
![Example of conversation](../../images/conversation-example.png?WT.mc_id=academic-105485-yoterada)

<br>

* 続きを書く**文章の一節**で、実際には文章の執筆支援を要求しています

    訳者追記：
    - Louis XIV is an important historical character because
    - ルイ14世が歴史的に重要な人物である理由は

![Example of text completion](../../images/text-completion-example.png?WT.mc_id=academic-105485-yoterada)

<br>

* **プログラムコード**の一部と、そのコードに関する説明や記述を求める要望、または特定の作業を行うコードの生成を依頼するコメント

    訳者追記：
    - A Python function to sum two numbers a and b
    - 二つの数値aとbを合計するPython関数

![Coding example](../../images/coding-example.png?WT.mc_id=academic-105485-yoterada)

<br>

上記に挙げた例は基本的なものであり、大規模言語モデルの機能を全て網羅したわけではありません。教育分野に限らず、生成 AI が持つ潜在的な可能性と利点を示しました。

また、生成 AI モデルの出力結果は決して完璧ではなく、場合によってはモデルの創造性が逆効果となって、現実を曲解するような言葉を組み合わせたり、不快な言葉を組み合わせて作り出すこともあります。また、生成 AI は知能を持っているわけではありません。少なくとも、批判的思考や創造的推理、感情知能を含む広い意味において知能はありません。そして決定論的でもなく、信頼性もありません。なぜなら、誤った参照や内容、声明などの作り話が、正しい情報と混ざり合って、説得力のある自信に満ちた言葉で提示されることがあるからです。次のレッスンでは、これらすべての制限に対処し、それらを軽減するために何ができるかを見ていきます。

## 課題

この課題では、「生成 AI」に関する知識を深め、まだ生成 AI が導入されていない領域を特定し、そこにどう取り込めるかを検討してください。従来の方法と比べて、どのような違いがあるでしょうか？これまでにできなかったことが、実現可能になるか、作業の速度が上がるかご検討ください。「問題点」「AIの活用方法」「導入による効果」といった見出しを用いて、理想の AI スタートアップについて 300 文字で概要をまとめてください。可能であれば、ビジネスプランも記述してください。  

この課題を達成すれば、マイクロソフトのスタートアップ向けインキュベータープログラム、[Microsoft for Startups Founders Hub](https://www.microsoft.com/startups?WT.mc_id=academic-105485-yoterada) への応募資格が得られるかもしれません。Azure や OpenAI の使用クレジット、メンタリング、その他多くの支援を提供していますので、詳細はウェブサイトをご覧ください。

## 知識チェック

大規模言語モデルについてどれが正しいですか?

1. 毎回まったく同じ回答が返ってきます
1. 物事を完璧に行い、計算をしたり、正しく動作するコードを生成するのに最適です
1. 同じプロンプトを使用しても、回答が異なる場合があります。また、テキストやコードなど最初に何らかのヒントを得るために利用するのには最適です。しかし、得られた結果は改善する必要があります。

A: 3, 大規模言語モデル（LLM）は決定的ではなく、出力結果にはばらつきがありますが、温度設定を調整することで、ばらつきを制御することが可能です。完璧な結果を期待するべきではありません。LLM は皆様の負担を軽減するために存在し、物事を始める際に最初の良い出発点を提供します。 ただ多くの場合、段階的に改善していく必要があるでしょう。

## お疲れ様でした! 次のレッスンを続ける

このレッスンを修了後、[生成 AI 学習コレクション](https://aka.ms/genai-collection?WT.mc_id=academic-105485-yoterada) に進んで、生成 AI の知識をさらに深めましょう!

レッスン 2 にお進みください。そこでは、[様々な LLM の調査と比較](../../../02-exploring-and-comparing-different-llms/translations/ja-jp/README.md?WT.mc_id=academic-105485-yoterada)方法に焦点を当てます！