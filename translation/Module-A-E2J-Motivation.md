(slide 1)
# FOSSology: License Analysis
FOSSology: ライセンス解析

Part I: Why do we need to look at licenses?  
Part I: なぜライセンスに着目しなければならないのか？

(slide 2)
## What is Open Source Software Licensing?
オープンソースソフトウェアのライセンス許諾とは何か？

Basics about Licensing  
ライセンス許諾の基本事項
- Obligations  
義務
- Restrictions  
制限事項
- Rights  
権利

Example for GPL version 2.0 (selection)
GPLバージョン2.0の例 (抜粋)
- Obligations  
義務
    - Include original source, copyrights  
    オリジナルのソースコードと著作権表示を含めること
    - Include license  
    ライセンス文を含めること
- Restrictions  
制限事項
    - Cannot be held liable  
    著作権者は一切の責任を問われない
- Rights  
許諾される権利
    - Modify  
    ソフトウェアを改変する権利
    - Distribute  
    ソフトウェアを配布する権利

Further reading:  
もっと知りたい人は…
- The Linux Foundation provides a public training including basics about licensing https://training.linuxfoundation.org/linux-courses/open-source-compliance-courses/compliance-basics-for-developers  
Linux Foundationは、ライセンス許諾の基礎を含むトレーニングを広く提供しています。 https://training.linuxfoundation.org/linux-courses/open-source-compliance-courses/compliance-basics-for-developers
- The TLDR Legal pages at https://tldrlegal.com/ provide OUTLINES about license obligations, restrictions, rights  
TL;DR Legal のページでは、多数のライセンスの義務、制限事項、権利の概要を閲覧できます。 https://tldrlegal.com/ 

(slide 3)
## Open Source Software Licenses
オープンソースソフトウェアのライセンス

Open Source Licenses  
オープンソースライセンス
- There are many of them  
多くの種類がある
- “License proliferation”  
「ライセンスの氾濫」の問題
- They can be categorized, but requires effort and assessment  
いくつかのカテゴリに分類可能であるが、労力と判断を要する
    - Copyleft vs. permissive licenses  
    コピーレフト vs. パーミッシブ
    - GPL version 2 compatibility  
    GPLバージョン2との両立性
    - Patent left effect  
    パテントレフト効果
    - … a lot more possible.  
    他にも分類可能…
    

Further reading:  
もっと知りたい人は…
- See the SPDX License List pages at http://spdx.org/licenses/ to see a selection of popular open source licenses  
SPDX License List は、よく知られているオープンソースライセンスのリストです。 http://spdx.org/licenses/

(slide 4)

## Analysis – Not Only Scanning but also Concluding
解析 - スキャンするだけではなく、結論を下すこと

### What are the goals?
ゴールは何か？  
It is about telling the software developers what to care for:  
ソフトウェア開発者に対して、何に気をつけなければならないかを伝えることがポイント

1. Identify obligations to fulfill, including providing for example  
満足しなければならない義務条件 (たとえば以下のような情報の提供) を明らかにすること  
	a) Credits (copyrights, prominent notice)  
	クレジット (著作権情報、改変の告示)  
	b) Information about licensing  
	ライセンスに関する情報  
	c) Source code  
	ソースコード  
1. Check for license compatibility  
ライセンスの両立性をチェックすること  
	a) Simple example: GPL version 2 and CC-BY-SA (copyleft effect examples)  
	コピーレフトの代表例としては、GPLバージョン2やCC-BY-SA  
1. Be able to check desired usage  
使いたい用途をチェックできるようになること  
	a) Does you business case match the licensing?  
	ライセンス許諾条件がビジネスケースに合っているか？  
	b) Is the context of usage envisaged from the OSS publishers  
	用途の背景は、そのOSSの公開者が想定しているものか？  

Further reading:  
もっと知りたい人は…
- On obligations there is the OSADL association
- They have published a set of obligation data for various licenses: https://www.osadl.org/Access-to-raw-data.oss-compliance-raw-data-access.0.html  
Open Source Automation Development Lab (OSADL) が、さまざまなライセンスの義務条件データを公開しています。https://www.osadl.org/Access-to-raw-data.oss-compliance-raw-data-access.0.html

(slide 5)
# FOSSology: Component Analysis
FOSSology: コンポーネント解析

Part II: Motivating Examples  
Part II: 一筋縄ではいかない例の数々

(slide 6)
## Examples for Licensing – Clarification Needed
ライセンス許諾の例 - 明確化が必要なもの

(all examples from the same package zlib-1.2.8.tar.gz)  
(これらの例はすべて zlib-1.2.8.tar.gz パッケージから)

