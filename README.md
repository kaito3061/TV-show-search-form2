# テレビ番組検索アプリ

このアプリは、[TVmaze API](https://www.tvmaze.com/api) を使ってテレビ番組を検索できる、シンプルなWebアプリケーションです。  
検索結果は番組の画像付きで表示され、画像をクリックすると番組の詳細ページにアクセスできます。

## 📺 デモ動画
![demo](https://github.com/user-attachments/assets/2bf62496-10d9-41be-b49a-a13d7443c41a)

## 開発の背景

このアプリは、Web API の活用方法や JavaScript の実践的な使い方を学ぶために制作しました。
私が映画やテレビ番組を見ることが好きなのでそこで自分でも使える番組検索ができるものが欲しかったので開発に至りました。
このアプリケーションを通して、以下のスキルを身につけることを目的としています。

- 外部API（TVmaze）の利用方法の理解
- 非同期通信（Axios）の扱い方
- DOM操作やイベント処理の基本
- 実用的な検索インターフェースの構築

また、実際に動作するWebアプリを作ることで、学習内容を形にし学習内容の理解を深めるといった目的があります。




 🚀 主な機能

- 番組名で検索が可能
- 番組画像付きの検索結果を表示
- 画像はクリック可能で、番組の詳細ページへリンク
- HTML・JavaScript・Axiosで構成された軽量なアプリ

🔧 使用技術

- HTML5
- JavaScript (ES6)
- Axios（API通信に使用）


💡 使い方

1. `tv.html`,`tv2.js` をご使用のPCにダウンロードしていただき、 `tv.html` をブラウザで開きます。
2. 検索フォームにテレビ番組名を入力します。
3. 「検索」ボタンを押すと、画像付きで結果が表示されます。
4. 画像をクリックすると、番組の詳細ページが新しいタブで開きます。
5. また新たに番組を検索すると、前回の検索の結果を画面から削除し、新しく検索した番組が表示されます。
6. もし、検索した番組に画像がなかった場合は『見つかりませんでした』と表示します。
7. またこの『見つかりませんでした』の表現も新たに番組検索をすると消えるようにしています。
　

## なぜAPI通信にAxiosを使用したか
1. もともとFetch APIから学習していてFetchでの実装を検討したのですが、AxiosはデフォルトでJSONを自動的にパースしてくれたり、タイムアウト設定やヘッダーの追加などが簡単にでき、エラーハンドリングも明確に書ける（※まだ実装はできていないが、今後機能が増えた時のため）ため、実装や保守が非常にしやすいと感じたからです。
2. 学習中の自分にとってもドキュメントが充実していて、実務的な書き方を学びながら自然にコードの品質を上げられる点が魅力でした。

##  実装予定の機能（２０２５年８月を目処に予定）

- 🔁 検索履歴の保存（ローカルストレージを活用）
- ⭐ お気に入り登録機能（気になる番組を保存）
- 🔍 ジャンル・言語による絞り込み検索
- 📱 レスポンシブ対応（スマホ・タブレットでの最適表示）
- 🌐 多言語対応（日本語/英語 切り替え機能）
- 🧩 Reactによるリファクタリング（関数の分離・保守性向上）
- 🌏デプロイ（VercelかNetlifyを予定）

## 📈 今後の改善方針

- APIの仕様やレスポンス構造を事前に正確に把握して、開発時のつまずきを減らします。
- データがないときのプレースホルダー画像表示や、エラーメッセージのデザインなど、ユーザー体験の改善に注力します。
- 機能の追加に伴い、コードの可読性・再利用性を考慮して、Reactや設計パターンの導入を検討中です。







# Explanation in English 
# 📺 TV Show Search App

This is a simple web application that allows users to search for TV shows using the [TVmaze API](https://www.tvmaze.com/api).  
Search results are displayed with show images, and clicking on an image takes the user to the detailed page for that show.

## 📹 Demo Video  
![demo](https://github.com/user-attachments/assets/2bf62496-10d9-41be-b49a-a13d7443c41a)

## 🎯 Motivation

This app was created as a project to practice using Web APIs and improve practical JavaScript skills.  
Since I enjoy watching movies and TV shows, I wanted to create a tool I could personally use to search for TV content.

Through this project, my main learning objectives were:

- Understand how to work with external APIs (TVmaze)
- Learn to handle asynchronous communication using Axios
- Practice DOM manipulation and event handling
- Build a user-friendly and functional search interface

Additionally, developing a fully functional web application helped solidify my learning and provided a real-world context for applying new skills.

---

## 🚀 Key Features

- Search TV shows by name
- Display search results with images
- Clickable images link to each show's detailed page
- Lightweight app built with HTML, JavaScript, and Axios

---

## 🛠️ Technologies Used

- HTML5  
- JavaScript (ES6)  
- Axios (for API communication)

---

## 💡 How to Use

1. Download `tv.html` and `tv2.js` to your local machine.
2. Open `tv.html` in your web browser.
3. Enter a TV show name into the search form.
4. Click the "Search" button to display the results with images.
5. Click on an image to open the show's detailed page in a new tab.
6. New searches will replace previous results automatically.
7. If no image is available for a result, a "Not Found" message is displayed. This message also disappears on a new search.

---

##  Why Axios for API Communication?

1. Although I initially learned using Fetch API, I chose Axios because it simplifies many tasks such as JSON parsing, adding headers, setting timeouts, and clear error handling — making the app more maintainable and scalable.
2. Axios also provides excellent documentation, which made it easier for me as a learner to write more professional and clean code.

---

##  Planned Features (Targeting August 2025)

- 🔁 Save search history (local storage)  
- ⭐ Favorite show bookmarking  
- 🔍 Filter by genre and language  
- 📱 Responsive design (mobile/tablet support)  
- 🌐 Multilingual support (English/Japanese toggle)  
- 🧩 Refactor with React for modular and scalable structure  
- 🌍 Deploy to Vercel or Netlify

---

## 📈 Future Improvements

- Better understanding of the API's response structure to reduce bugs  
- Add placeholder images and improve error UI for a better user experience  
- Consider using frameworks like React and architectural patterns to improve maintainability as the app grows








