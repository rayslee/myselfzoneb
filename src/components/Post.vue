<template>
    <div class="post">
        <div class="head">
            <div class="publisher">
            <el-avatar :size="35" :src="circleUrl" />
            <span class="name">黄晓丹</span>
            <el-icon><CirclePlus /></el-icon>
            </div>
            <div class="operations">
            <el-icon><Star /></el-icon>
            <el-icon><Hide /></el-icon>
            </div>
        </div>
        <div class="content">
            <el-image :src="contentImgUrl" />
            <div class="desc">
            <h3>陶渊明也烦恼</h3>
            <h4>给家长的传统文化启蒙课</h4>
            <p>
                传统文化教育是当下家长们关心却往往不得要领的难题：国学班比比皆是、毁誉参半，如何看待？当下流行的“大语文”是否给了孩子学习古典文化的通途？学校教育中要求的《弟子规》等文本是否给了孩子真正的传统文化熏陶？古典诗词之美、古典文学之妙，怎样传达给孩子？中国古典的审美如何传承给现代的孩子？
            </p>
            </div>
        </div>
    </div>
</template>

<script setup lang="ts">
import circleUrl from '@/assets/images/hxd.jpeg'
import contentImgUrl from '@/assets/images/s33895502.jpg'
</script>

<style scoped lang="scss">
.post {
  background: #fff;
  margin: 10px 0;
  border-radius: 10px;
}

.head {
  display: flex;
  justify-content: space-between;

  .publisher {
    padding: 5px;
    display: flex;

    .name {
      padding: 0 5px 0px 10px;
    }

    .name, .el-icon {
      align-self: center;
    }
  }

  .operations .el-icon {
    padding: 5px;
  }
}

.content {
  height: 18vh;
  overflow: hidden;
  display: flex;
  justify-content: space-between;

  .el-image {
    width: 25%;
    padding: 10px;    
  }

  .desc {
    width: 70%;
    padding: 10px 10px 10px 0;
    
    display: flex;
    flex-direction: column;

    h4 {
      padding: 5px 0;
      font-size: 12px;
    }

    p {
      display: -webkit-box;
      /* 垂直对齐 */
      -webkit-box-orient: vertical;
      /* 几行省略 */
      -webkit-line-clamp: 4;
      overflow: hidden;
      text-overflow: ellipsis;
    }

  }
}
</style>