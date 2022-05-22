<!-- 普通使用方式 -->
<image-wrapper :src="imageSrc" :desc="context"></image-wrapper>

<!-- 使用 slot 的 desc 方式 -->
<image-wrapper :src="imageSrc">
<span slot="desc">{{ context }}</span>
</image-wrapper>

<script>
import ImageWrapper from '@/components/ImageWrapper';

export default {
  // 引入组件
  components: {
    ImageWrapper
  },
  data () {
    return {
      context: '示意图',
      imageSrc: 'https://os.alipayobjects.com/rmsportal/mgesTPFxodmIwpi.png'
    }
  }
}
</script>

<style scoped>

</style>
