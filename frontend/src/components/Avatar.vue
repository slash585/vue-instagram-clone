<script>
export default {
    name:"Avatar",
    props: {
        src: {
            type: String,
            default: "https://instagram.fist13-1.fna.fbcdn.net/v/t51.2885-19/s150x150/46761107_314855415786824_5734866948978638848_n.jpg?_nc_ht=instagram.fist13-1.fna.fbcdn.net&_nc_ohc=0GmRZfOgEwsAX_m9ddi&tp=1&oh=060a36077ee33fbfab9898c37e3accc6&oe=60588803"
        },
        alt: {
            type: String
        },
        size: {
            type: Number
        }
    }
}
</script>

<template lang="pug">
figure.avatar
  img(:src="src" :alt="alt" :width="size" :height="size")
</template>

<style>
.avatar {
    display: inline-flex;
    padding: 3px;
    border-radius: 999px;
    background: linear-gradient(
        219deg,
        rgba(184, 63, 140, 1) 0%,
        rgba(237, 158, 90, 1) 100%
    );
}

.avatar img{
    border-radius: inherit;
    border: 2px solid white;
}
</style>