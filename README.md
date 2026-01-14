# LangChain GraphRAG Demo with Neo4j

このリポジトリは、LangChainとNeo4jを使用したGraphRAG（グラフ構造を活用したRAG）のサンプル実装。

Qiita記事「[GraphRAGをわかりやすく解説 #LLM](https://qiita.com/ksonoda/items/98a6607f31d0bbb237ef)」の内容を参考に、Pythonコードとして実行可能な形式にまとめている。

## 特徴

* **Graph Construction**: `LLMGraphTransformer` を使用して、非構造化テキストからノードとリレーションシップを自動抽出・構築。
* **Hybrid Search**: Neo4jVectorを使用したベクトル検索と、Cypherクエリを使用したグラフ構造検索を組み合わせたハイブリッド検索を実装。
* **Sample Data**: デモとして「サザエさん」の家族関係テキストを使用し、複雑な人間関係の推論をテストできる。

## 前提条件

* Python 3.9 以上
* [Neo4j](https://neo4j.com/) データベース（AuraDB Free Tier推奨）
* OpenAI API Key（GPT-4モデル推奨）
