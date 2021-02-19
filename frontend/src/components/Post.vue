<script>
import Avatar from '@/components/Avatar.vue'
import CustomText from '@/components/CustomText.vue'
import IconMore from '@/icons/more.svg'
import IconLike from '@/icons/like.svg'
import IconComment from '@/icons/comment.svg'
import IconDirect from '@/icons/direct.svg'
import IconSave from '@/icons/save.svg'
export default {
    name:"Post",
    components:{
        Avatar,
        CustomText,
        IconMore,
        IconLike,
        IconComment,
        IconDirect,
        IconSave
    }
}
</script>

<template lang="pug">
.post
  header.header.section
    .header-author
      Avatar(:size="40")
      .header-author-info
        .author-name
          CustomText(tag="b") alitigin
        .post-location
          CustomText(size="xsmal") Giresun - Tirebolu
    .header-more
      button(type="button")
        IconMore
  .post-media
    img(src="https://hedza.com/wp-content/uploads/2018/02/mountain_at_night-wallpaper-1600x900.jpg")
  .action-buttons.section
    button(type="button")
      IconLike
    button(type="button")
      IconComment
    button(type="button")
      IconDirect
    button(type="button" class="action-save")
      IconSave
  .view-count.section
    CustomText(tag="b") 1.597 like
  .post-description.section
    .author-name
      CustomText(tag="b") alitigin
    .description
      CustomText(tag="p") Takılıyoruz moruk.
  .comments.section
    .comment-author
      CustomText(tag="b") Zeyd
    .comment
      CustomText(tag="p") Harika bir manzara.
    .comment-like
      IconLike
  .comments.section
    .comment-author
      CustomText(tag="b") Ahmet
    .comment
      CustomText(tag="p") Çok iyi.
    .comment-like
      IconLike
  .comments.section
    .comment-author
      CustomText(tag="b") Mehmet
    .comment
      CustomText(tag="p") Burası neresi ?
    .comment-like
      IconLike
</template>

<style scoped>
.post {
    border-radius: 3px;
    border:1px solid rgb(var(--b6a));
}

.section {
    padding: 0px 16px 0px 16px;
}

.header {
    height: 60px;
    display: flex;
    align-items: center;
}

.header .header-author {
    display: flex;
    align-items: center;
}

.header .header-author-info {
    margin-left: 8px;
}

.header .header-more {
    margin-left: auto;
}

.action-buttons {
    height: 60px;
    display: flex;
    align-items: center;
}

.action-buttons button {
    margin-right: 16px;
}

.action-buttons .action-save {
    margin-left: auto;
    margin-right: 0;
}

.post-description {
    display: flex;
}

.post-description .author-name {
    padding-right: 10px;
}

.comments {
    display: flex;
}

.comments .comment-author {
    padding-right: 10px;
}

.comments .comment-like {
    margin-left: auto;
    align-items: center;
}

</style>