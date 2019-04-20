<template>
    <section class="posts-list">
                <PostPreview 
                id="1"
                thumbnail="https://cloud.oracle.com/opc/images/trends-hightech-4.jpg"
                title="Hello There!"
                previewText="This is my first post!"
                />
                <PostPreview 
                id="2"
                title="Hello There - the second time!"
                thumbnail="https://cloud.oracle.com/opc/images/trends-hightech-4.jpg"
                previewText="This is my second post!"
                />
                <PostPreview 
                id="3"
                title="Hi"
                thumbnail="https://cloud.oracle.com/opc/images/trends-hightech-4.jpg"
                previewText="This is my third post!"
                /> 
        </section>
</template>

<script>
    import PostPreview from '@/components/Posts/PostPreview'
                                
export default {
    components:{
        PostPreview
    }
}
</script>

<style scoped>
    .featured-posts {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}

</style>
