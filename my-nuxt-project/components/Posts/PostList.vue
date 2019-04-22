<template>
    <section class="posts-list">
                <PostPreview 
                id="1"
                :is-admin="isAdmin"
                thumbnail="https://cloud.oracle.com/opc/images/trends-hightech-4.jpg"
                title="Hello There!"
                previewText="This is my first post!"
                />
                <PostPreview 
                id="2"
                :is-admin="isAdmin"
                title="Hello There - the second time!"
                thumbnail="https://cloud.oracle.com/opc/images/trends-hightech-4.jpg"
                previewText="This is my second post!"
                />
                <PostPreview 
                id="3"
                :isAdmin="isAdmin"
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
    },
    props:{
        isAdmin:{
            type: Boolean,
            default:false
        }
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
