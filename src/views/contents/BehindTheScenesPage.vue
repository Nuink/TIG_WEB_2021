<template>
  <div id="behind-the-scenes-page">
    <content-page-template
      :videoSrc="videoSrc"
      :contentGenre="contentGenre"
      :contentTitle="contentTitle"
      :contentDescriptions="contentDescriptions"
      :isOurs="true"
      :announceSentences="announceSentences"
    >
      <template #body>
      </template>
    </content-page-template>
  </div>
</template>

<script>
import ContentPageTemplate from '@/components/template/ContentPageTemplate.vue'
export default {
  components: {
    ContentPageTemplate
  },
  setup() {
    const videoSrc = ""
    const contentGenre = "Behind The Scenes"
    const contentTitle = "新しい学校のリーダーズ feat. Nu ink."
    const contentDescriptions = [
      "10月10日に六本木ヒルズアリーナで行われたINNOVATION WORLD FESTA 2021にて、2日目のオープニングアクトを務めた「新しい学校のリーダーズ feat. Nu ink.」のライブステージの舞台裏をまとめました。", 
      "映像製作やリハーサルの様子を撮影し、ライブステージの演出が完成に至るまでの過程を公開。本番前の楽屋や舞台袖の様子も撮影し、ライブを終えた新しい学校のリーダーズさんにインタビューをさせていただきました。また、映像制作者とNu ink.メンバーによるイノフェスを振り返っての対談も。ぜひご覧ください。"  
    ]
    const announceSentences = [
      "※本作はライブ配信時のみ公開する予定です。"
    ]
    
    return { videoSrc, contentGenre, contentTitle, contentDescriptions, announceSentences }
  }
}
</script>