- These real world examples show references to a licensing statement, which is elsewhere  
これらの例では、どこか別の場所に書かれたライセンス文への参照情報が書かれているのみである
- A scanner for text cannot generally determine the licensing from these files without capturing the particular occurrence and context  
ソースコードのテキストをツールでスキャンしても、これらの記述から前後関係を見つけ出してライセンス情報を特定することは一般的に不可能である
- A person is required to clarify the licensing  
人手でライセンス情報を明確化する必要がある


(slide 7)
## Examples for Licensing – Clarification Needed 2
ライセンス許諾の例 - 明確化が必要なもの２

(from zlib-1.2.8.tar/ zlib-1.2.8/ contrib/ amd64/ amd64-match.S)  
(zlib-1.2.8.tar/zlib-1.2.8/contrib/amd64/amd64-match.S より)

Another real world example:  
もう一つの、現実にある例：この例では、チェ・ゲバラのグッズを持っている人の使用を禁止すると書いてある
- What was meant to be fun (or a political statement), is difficult for license analysis  
面白さを狙って (あるいは政治的な意見を) 書かれたものは、ライセンス解析には厄介
- Question: Can this be ignored or shall the origination check for ownership of referred parafernalia?  
質問：これは無視して良いでしょうか、それとも、著作者はそのようなグッズの所有をチェックするのでしょうか？

(slide 8)
## Examples for Licensing – Clarification Needed 3
ライセンス許諾の例 - 明確化が必要なもの３

(TrueCrypt 7.1a Source.zip/ Common/ Cache.c)  
(TrueCrypt 7.1a Source.zip/Common/Cache.c)

Another real world example:  
もう一つの、現実にある例：  
The text is actually occurs with this formatting in file  
このテキストは、ファイルの中にこのフォーマットで実際に出現している  
Very special occurrence in fact that requires review  
レビューが必要な、極めて特別な例である

(slide 9)
## Examples for Licensing – Clarification Needed 4
ライセンス許諾の例 - 明確化が必要なもの４

(TrueCrypt 7.1a Source.zip/ Crypto/ AesSmall.h)  
(TrueCrypt 7.1a Source.zip/Crypto/AesSmall.h)

Another real world example:  
もう一つの、現実にある例：
- How does the organization decide which license to choose  
このソフトウェアを利用する組織は、どちらのライセンスを選択するか？  
- There may be an external reason for choosing either one or the another  
ライセンスを選択するにあたって、外部要因があるかもしれない

(slide 10)
## Examples for Licensing – Attention Needed 5
ライセンス許諾の例 - 明確化が必要なもの５

Another real world example:  
もう一つの、現実にある例：
- It is actually based on an MIT license text  
これはMITライセンスに基づいている
- MIT license: very popular and permissive  
MITライセンスは大変良く知られており、パーミッシブである
- Added two conditions inside the original license text
(not so permissive)  
オリジナルのライセンス文に、あまりパーミッシブではない２つの条件が追加されている
- Very hard to identify with regular expression matching  
これを正規表現によるマッチングで見つけるのはとてもむずかしい

(slide 11)
## Some Example from out in the wild (1)
その他の現実に起きている例 (1)

- 文字コード (u00A9)
- 文字化け
- ？

(slide 12)
## Some Example from out in the wild (2)
その他の現実に起きている例 (2)

- 年が変数 ($THIS_YEAR)
- 著作者が "the original author or authors" とだけ書かれていて、著作者名はjavadocに別途記載
- 著作者名をファイルの末尾に別途記載

(slide 13)
## Examples for Copyrights – Clarification Needed
著作権情報の例 - 明確化が必要なもの

1. Examples of incomplete statements  
不完全な宣言文の例  
    a) Year missing  
    年が欠落  
    b) Individual or organization missing  
    個人名や組織名が欠落
1. Copyright notice missing  
著作権の告知の欠落  
    a) Again: What about orphaned files? Who wrote them?  
    著作者が不明のファイルはどうするか？誰がそれを書いたのか？
1. Ambiguous copyright information for every file  
各ファイルの著作権情報が不明確  
    a) Copyright or copyright sign, year or years, individual or organization  
    著作権や著作権記号、年、個人名や組織名  
    b) Common understanding is covered by the Berne convention  
    共通認識はベルヌ条約でカバーされている
1. How about authored, thanks to, contributed?  
authored, thanks to, contributed などの記述をどう取り扱うか？  
    a) They do not express copyright, consult your legal counsel for guidance in these cases  
    これらは著作権を表していないので、困ったら法務部門等に相談して助言を受けること


