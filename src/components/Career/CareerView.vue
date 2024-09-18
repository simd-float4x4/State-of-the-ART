<template>
    <h1 class="section-title">CAREER</h1>
    <div>
        <CareerItemView 
            companyName="D社" 
            history="2024年3月〜2024年9月" 
            projectName="iOSアプリケーションの新規開発（0→1）" 
            projectStack="Swift5／SwiftUI／VIPER／Moya／GitHub"
            projectConcept="マンガアプリ（主幹サービス）のリニューアル対応" 
            :whatIachieved=ninethItem >
        </CareerItemView>
        <CareerItemView 
            companyName="D社" 
            history="2023年11月〜2024年2月" 
            projectName="iOSアプリケーションの新規開発（0→1）" 
            projectStack="Swift5／UIKit／Moya／GitHub"
            projectConcept="ビジネス系オウンドメディアのアプリリニューアル" 
            :whatIachieved=seventhItem >
        </CareerItemView>
        <CareerItemView 
            companyName="D社" 
            history="2023年9月〜2023年11月末" 
            projectName="iOSアプリケーションの新機能開発" 
            projectStack="Swift5／UIKit／MVC／GitHub"
            projectConcept="マンガアプリの機能拡張と新機能開発" 
            :whatIachieved=sixthItem >
        </CareerItemView>
        <CareerItemView 
            companyName="C社" 
            history="2023年7月〜2023年8月末" 
            projectName="品質保証／品質管理業務" 
            projectConcept="インディーズゲームデベロッパーのデバッグ業務／メタバースのデバッグ業務など" 
            :whatIachieved=fifthItem >
        </CareerItemView>
        <CareerItemView 
            companyName="B社" 
            history="2022年12月〜2023年3月" 
            projectName="スマートフォンアプリケーションの受託開発（クロスプラットフォーム）" 
            projectStack="Flutter3.3.10／Dart2.8.16" 
            projectConcept="某中枢中核都市における行政情報一元化スマートフォンアプリ（Android担当）" 
            :whatIachieved=fourthItem >
        </CareerItemView>
        <CareerItemView 
            companyName="B社" 
            history="2022年7月〜2022年11月" 
            projectName="Webアプリケーションの受託開発" 
            projectStack="PHP8／Laravel8／CentOS／MySQL5.7.19（+ javaScript）" 
            projectConcept="学校指定スポーツ用品店における商品発注管理/在庫管理システム" 
            :whatIachieved=thirdItem >
        </CareerItemView>
        <CareerItemView 
            companyName="B社" 
            history="2022年4月〜2022年9月" 
            projectName="さまざまなWebアプリケーション開発" 
            projectStack="PHP／Laravel／Java／SpringBoot／javaScript" 
            projectConcept="新卒研修（ECサイトの改修）／証憑管理システムの保守／勤怠管理システムの補修 etc." 
            :whatIachieved=secondItem >
        </CareerItemView>
        <CareerItemView 
            companyName="A社" 
            history="2020年6月〜2020年12月" 
            projectName="iOSアプリケーションの機能拡張・不具合修正" 
            projectStack="Swift4／UIKit+InterfaceBuilder／MVC／GitHub" 
            projectConcept="モバイルオーダー領域・店舗内注文管理用タブレットアプリ" 
            :whatIachieved=firstItem >
        </CareerItemView>
    </div>
</template>

<script>
import CareerItemView from "./CareerItemView.vue"

export default {
  components: {
      CareerItemView
  },
  data() {
    return {
        ninethItem: [
            "Moya（GET, POST, DELETE）を用いた画面の実装",
            "AppsFlyer, Firebaseのセットアップ"
        ],
        seventhItem: [
            "Moya（GET）を用いた画面の実装",
            "新規登録／ログインの実装",
            "ポイント履歴画面の実装"
        ],
        sixthItem: [
            "特定の情報を表示するエリアを別セクションに移動させる",
            "SPM対応／Privacy Manifest対応"
        ],
        fifthItem: [
            "インディーズゲームが展示会に向けて開発中のゲームタイトルの試遊版のデバッグ業務",
            "プラットフォーム移植中のアダルト系ゲームのデバッグ業務",
            "某大手会社が運用するメタバースプラットフォームのデバッグ業務"
        ],
        fourthItem: [
            "トップ画面・ベースUIの開発",
            "アプリ内複数機能の実装",
            "アプリ内複数機能についてUserStatusによってコンテンツの出し分けをする処理の実装",
            "Python + Google Calendar APIを用いたカレンダー設定処理",
            "軽いテストコードの実装　など",
        ],
        thirdItem: [
            "CRUD機能を有する複数画面のフルスクラッチ実装",
            "ステータスコードの取得及び400／500エラー発生時の画面遷移",
            "テーブルのレコードを表示する画面で検索機能の実装",
            "軽微な不具合修正"
        ],
        secondItem: [
            "ECサイトの不具合修正　チームリーダーとして開発を主導（新卒研修）",
            "既存の実装を参考にしながら新機能の追加（証憑管理システム）",
            "軽微な不具合修正（勤怠管理システム）"
        ],
        firstItem: [
            "税率の計算方法の修正",
            "配色の修正",
            "クーポンが反映されない不具合の修正",
            "清算合計金額の修正",
            "自発的なドキュメンテーション作成と報告"
        ]
    }
  }
}
</script>