- The Wikipedia article on the Berne convention presents the basics and origin about copyright law https://en.wikipedia.org/wiki/Berne_Convention  
ベルヌ条約についての Wikipedia の記事 https://en.wikipedia.org/wiki/Berne_Convention

(slide 14)
# FOSSology: Component Analysis
FOSSology: コンポーネント解析

Part III: Scope and Terminology  
Part III: スコープと用語

(slide 15)
## Analyzing the License Situation of a Component
ソフトウェアコンポーネントのライセンス状況を解析する

Analysis & Clarification of Compliance Issues  
コンプライアンス上の課題の解析と明確化

1. Analyzing Component vs. Usage Analysis  
コンポーネントの解析 vs. 用途の解析  
    a) On a per component basis  
    コンポーネント単位での解析  
    b) Shall not consider a particular usage case – enabling reuse of license analysis  
    一つの特定のユースケースを検討すべきではない - ライセンス解析の結果を再利用できるように  
    c) Opposed the usage clearing: considers all involved components  
    用途で分析するのではなく、関係するコンポーネントすべてを検討

(slide 16)
## Misconceptions: Other Terms and Analysis
誤った認識：その他の条件と解析

Component Analysis & Clarification of Component License Condition  
コンポーネントの解析＆コンポーネントのライセンス条件の明確化

1. License Analysis  
ライセンス解析

    a) How to call what: license analysis vs. component analysis?  
    何をどう呼ぶか：ライセンス解析か、それともコンポーネント解析か？  
    b) There is also clarifying license terms required, for example: new licenses, rare licenses, licenses written for the US law, used in Europe, etc.  
    ライセンス条件の明確化も必要である、例えば、新しいライセンス、珍しいライセンス、米国の法律に準拠して書かれたライセンスを欧州で使う場合など

1. Looking at OSS components or your own product?  
OSSコンポーネントに着目するか、それとも自社のプロダクトに着目するか？  

    a) For re-using license analysis: going OSS component by OSS component  
    ライセンス解析の結果を再利用するには、OSSコンポーネント毎に調べる  
    b) An analysis on product level considers incompatible licensing or business case compatibility  
    プロダクトレベルの解析は、ライセンスの両立性やビジネスケースとの整合性を検討する

(slide 17)
## License Analysis of a Component - Summary
コンポーネントのライセンス解析 - まとめ

1. Overall goals  
全体的なゴール  
    a) Comply with OSS community and mitigate risk  
    OSSコミュニティのライセンス条件を遵守することでリスクを軽減する  
    b) Help the engineering with definitive instructions  
    確定的な答えを出すことで、エンジニアリング部門を助ける  
    c) Building a list of reusable assets, requires usage independent clearing of component  
    コンポーネントのライセンスを、用途に依存することなく明確化することで、再利用可能な情報資産を構築する
1. How to perform a component analysis for licensing  
コンポーネントのライセンス解析  
    a) Reviewing file notices  
    ファイルの告知文をレビューする  
    b) Reviewing license texts  
    ライセンステキストをレビューする  
    c) Determining the exact text for obligations (rights, restrictions)  
    テキストそのものから義務、権利、制限事項を確定する  
    d) Identify new licenses  
    新しいライセンスを特定する  
    e) License clarification required?  
    ライセンスの明確化が必要ならば？  
     - OSS Expert group available in organisation  
     組織内のOSSエキスパート部門の活用  
     - Legal advice required  
     法的アドバイスの活用

- The FOSSology project enables the tool-based identification of licenses:  
FOSSology プロジェクトは、ツールによるライセンスの特定を可能にする
    - Finding license relevant texts  
    ライセンスに関連するテキストの検出  
    - Aggregation in a hierarchy  
    検出結果の階層的集約  
    - Highlighting text occurrences  
    テキスト中の着目部分をハイライト  
    - Identifying wording differences compared with reference texts  
    リファレンステキストと比較して差分を特定  
    - Searching for licensing phrases  
    ライセンス関連フレーズを検索  
    - Reporting of found licenses  
    検出したライセンスのレポート生成  

(slide 18)
## Thank you for your attention!
お疲れ様でした！

(C) 2016-2018  Siemens AG, The Linux Foundation


CC-BY-SA 4.0  
https://creativecommons.org/licenses/by-sa/4.0/

Internet  
https://www.fossology.org

Github  
https://github.com/fossology/fossology

もっと知りたい人は、  
https://www.spdx.org  
https://www.openchainproject.org  
https://github.com/sw360/sw360portal  


(C) 2016-2018  Siemens AG, The Linux Foundation - CC-BY-SA 4.0
